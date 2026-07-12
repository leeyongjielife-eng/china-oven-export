# Research Playbook — WHO / WHERE / PAIN 分步手册

> 按 GPT Core 原则执行。每步有**数据来源**、**怎么做**、**写到哪里**。

---

## 总流程（5 步 × 1 国约 30–40 分钟）

```text
WHERE（需求） → WHO（买家） → PAIN（痛点） → 竞品 → 打分
```

正式 `正式Research` 时：对短名单 **至少 3 国** 跑完，再选 1 国。

---

## Step 1 — WHERE：需求在哪

### 问什么

- 这个国家从中国进口 grill / kamado / BBQ 设备多吗？
- 终端消费者认 Kamado 吗？（还是只认 gas grill）

### 怎么做

| 动作 | 主工具 | 备选方案（主源打不开/收费时） | 记录 |
|------|--------|------------------------------|------|
| 搜进口数据 | **UN Comtrade**（免费官方） | Volza / ImportYeti（付费墙，可访问再补充） | 进口量趋势 |
| 看零售热度 | Amazon.[country] "kamado grill" | 目标国站受限 → 用美国站评论提取通用痛点 | Bestseller 价格带 |
| 看文化信号 | Reddit r/kamadojoe, r/biggreenegg, 当地 BBQ 论坛 | Google `site:reddit.com kamado [country]` | 讨论活跃度 |

#### ⚠️ HS 编码（正式 Research 第一步先核实）

**不要用 8514**（那是工业电炉，旧烘焙炉方案残留）。Kamado 陶瓷炭烤炉可能归入：

- **HS 6914** — 陶瓷制品细分
- **HS 7321** — 非电动家用炉具（含烤架/炭烤炉）

**核实方法：** 查 YUEFU 报关单上的实际 HS code（问叔叔一句即可），或看 Alibaba 同类 listing 标注的 HS code，确认后再批量查 UN Comtrade。

### 写到哪里

- 分数 → `country-scoring.md` 维度 A
- 笔记 → `candidates/[country].md` 或 `company/research.md` 每周日志

---

## Step 2 — WHO：谁买

### 买家类型（按可接触性排序假设）

| 优先级 | 类型 | 怎么找 | 适合阶段 |
|--------|------|--------|----------|
| 1 | BBQ equipment distributor | Google + LinkedIn | ⭐ 首选 |
| 2 | Outdoor living / garden retailer | Google "outdoor kitchen retailer" | |
| 3 | E-commerce seller (Amazon FBA) | Amazon seller 页面 / LinkedIn | 13"/16" 轻量 |
| 4 | Restaurant outdoor kitchen | 本地餐饮设备商 | 单量小 |
| 5 | OEM / private label | Alibaba buyer 帖 / LinkedIn | 有量后 |

### 怎么做

```text
Google:  "kamado grill distributor" + [country]
         "BBQ equipment wholesaler" + [country]
         "HPBA expo exhibitor list"（美国 BBQ 行业最大展会，买家名录公开）
LinkedIn（备选：直接搜易触发限制，优先用 Google 语法）:
         site:linkedin.com/in "purchasing manager" "BBQ" [country]
         site:linkedin.com/in "owner" "BBQ equipment" [country]
```

**验证标准**：网站有 grill/BBQ 品类 + 有 wholesale/import 字样 = 有效 lead 类型

**排除词**：搜索时加 `-used -secondhand -"for sale by owner"`，避免二手个人卖家污染结果

### 买家排序对 Lee 的具体论证（英文 B 档、零经验、2h/天）

| 类型 | 为何适合/不适合 Lee |
|------|---------------------|
| BBQ 分销商 ⭐ | 决策人少（往往老板本人）、邮件往来慢节奏（有时间用 AI 起草）、一单量大摊薄沟通成本 |
| 户外零售商 | 类似分销商，但更可能只买本地品牌，需筛选 |
| 电商卖家 | 流程标准化，但比价激烈、响应要快，2h/天 难跟上节奏 |
| 餐厅 | 单量 1-2 台，英语电话沟通多，B 档吃力 |
| OEM | 量大但要验厂、打样、合同复杂，零经验暂缓 |

### 写到哪里

- 排序结论 → `company/research.md` Top 3 买家类型
- 示例公司名 → 留给 Sales 写入 `workspace/buyers/pipeline.md`（Week 2 Day 3+）

---

## Step 3 — PAIN：他们怕什么

### 痛点清单（用竞品页/评论验证）

| 痛点 | 验证来源 | 我们回应（Offer） |
|------|----------|-------------------|
| 价格空间 | BGE 21" 零售价 vs 中国 FOB | FOB 透明 + 运费拆分 |
| 认证 | 目的国法规、Amazon 上架要求 | EN1860-1、FDA 扫描件 |
| 陶瓷易碎 | 差评里 "arrived cracked" | 包装方案、保险 |
| 运费占比 | 21" 82kg，LCL 报价 | 拆 FOB + freight |
| 保修/备件 | 论坛抱怨垫片、烤网 | 供应商条款写清 |
| MOQ | 分销商能否 1–2 台试单 | 问叔叔（有询盘后） |
| **关税** | 该国对中国产炉具的进口关税（美国注意 Section 301 附加税） | 报价区间前先算入到岸成本 |

### 小单物流可行性（「1–2 台试单」战略的前提，必查）

「先找买家再谈价」能否落地，取决于小单寄不寄得出去：

- [ ] 21" 单台（82kg、约 0.4cbm）LCL 最小计费吨位是否划算？（LCL 常有 1cbm 起收）
- [ ] 有没有接易碎陶瓷小单的拼箱货代（consolidator）？问 1–2 家货代拿参考价
- [ ] 若 21" 试单运费离谱 → 试单单位改推 **13"/16"**（22.7kg/40kg，可走快递或小拼箱）
- [ ] 结论写回 `company/research.md`

### 怎么做

- 读 Amazon 1–3 星评论（关键词 cracked, warranty, shipping）
- 读 BGE/KJ 官网 FAQ
- 记录该国进口商网站 FAQ

### 写到哪里

- 摘要 → `company/research.md` 或 `company/customers.md` 买家关心表
- 教训 → `company/lessons.md`

---

## Step 4 — 竞品

见 [`competitor-benchmark.md`](competitor-benchmark.md)

填完后更新 `country-scoring.md` 维度 E。

---

## Step 5 — 决策

1. 填完 `country-scoring.md` 所有分数
2. 算加权分，排出 Top 3
3. **强制选 1 国** — 写入 `company/customers.md`
4. 定义 **one niche**（国家 + 买家类型 + 尺寸）
5. 生成 20 关键词 → `keywords.md`

---

## Week 2 分日计划（2h/天）

| 天 | Research 任务 | Sales 任务（并行） |
|----|---------------|-------------------|
| Day 0 | **问叔叔出口史**（南非/南美/澳客户、认证、HS 编码） | — |
| Day 1 | 南非 + 澳：Step 1–2（工厂已验证地优先） | — |
| Day 2 | 美 + 智利/巴西；说 `正式Research` 可一天做完 | — |
| Day 3 | Step 3–5，填 scoring，**选定 1 国** | 找 10 买家 |
| Day 4–7 | 更新 keywords；微调 niche | 每天 10 买家，共 50 |

---

## 与 GPT 原方案对照

| GPT（商用烘焙炉） | 本项目（Kamado） |
|-------------------|------------------|
| bakery, restaurant, hotel | BBQ distributor, outdoor retail, e-commerce |
| commercial baking oven | kamado / ceramic charcoal grill |
| CE for electrical ovens | EN1860-1, FDA, fragile ceramic shipping |
| small bakery niche | mid-size BBQ equipment distributor niche |
