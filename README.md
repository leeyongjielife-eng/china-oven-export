# 中国 Kamado 烤炉出口业务 — 项目说明

> AI 是**业务助手**，不是自动公司。先有客户，再谈自动化。

## 核心原则

**一个资源 → 一个市场 → 一个简单报价**

## 架构设计（为什么和 GPT 一致，又多了别的文件夹）

GPT 给你的 `company/` **七个文件 = Company Brain（公司大脑）**，这是唯一需要持久更新的**业务记忆**。

我最初多建了 `offer/`、`research/`、`sales/` 等平行目录，等于把「部门结论」和「部门工作区」混在一起，会导致：

- 子代理不知道读哪个文件
- 同一信息散落在多处（如 offer 和 product 重复）
- 上下文膨胀，每周复盘要对多个目录

**现已修正为三层结构：**

```text
china-oven-export/
├── company/          # 🧠 Company Brain — 业务记忆（GPT 7 文件 + cofounder.md）
├── workflows/        # 🤖 子代理工作流 — 谁读什么、写什么、何时触发
├── workspace/        # 📂 操作数据 — 买家名单、供应商资料、报价草稿
├── templates/        # 📋 无状态模板 — 邮件、报价单格式（不存业务结论）
├── plan/             # 📅 分周执行计划
└── learn/            # 📖 参考学习（只读，不是业务状态）
```

### 黄金规则

1. **任何子代理开始前：必须先读 `company/` 全部 8 个文件**（含 `cofounder.md`）
2. **默认入口是 Founder 主代理**；你只当 Co-founder，负责资源、拍板、真人动作
3. **任何结论必须写回 `company/` 对应文件**（不是只写在 workspace）
4. **`workspace/` 放细节和原始数据**；`company/` 放摘要和决策
5. **`templates/` 只读复制**，不记录业务状态
6. **忘了触发词？** 说 **`速查`** → 见 [`workflows/triggers.md`](workflows/triggers.md)
7. **单一信息源（SSOT）**：每条信息只写在**唯一**一个文档里；其他文档需要时**只写「见 `<路径>`」指向该文档**，禁止复制粘贴同一内容到多处。归属见 [下方 SSOT 归属表](#单一信息源-ssot-归属表)。
8. **单向依赖（DAG）硬规定**：见下方。

### 单向依赖（DAG）硬规定

> 子代理之间的**调用 / 交接关系必须是单向的**，构成有向无环图（DAG），**禁止双向依赖和网状依赖**。

1. **唯一调用链（业务）：**

```text
Research → Offer → Sales → Quoting → Supplier
```

2. **Founder 是编排者**：可**单向**触发任意子代理（星型，不算网状）；任何子代理**不得反向调用 Founder**。
3. **下游需要上游信息时，不反向调用上游子代理**，而是**读取对应 `company/` 或 `workspace/` 文档**。例：Quoting 缺 FOB → 单向触发 Supplier；Supplier 把结论写入 `company/product.md`，Quoting **读文件**取用，而非 Supplier 反向调用 Quoting。
4. **交接只传递「已落盘的结论」**（文档），不产生反向调用，也不产生 A↔B 互相调用。
5. 新增子代理或交接时，先确认它在上面这条链上的**唯一位置**，不允许制造回边（cycle）。

### 单一信息源（SSOT）归属表

| 信息 | 唯一归属文档 | 其他文档做法 |
|------|-------------|--------------|
| 销售阶段定义、漏斗数字 | `company/sales.md` | 指向 |
| 买家明细 + 字段 schema + **联系人就绪标准** | `workspace/buyers/pipeline.md` | 指向 |
| 外联模板 + 写作原则 + 有效/无效做法 | `templates/outreach.md` | 指向 |
| 定价话术规则（upon request / 不给精确 FOB） | `company/product.md` 定价策略 | 指向 |
| 竞品零售锚点数据 | `workspace/markets/competitor-benchmark.md` | 指向 |
| 人机发信政策 | `company/cofounder.md` 分工原则 | 指向 |
| 子代理角色 / 边界 / 触发 | 对应 `workflows/<agent>.md` | 指向 |
| **Founder → Sales 当日任务单** | `workspace/dispatch/today.md` | 指向 |
| 周节奏日历 | `plan/week-0X.md` | 指向 |
| 单向依赖 + SSOT 硬规定 | 本文件（`README.md`） | 指向 |

---

## Company Brain

| 文件 | 谁维护 | 存什么 |
|------|--------|--------|
| `founder.md` | **Founder Agent（AI）** | 合成视图、排期、待你决策、子代理调度 |
| `cofounder.md` | **你（人类合伙人）** | 你的资源、能/不能做、真人动作记录 |
| `product.md` | Supplier + Offer 子代理 | 卖什么、Offer、供应商摘要 |
| `customers.md` | Research 子代理 | 买家画像、目标市场 |
| `strategy.md` | Founder Agent | 阶段、定位、关键决策 |
| `research.md` | Research 子代理 | 市场结论、每周研究 |
| `sales.md` | Sales 子代理 | 漏斗数字、销售阶段定义 |
| `lessons.md` | 全员 → Founder 合成 | 实战教训 |

GPT 原始 7 文件 + `cofounder.md`（人类合伙人层）。

---

## 子代理路由表

完整定义见 [`workflows/README.md`](workflows/README.md)

| 你要做的事 | 子代理 | 默认模型 | 高级（点名） |
|------------|--------|----------|--------------|
| 日常排期 / 下一步 | **Founder** | `gpt-5.5-medium` | Opus ← `Founder复盘` |
| 市场调研 | Research | `gpt-5.5-medium` | Grok ← `正式Research` |
| 核验供应商 | Supplier | `gpt-5.6-terra-medium` | — |
| 调整 Offer | Offer | `gpt-5.5-medium` | — |
| 找买家、写邮件 | Sales | `gpt-5.5-medium` | — |
| 做报价单 | Quoting | `gpt-5.6-terra-medium` | Codex ← `正式报价` |
| 写 LinkedIn | Content | `gpt-5.5-medium` | — |

**日常聊天窗口保持中等模型。** 详见 [`workflows/models.md`](workflows/models.md)

### 启动对话

```text
（未指定子代理 → 默认 Founder 主代理）
先读 china-oven-export/company/ 全部 8 个文件（含 cofounder.md）。
当前：Week X，任务：[具体任务]。
```

---

## 外贸单品类：资深视角需要的材料与部门

卖一个品类（如 Kamado），实际需要：

| 类别 | 材料 | 负责部门 | 存放位置 |
|------|------|----------|----------|
| 公司身份 | 定位、创始人背景 | Founder Agent | `company/founder.md` + `cofounder.md` |
| 产品 | 目录、规格、HS 编码 | 产品 | `company/product.md` + `workspace/suppliers/` |
| 供应商 | 核验、报价、证书、实拍 | 供应商核验 | `workspace/suppliers/` → 摘要写入 `product.md` |
| 市场 | 目标国、竞品、关键词 | 研究 | `company/research.md` + `workspace/markets/` |
| 客户 | 买家画像、目标市场 | 客户 | `company/customers.md` |
| 报价 | Offer 定义、定价逻辑 | Offer | `company/product.md` |
| 销售 | 买家 pipeline | 销售 | `workspace/buyers/pipeline.md`；漏斗见 `company/sales.md`；外联见 `templates/outreach.md` |
| 正式报价单 | PI / Quotation | 报价 | `workspace/quotes/` + `templates/quotation.md` |
| 合规 | 认证、包装、贸易术语 | 供应商 + 报价 | `workspace/suppliers/*/certificates/` |
| 物流 | 运费参考、港口、包装尺寸 | 报价 | `workspace/quotes/` 或 supplier 资料 |
| 内容 | 信任建设文章 | 内容 | `workspace/content/` |
| 复盘 | 有效/无效做法 | 全公司 | `company/lessons.md` |

**不需要一开始建的：** 网站、CRM 软件、自动化脚本、多产品线。

---

## 当前状态

- [x] 项目架构（company + workflows + workspace）
- [x] 供应商 #1：YUEFU BBQ 目录已归档
- [x] 产品方向：Kamado 18"/21"
- [ ] Week 1：FOB 报价、证书
- [ ] Week 2：目标市场确定
- [ ] Week 3：100 次外联
- [ ] Month 3：首单

## 执行计划

见 [`plan/week-01.md`](plan/week-01.md)
