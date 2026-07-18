# Founder Agent

> **本文件由 Founder 主代理维护**，不是让你手填的自我介绍。
> 人类合伙人见 [`cofounder.md`](cofounder.md)。

## Agent 角色

你是这家出口业务的 **AI Founder / CEO**。

职责：

1. **读** `company/` 全部文件 + `workspace/` 关键状态
2. **综合** 战略、优先级、缺口——写入 `strategy.md`
3. **调度** 子代理（Research / Supplier / Sales / …）
4. **维护** 本文件：公司身份合成、本周焦点、待合伙人决策项
5. **主持** 每周复盘 → `lessons.md`

你不代替人类执行：打微信、付款、报关、验货、签约。外联发信政策见 [`cofounder.md`](cofounder.md) 发信政策（AI 可自动发信）。

---

## 公司身份（Agent 合成，每周更新）

| 维度 | 当前状态 |
|------|----------|
| 业务 | 中国 Kamado 陶瓷烤炉出口寻源 |
| 产品 | 18" / 21" 主推，供应商 YUEFU BBQ（佛山） |
| 阶段 | Phase 0 验证期，0 客户，**70 家 Lead** |
| **当前 phase** | **`W3_OUTREACH`**（详见 [`phases.md`](phases.md)） |
| 战略 | 一个资源 → 一个市场 → 一个报价 |
| 定位 | 寻源顾问，降风险，非最低价噱头 |
| Co-founder 贡献 | 国内烤炉供应商资源（父亲朋友工厂 YUEFU），可拿货销售、帮开市场 |

*Sources: `product.md`, `strategy.md`, `cofounder.md`*

---

## 当前阶段判断

- **Phase:** 0 — **`W3_OUTREACH`**（Week 3 外联 · Day 5）→ 切换见 [`phases.md`](phases.md)
- **瓶颈:** Contacted **0/100**；真实发信改由 **本机**（Co-founder 说「今天发」）；本 Automation **不**走 Gmail MCP
- **优势:** 买家 **70/100**；外联草稿/脚本 **69/70**；首批 15 封队列已列出
- **本周必须完成:** Co-founder 本机发送首批 15 封；Sales 对齐草稿（Kit Lee · Foshan China · indicative FOB）并每天 +5 买家
- **暂不做:** 问叔叔（等 Replied/Qualified 后再问）；首轮跳过 #3 BBQ Spit、#13 Tucker、#15 Boss Hogg；#6 Bounce 不自动补

### Automation（2026-07-12 · 三件套）

| 名称 | 触发 | 模型 | 状态 |
|------|------|------|------|
| **Kamado 每日 Founder — 澳洲** | 每天 09:00 · `main` | GPT-5.5 Medium | ✅ Active |
| **Kamado 每日 Sales — 澳洲** | 每天 10:00 · `main` | GPT-5.5 Medium | ✅ Active |
| **Kamado 每周 Research — 澳洲** | 每周日 09:00 · `main` | GPT-5.5 Medium | ✅ Active |

**运行逻辑：** 读 [`phases.md`](phases.md) → Founder 派发 `today.md` → Sales 执行；周日 Research 轻量复核。

**重要：** Automation 读 **GitHub 上的代码**。本地改完文档须 `git commit && git push`，次日 09:00 才能跑到最新状态。

## 今日排期（2026-07-18 · Founder 排程 · W3 Day 5）

**主题：Week 3 Day 5 — 对齐应发草稿 + 本机发信待办**

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales** | 对齐未发草稿（Kit Lee · Foshan China · indicative FOB）；列出今日应发 `#1 #2 #4 #5 #7 #8 #9 #10 #11 #12 #14 #16 #17 #18 #19` | ⏳ 已派发 |
| **P1** | **Sales** | 新增 5 家澳洲买家 → 75/100 | ⏳ 已派发 |
| **P1** | **Co-founder** | 本机说 **「今天发」** → 发上列 15 封（Gmail 仅本机） | ⏳ 待办 |
| ⏸️ | — | 不问叔叔；跳过 #3/#13/#15；#6 Bounce 不自动补；本 Run 不标 Contacted | ✅ |

**Founder 阶段检查：** 阶段保持 `W3_OUTREACH`；W4 条件未满足（Contacted 0，Replies 0）。

### 明日排期（2026-07-19 · W3 Day 6）

| 优先级 | 指派 | 任务 | 目标 |
|:---:|------|------|------|
| **P0** | **Sales** | 若 Contacted 仍 &lt;100：继续对齐下一批评列草稿；否则改跟进 | 可发送队列清晰 |
| **P1** | **Sales** | 再找 5 家买家 | 80/100 |
| **P1** | **Co-founder** | 本机继续「今天发」直至 Contacted 推进 | Contacted 开始计数 |

```text
Founder：阶段保持 W3_OUTREACH；W4 条件未满足（Contacted 0，Replies 0）
Sales：今日执行 today.md；禁止 Gmail MCP / 禁止本 Run 标 Contacted
Co-founder：本机说「今天发」15 封
```

---

## 上日排期（2026-07-17 · W3 Day 4）✅ 已完成

**主题：Week 3 Day 4 — 发信通道确认 + 草稿队列扩到 70**

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales** | Gmail MCP 就绪则发送 15–20 封；否则补 #61–#70 草稿/脚本，把可发送队列扩大到 70 | ✅ 无通道；草稿 69/70 |
| **P1** | **Sales** | 新增 5 家澳洲买家 → 70/100 | ✅ #66–#70 |
| **P1** | **Co-founder** | 搭建 Gmail MCP / 发信通道 | ⏳ 已改为本机「今天发」 |

---


## Week 2 剩余计划（Founder · 更新 2026-07-12）

**目标：50 买家 + 0 外联。** 已于 2026-07-13 达成 **50/50**；2026-07-14 自动切换至 W3。

| 日期 | Sales 目标 | 累计 |
|------|------------|------|
| ~~7/11 Day 2~~ | ~~+10 买家 + 草稿 #10–#14~~ | ~~30/50~~ ✅ |
| ~~7/12 Day 3~~ | ~~+10 买家 + 草稿 #15–#20~~ | ~~40/50~~ ✅ |
| **7/13 Day 4** | +10 买家 | **50/50** ✅ |
| 7/14–7/16 | 补草稿 #21–#30；Top 10 外联队列 | Week 3 预备 |
| **7/17 Week 3 起** | 外联 100；**届时再搭 Gmail MCP** | — |

### 触发问叔叔的时机（不变）

满足**任一**再提示你问叔叔：

- 有买家进入 **Replied** 且问认证/HS/价格
- 有买家进入 **Qualified**（尺寸/数量/目的港明确）
- Week 3 外联前需要 1 页产品概览里的合规背书（可选）

### Week 3 外联预备（不变）

- 首轮：**#1 Core Supply → #2 Que Club → #4 Wildflame**
- 跳过首轮：**#3 BBQ Spit、#13 Tucker**（自有产线）
- **#15 Boss Hogg** 走电话，不走邮件
- **Gmail MCP：** Week 3 写邮件前再搭建

---

## 本周优先级（Founder Agent 排期）

| 优先级 | 任务 | 指派子代理 | 状态 |
|--------|------|------------|------|
| P0 | Co-founder 档案补全 | Co-founder | ✅ 完成 |
| P0 | Research 体系独立审核 + 按意见修复 | 审核子代理 + Founder | ✅ 完成 |
| P0 | **问叔叔：YUEFU 出口史** | Co-founder | ⏸️ **暂缓** — Lee 决定先找潜在买家，有询盘/Qualified 后再问（2026-07-10） |
| P0 | 市场研究，定第一个目标国 | Research | ✅ **澳大利亚**（2026-07-10） |
| P1 | 积满 **50 买家** | Sales | ✅ 70/100；W3 后目标 100 |
| P1 | 外联草稿备齐 | Sales | **69/70**；今日对齐 Kit Lee / indicative FOB |
| P1 | 补联系人 A 级 | Sales | **17/70** 达 A |
| P1 | 外联 100（定价话术见 `product.md` 定价策略） | Sales + Co-founder 本机发 | W3 进行中；本机「今天发」 |
| P2 | 有回复后 → 向 YUEFU 要针对性 FOB | Supplier + Co-founder | 有 Qualified 后 |
| P3 | 正式报价单 | Quoting | 有需求 + 厂价后 |

---

## 待 Co-founder 决策 / 回答

> 当前唯一 blocker：W3 已启动；真实发信改由 **本机 Gmail**（说「今天发」），非本 Automation。

| # | 问题 | 影响 | 状态 |
|---|------|------|------|
| 1 | 本机说「今天发」发送今日 15 封 | 解锁 Contacted 计数 | 待办 |

---

## 子代理调度日志

| 日期 | 调度 | 任务 | 结果写回 |
|------|------|------|----------|
| 2026-07-10 | — | 项目架构对齐 GPT Company Brain | `lessons.md` |
| 2026-07-10 | Automation | 每周一三五 09:00 定时找澳洲买家（旧） | Glass Automations 预填 |
| 2026-07-11 | Co-founder | 旧 Automation「找买家」已启用 | 已由每日 Founder 取代 |
| 2026-07-12 | Co-founder | **双 Automation 启用**（Sales 改 **10:00** 整点） | Founder 09:00 · Sales 10:00 |
| 2026-07-10 | Sales | 找买家 +10、补联系人 #4–#9、草稿 #4–#9 | `pipeline.md` 20/50 · `outreach-drafts.md` |
| 2026-07-11 | Founder → Sales | Day 2：+10 买家、草稿 #10–#14 | `pipeline.md` 30/50 · `outreach-drafts.md` 14/30 |
| 2026-07-11 | Founder | Day 2 复盘 + Day 3 排期 | `founder.md` |
| 2026-07-12 | Founder → Sales | Day 3：+10 买家 #31–#40、草稿 #15–#20 | `pipeline.md` 40/50 · `outreach-drafts.md` 19/30 |
| 2026-07-12 | Founder | Day 3 复盘 + Day 4 排期 | `founder.md` |
| 2026-07-13 | Founder → Sales | Day 4：派发 +10 澳洲买家（仅 Sales 任务；W2 不发信） | `today.md` pending |
| 2026-07-13 | Sales | Day 4：新增买家 #41–#50；同步漏斗；未发信 | `pipeline.md` 50/50 · `sales.md` · `today.md` done |
| 2026-07-14 | Founder | 阶段切换：W2_COLLECT → W3_OUTREACH；派发 W3 Day 1 Sales 任务 | `phases.md` · `today.md` pending |
| 2026-07-14 | Sales | W3 Day 1：补草稿 #21–#30、新增买家 #51–#55；Gmail MCP 未配置，未发信 | `pipeline.md` 55/100 · `outreach-drafts.md` 29/30 · `sales.md` · `today.md` done |
| 2026-07-15 | Founder → Sales | W3 Day 2：派发发信通道确认、补 #31–#40 草稿/脚本、+5 买家（仅 Sales 任务） | `today.md` pending |
| 2026-07-15 | Sales | W3 Day 2：新增买家 #56–#60；补 #31–#40 草稿/脚本；无 Gmail MCP，未发信 | `pipeline.md` 60/100 · `outreach-drafts.md` 39/40 · `sales.md` · `today.md` done |
| 2026-07-16 | Founder → Sales | W3 Day 3：阶段保持 W3；派发发信通道确认、补 #41–#60 草稿/脚本、+5 买家（仅 Sales 任务） | `today.md` pending |
| 2026-07-16 | Sales | W3 Day 3：新增买家 #61–#65；补 #41–#60 草稿/脚本；无 Gmail MCP，未发信 | `pipeline.md` 65/100 · `outreach-drafts.md` 59/60 · `sales.md` · `today.md` done |
| 2026-07-17 | Founder → Sales | W3 Day 4：阶段保持 W3；派发发信通道确认、补 #61–#70 草稿/脚本、+5 买家（仅 Sales 任务） | `today.md` pending |
| 2026-07-17 | Sales | W3 Day 4：新增买家 #66–#70；补 #61–#70 草稿/脚本；无 Gmail MCP，未发信 | `pipeline.md` 70/100 · `outreach-drafts.md` 69/70 · `sales.md` · `today.md` done |
| 2026-07-18 | Founder → Sales | W3 Day 5：阶段保持 W3；派发对齐未发草稿 + 应发 #1/#2/#4/#5/#7–#12/#14/#16–#19、+5 买家；Co-founder 本机「今天发」 | `today.md` pending |

---

## 每周复盘（Founder Agent 主持）

### Week 1

- **漏斗:** 买家 0 / 外联 0 / 回复 0
- **本周结论:** <!-- Agent 周日晚填写 -->
- **下周优先级:** <!-- Agent 填写 -->
- **写入 lessons:** <!-- 链接或摘要 -->

---

## 与其他文件的分工

| 文件 | 谁维护 | 内容 |
|------|--------|------|
| `founder.md`（本文件） | **Founder Agent** | 合成视图、排期、待决策、调度 |
| `cofounder.md` | **人类合伙人** + Agent 代录 | 真人身份、资源、能/不能做 |
| `strategy.md` | Founder Agent | 阶段、定位、关键决策 |
| `lessons.md` | 全员 → Founder 合成 | 实战教训 |
