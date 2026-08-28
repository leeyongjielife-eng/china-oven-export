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
| **当前 phase** | **`W3_OUTREACH`**（详见 [`phases.md`](phases.md)） |
| 战略 | 一个资源 → 一个市场 → 一个报价 |
| 定位 | 寻源顾问，降风险，非最低价噱头 |
| Co-founder 贡献 | 国内烤炉供应商资源（父亲朋友工厂 YUEFU），可拿货销售、帮开市场 |

*Sources: `product.md`, `strategy.md`, `cofounder.md`*

---

## 当前阶段判断

- **Phase:** 0 — **`W3_OUTREACH`** + **A 软切 + 选项 2**（续至 **8/30**；回复 **4**&lt;5 → 不切 W4）
- **瓶颈:** 回复 **4**/5；热线索等对方（Alex 选尺寸、Brad/Angela 不催）
- **优势:** 买家 **221**；Contacted **191**；A Lead **20≥20**（闸门关）；`#132` HiBBQ 已 Yes
- **今日主线（2026-08-28 · 周五）：** 续同批冷 `#213–#221`（9）+ A 跟进 `#1 #2 #93–#96`（6）=15 对齐；P1 停扩；本机 **「今天发」**；**勿催 Brad / Martin / `#175` OOO**
- **暂不做:** B/C；催 #41；硬切 Reset；**8/30 前不正式 Research**；Bounce 不自动补；电话未授权

### Automation（2026-07-13 · 单 Run + Research）

| 名称 | 触发 | 模型 | 状态 |
|------|------|------|------|
| **Kamado 每日运营 — 澳洲** | 每天 09:00 · `main` | GPT-5.5 Medium | ✅ Active（禁止 Gmail 实发） |
| **Kamado 每周 Research — 澳洲** | 每周日 09:00 · `main` | GPT-5.5 Medium | ✅ Active |

**运行逻辑：** 读 [`phases.md`](phases.md) → 单 Run 内 Founder 派发 + Sales 扩买家/草稿 → **本机 Co-founder `今天发`** 实发；周日 Research 轻量复核。账本 SSOT=本机 `pipeline` Contacted。

**重要：** Automation 读 **GitHub 上的代码**。本地改完文档须 `git commit && git push`，次日 09:00 才能跑到最新状态。

| 📅 | — | **8/30** 再复评软切 | 锁定 |

### Co-founder 今日说明

软切续至 **8/30**。应发队列仍为冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（共 15）— 本机说 **「今天发」**。云端不实发。等 `#132` 选尺寸。

---

## 今日排期（2026-08-28 · 周五）✅ Sales 对齐 · ⏳ 待本机「今天发」

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 续同批冷邮 `#213–#221`（9）+ A 跟进 `#1 #2 #93 #94 #95 #96`（6） | ✅ Sales 对齐 · ⏳ 待本机 |
| **P1** | **Sales** | **停扩**（A Lead=20≥20） | ✅ |

---

## 上日排期（2026-08-27 · 周四）✅ Sales 对齐 · ⏳ 待本机「今天发」（未投递 → 今日续同批）

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 续同批冷邮 `#213–#221`（9）+ A 跟进 `#1 #2 #93 #94 #95 #96`（6） | ✅ Sales 对齐 · ⏳ 待本机 |
| **P1** | **Sales** | **停扩**（A Lead=20≥20） | ✅ |

---

## 上上日排期（2026-08-26 · 周三）✅ Sales 对齐 · ⏳ 待本机「今天发」（未投递 → 续同批）

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 续同批冷邮 `#213–#221`（9）+ A 跟进 `#1 #2 #93 #94 #95 #96`（6） | ✅ Sales 对齐 · ⏳ 待本机 |
| **P1** | **Sales** | **停扩**（A Lead=20≥20） | ✅ |

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
| P1 | 积满 **50 买家** | Sales | ✅ **139**；W3 外联池续扩 |
| P1 | 外联草稿备齐 | Sales | 进行中；Kit Lee / indicative FOB |
| P1 | 补联系人 A 级 | Sales | 持续补 |
| P1 | 外联 100（定价话术见 `product.md` 定价策略） | Co-founder 本机跟进/冷邮 + Sales 草稿 | W3 **A 软切+选项2**：A Lead 首封 · 停日扩（A Lead&lt;20 须补 A）· 回复 **4** · **8/30** 再复评 |
| P2 | 有回复后 → 向 YUEFU 要针对性 FOB | Supplier + Co-founder | 有 Qualified 后 |
| P3 | 正式报价单 | Quoting | 有需求 + 厂价后 |

---

## 待 Co-founder 决策 / 回答

> 发信规则已锁定：本机 `今天发` · 跟进优先 · Contacted≥100 停新冷邮。账本 SSOT=本机 pipeline。

| # | 问题 | 影响 | 状态 |
|---|------|------|------|
| 1 | 搭建 Gmail MCP / 发信账号连接 | 解锁 W3 外联 | ✅ 2026-07-15 |
| 2 | #41 Martin | 曾 Replied；暂不催 | ✅ 暂不催（2026-08-03） |
| 3 | **#17 / #126 Bounce** | 救 ICP | ⏳ #17 待定；**#126 无可用邮箱**（公开邮箱=死域名；仅电话 03 9889 6542 / 0418 551 520）· 2026-08-04 查毕 · 不改发 |
| 4 | Research Reset / 软切复评 | 是否换国或硬切 | ✅ **2026-08-19 续软切+选项2 至 8/30**（回复 4&lt;5，不切 W4 / 不硬切 / 不正式 Research） |
| 5 | 8/4 日配额 | A Lead `#139–#154` | ✅ 15/15 已发（2026-08-04） |

---

## 子代理调度日志

| 日期 | 调度 | 任务 | 结果写回 |
|------|------|------|----------|
| 2026-08-28 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-28 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-27 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-27 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-26 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-26 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-25 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-25 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-24 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-24 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-23 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted；**周日不发** | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-23 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；**周日不发**；周一「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-22 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-22 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-21 | **Sales 完成** | W3：续对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-21 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-20 | **Sales 完成** | W3：对齐应发冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-20 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#213–#221` + A 跟进 `#1 #2 #93–#96`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-19 | **Founder / Co-founder** | **8/16 软切复评落盘**：续 A 软切+选项 2 至 **8/30**；不切 W4；不硬切；不正式 Research；A Lead&lt;20 须补 A | `strategy.md` · `phases.md` · `customers.md` · `founder.md` · `cofounder.md` · `workflows/sales.md` |
| 2026-08-19 | **Sales / 本机** | 补A库存 `#213–#221`（9，全 A，均有公开邮箱）；A Lead 11→**20**；买家 **221**；闸门关；**未发信** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` |
| 2026-08-19 | **Co-founder 本机** | 回 `#132` 1-pager+关键页；补发冷 `#204–#212`；跟进 6；日配 15/15；A Lead→**11**；Contacted **191**；Replied **4** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-18 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#199–#203` + A 跟进 `#189–#193 #170–#174`；A Lead 16→**11**；Contacted **183** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-15 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#194–#198` + A 跟进 10；A Lead 21→**16**；Contacted **178** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-13 | **Sales 完成** | W3：续对齐应发冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-13 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-12 | **Sales 完成** | W3：续对齐应发冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-12 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续同批**冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-11 | **Sales 完成** | W3：对齐应发冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 停扩；未发信、未标 Contacted | `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-11 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 对齐冷 `#179–#183` + A 跟进 `#145–#154`（15）；P1 **停扩**（A Lead=20）；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-10 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#174–#178` + A 跟进 10（`#177` Bounce）；A Lead→**20** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-09 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#169–#173` + 跟进 `#124 #125 #127–#133 #44`（跳过 `#134`）；A Lead 24→**19** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-09 | **Sales 完成** | W3：续对齐应发冷 `#169–#173` + 跟进（15）；P1 停扩；本机随后实发 | `outreach-drafts.md` · `sales.md` · `today.md` |
| 2026-08-09 | **Founder → Sales** | W3：阶段保持 W3；**复评续软切至 8/16**；选项 2 → P0 **续发同批**；P1 **停扩**；Co-founder 本机「今天发」；禁止 Gmail | `today.md` · `strategy.md` · `phases.md` |
| 2026-08-08 | **Sales 完成** | W3：续对齐应发冷 `#169–#173` + 跟进 `#124 #125 #127–#134`（15）；补 A `#179–#183`；未发信、未标 Contacted | `pipeline.md` 183 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-08 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 **续发同批**冷 `#169–#173` + 跟进 `#124 #125 #127–#134`（15）；P1 库存闸门补 A `#179+`；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-07 | **Sales 完成** | W3：对齐应发冷 `#169–#173` + 跟进 `#124 #125 #127–#134`（15）；补 A `#174–#178`；未发信、未标 Contacted | `pipeline.md` 178 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-07 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 对齐冷 `#169–#173` + 跟进 `#124 #125 #127–#134`（15）；P1 库存闸门补 A `#174+`；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-06 | **Sales 完成** | W3：对齐应发冷 `#160–#168` + 跟进 `#124–#130`（15）；补 A `#169–#173`；未发信、未标 Contacted | `pipeline.md` 173 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-06 | **Founder → Sales** | W3：阶段保持 W3；选项 2 → P0 对齐 A Lead `#160–#168` + 跟进 `#124–#130`（跳#126）共 15；P1 库存闸门补 A `#169+`；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-04 | Co-founder 本机 | 「今天发」A Lead `#139–#154` 15/15（跳过 #142） | `pipeline.md` · `outreach-drafts.md` · `sales.md` |
| 2026-08-04 | **Founder 派发** | 8/4：A Lead 冷邮 `#139–#154`（15）；停扩；#126 查无邮箱；8/9 复评日历锁定 | `today.md` done · `founder.md` · `strategy.md` · `pipeline.md` |
| 2026-08-03 | Co-founder 本机 | 「今天发」A Lead 冷邮 #124–#138 15/15 | `pipeline.md` · `outreach-drafts.md` · `sales.md` |
| 2026-08-03 | **选项 2 落地** | 放宽 ≥100 停冷邮例外：仅 A Lead 可首封；停日扩；#41 暂不催；周一队列 #124–#138 | `strategy.md` · `cofounder.md` · `today.md` · `pipeline.md` |
| 2026-08-02 | **A 软切落地** | Co-founder 选 A：保持 W3；停日扩；跟进仅 buyer_class A；8/9 评估正式 Research | `strategy.md` · `founder.md` · `phases.md` · `workflows/sales.md` · `today.md` |
| 2026-08-02 | **buyer_class 落地** | 规则+闸门写入 customers/cofounder/strategy/workflows/phases；pipeline 全量打标；抽检纠偏后 A59/B45/C55 | `customers.md` · `pipeline.md` · `buyer-class-summary.md` · `sales.md` · `founder.md` |
| 2026-08-02 | **Founder复盘** | 周复盘：Contacted≥100 / 回复率 0.9% / 第 3 周日&lt;5% → 待拍板 Reset 路径；补 Research 周日志 + lessons | `founder.md` · `research.md` · `lessons.md` · `strategy.md` |
| 2026-08-02 | Co-founder 本机 | 「今天发」跟进 #34–#51 批 15/15 | `pipeline.md` · `outreach-drafts.md` |
| 2026-08-02 | Sales 完成 | W3：跟进草稿 #34–#51；+5 ICP #155–#159；未发信、未标 Contacted；Contacted≥100 停新冷邮 | `pipeline.md` 159 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-02 | Founder → Sales | W3：阶段保持 W3；Contacted **113**≥100 → P0 **跟进** #34–#51（停新冷邮）；P1 +5 买家 #155+；Co-founder 本机「今天发」；禁止 Gmail | `today.md` pending |
| 2026-08-01 | Sales 完成 | W3：对齐应发 #109–#123；+5 ICP #150–#154；未发信、未标 Contacted | `pipeline.md` 154 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-01 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#109–#123**（仍 Lead 同批续发）；P1 +5 买家 #150+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-31 | Sales 完成 | W3：对齐应发 #109–#123；+5 ICP #145–#149；未发信、未标 Contacted | `pipeline.md` 149 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-31 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#109–#123**（仍 Lead 同批续发）；P1 +5 买家 #145+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-30 | Sales 完成 | W3：对齐应发 #109–#123；+5 ICP #140–#144；未发信、未标 Contacted | `pipeline.md` 144 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-30 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#109–#123**（昨日本机已发 #93–#108）；P1 +5 买家 #140+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-29 | Sales 完成 | W3：对齐应发 #93–#98+#100–#108；+5 ICP #135–#139；未发信、未标 Contacted | `pipeline.md` 139 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-29 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#93–#98+#100–#108**（仍 Lead 同批续发）；P1 +5 买家 #135+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-28 | Sales 完成 | W3：对齐应发 #93–#98+#100–#108；+5 ICP #130–#134；未发信、未标 Contacted | `pipeline.md` 134 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-28 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#93–#98+#100–#108**（仍 Lead 同批续发）；P1 +5 买家 #130+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-27 | Sales 完成 | W3：对齐应发 #93–#98+#100–#108；补草稿 #109–#119；+5 ICP #125–#129；未发信、未标 Contacted | `pipeline.md` 129 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-27 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#93–#98+#100–#108**（昨日未投递）+ 补 #109–#119；P1 +5 买家 #125+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-26 | Research（本机补） | 周日轻量复核：Automation 仅跑 Day13 Founder/Sales、**无 Research 提交** → 本机补竞品价确认 + 关键词 #26–#30 + 周日志；回复率 1.2% = 第 2 个周日 &lt;5% → **暂不 Reset** | `research.md` · `competitor-benchmark.md` · `keywords.md` |
| 2026-07-26 | Sales 完成 | W3：对齐应发 #93–#98+#100–#108；+5 ICP #120–#124；未发信、未标 Contacted | `pipeline.md` 124 · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-07-26 | Founder → Sales | W3：阶段保持 W3；P0 对齐应发 **#93–#98+#100–#108**；P1 +5 买家 #120+；Co-founder 本机「今天发」15；禁止 Gmail | `today.md` pending |
| 2026-07-26 | Founder merge | **push 前合入 origin/main**：本机 Contacted SSOT 保留；云端 Day8–12 独有买家改号为 **#100–#119**；本机 ICP 保持 **#93–#99** | merge → push |
| 2026-07-24 | Founder → Sales + 本机 | 补派今日；本机**直接发**跟进 #19–#33；Sales 续扩 #100+ | 本机跟进 ✅ 15/15 · Sales `today.md` 仍 pending |
| 2026-07-23 | Founder → Sales | **补派今日**：阶段保持 W3；P0 换画像扩 #93+；本机跟进队列 #19–#33；禁止 Gmail | Sales ✅ #93–#99 · 本机跟进 ❌ → 今日补 |
| 2026-07-22 | Founder → Sales + 本机 | **战略转向**：配额全跟进（Martin+#1/#2/#4/#5/#7–#12/#14/#16–#18）；Sales #93+ 仅 importer/distributor/multi-store/own-brand | `strategy.md` · 本机 ✅ · Sales ❌ 未执行 |
| 2026-07-22 | Founder → Sales | W3：阶段保持 W3；**可发池空** → 派发 P0 扩有邮箱买家 #93+（≥5，目标 10–15）+ 草稿；明日应发列表；禁止 Gmail / 禁止覆盖 Contacted | `today.md` **已重派**（画像收紧） |
| 2026-07-21 | Co-founder 本机 | `今天发` → #80–#92 共 13 封（池尽）；Contacted 85/100 | `pipeline.md` · `sales.md` |
| 2026-07-20 | Founder → Sales | W3 Day 7：阶段保持 W3；派发对齐未发草稿 + 应发 #35–#51（跳过 #46/#48）、+5 买家；Co-founder 本机「今天发」 | `today.md` pending |
| 2026-07-20 | Sales 完成 | W3 Day 7：对齐 15 封草稿（#35–#51）；新增买家 #81–#85；未发信、未标 Contacted | `pipeline.md` 85/100 · `outreach-drafts.md` 84/85 · `sales.md` · `today.md` done |
| 2026-07-19 | Founder → Sales | W3 Day 6：阶段保持 W3；派发对齐未发草稿 + 应发 #20–#34、+5 买家；Co-founder 本机「今天发」 | `today.md` pending |
| 2026-07-19 | Sales 完成 | W3 Day 6：对齐 15 封草稿（#20–#34）；新增买家 #76–#80；未发信、未标 Contacted | `pipeline.md` 80/100 · `outreach-drafts.md` 79/80 · `sales.md` · `today.md` done |
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
| 2026-07-18 | Sales 完成 | W3 Day 5：对齐 15 封草稿；新增买家 #71–#75；未发信、未标 Contacted | `pipeline.md` 75/100 · `outreach-drafts.md` 74/75 · `sales.md` · `today.md` done |

---

## 每周复盘（Founder Agent 主持）

### Week 1

- **漏斗:** 买家 0 / 外联 0 / 回复 0
- **本周结论:** 启动架构与 Co-founder 档案
- **下周优先级:** Research 定澳；积买家
- **写入 lessons:** 2026-07-10 多条

### Week 3 收官 / Week 4 交界（2026-08-02 · Founder复盘）

- **漏斗:** 买家 **188** · 已联系 **164/100** · Contacted **162** · Replied **2** |
- **本周结论:**
  1. **Contacted≥100 已达成** → 停新冷邮正确；W4 未开（回复 &lt;5）
  2. **连续 3 个周日回复率 &lt;5%** → 触及 `W3_RESEARCH_RESET` 决策门槛（见 `phases.md` / `research.md`）
  3. 渠道质量：BG/Weber 区域店占比高；ICP `#93–#98` 已发仍 0 回复；唯一信号来自 kamado 专营 `#41`
  4. 运营债：同批冷邮可欠发多日；云端仍扩池 → 已记 lessons
  5. 今日动作：跟进 `#34–#51` 15 封已发；Research 周日志已补
- **决策（已拍板）：** ✅ **A 软切** + ✅ **选项 2**（2026-08-03）— 不找新名；对 **A Lead** 开冷邮；#41 暂不催；**8/9** 再评估
- **备选未选：** 选项 1（只跟进已 Contacted A）· 选项 3（恢复扩名）· B 硬切 · C 再跟一周
- **下周优先级：** 日配额打 A Lead 首封（#124+）；不扩 Lead 名；不问叔叔
- **写入 lessons:** `lessons.md`；`strategy.md` 选项 2 |

---

## 与其他文件的分工

| 文件 | 谁维护 | 内容 |
|------|--------|------|
| `founder.md`（本文件） | **Founder Agent** | 合成视图、排期、待决策、调度 |
| `cofounder.md` | **人类合伙人** + Agent 代录 | 真人身份、资源、能/不能做 |
| `strategy.md` | Founder Agent | 阶段、定位、关键决策 |
| `lessons.md` | 全员 → Founder 合成 | 实战教训 |
