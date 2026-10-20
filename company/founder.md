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
| **当前 phase** | **`W4_FOLLOWUP`**（2026-10-09 起；英新冷邮并行；详见 [`phases.md`](phases.md)） |
| 战略 | 一个资源 → 一个市场 → 一个报价 |
| 定位 | 寻源顾问，降风险，非最低价噱头 |
| Co-founder 贡献 | 国内烤炉供应商资源（父亲朋友工厂 YUEFU），可拿货销售、帮开市场 |

*Sources: `product.md`, `strategy.md`, `cofounder.md`*

---

## 当前阶段判断

- **Phase:** 0 — **`W4_FOLLOWUP`**（2026-10-09 起 · 英新冷邮并行；英国 A **243**；英 A Contacted **133** · 英 Replied **5**）
- **瓶颈（2026-10-20 复盘）:** **Replied → Qualified**。英 Replied 5 中真需求仅 `#369` `#285`、软兴趣 `#357`；`#298` `#342` 非采购信号。10/09 回访 5 封后至今账本无回信记录（10/10–10/20 未落盘，待核收件箱）。英新冷邮 10/09 恢复（门槛英 Contacted≥300，现 **133**）
- **优势:** EN1860-1；首封 **hero + one-pager**；英线 Replied 5 · 英 Contacted 过百
- **今日主线（2026-10-09）：** **补A** `#507–#521`（15 · 全英 A · **未发信**）· 英 A 228→**243** · 英 A Lead **111** · 全库 **521** · 未发 `#415–#521` · 今日未发邮件 · **停冷邮规则改**：恢复英新冷邮，门槛 100→**300**
- **暂不做:** 云端 Gmail 实发；澳新冷邮；催 Brad/Martin；电话；问叔叔；Bounce 不自动改发；**不回** `#280` `#306` `#335`；找客方法暂不入 SSOT

### Automation（2026-07-13 · 单 Run + Research）

| 名称 | 触发 | 模型 | 状态 |
|------|------|------|------|
| **Kamado 每日运营 — 澳洲** | 每天 09:00 · `main` | GPT-5.5 Medium | ⚠️ 名称未改；**必须读 `phases.md`**：现为英国 `W3_OUTREACH`，P0=按 **Wave-1 发信序**（`buyer-class-summary`），**云端不实发** |
| **Kamado 每周 Research — 澳洲** | 每周日 09:00 · `main` | GPT-5.5 Medium | ✅ Active（轻量复核改盯**英**零售/关键词；≠ 正式Research） |

**运行逻辑：** 读 [`phases.md`](phases.md) → 单 Run 内 Founder 派发 + Sales 扩买家/草稿 → **本机 Co-founder `今天发`** 实发；周日 Research 轻量复核。账本 SSOT=本机 `pipeline` Contacted。

**重要：** Automation 读 **GitHub 上的代码**。本地改完文档须 `git commit && git push`，次日 09:00 才能跑到最新状态。

| 📅 | — | **换英已确认** → `W2_COLLECT` 积 50 英 A | ✅ |
| 📅 | 2026-09-10 | **英 A 50/50** → 切 **`W3_OUTREACH`** | ✅ |
| 📅 | 2026-09-15 | P3 冷 9+首跟 6 · 英 Contacted 50 | ✅ |
| 📅 | 2026-09-28 | 「发邮件」首跟 15/15 `#317` `#321` `#322` `#324–#326` `#328` `#333` `#334` `#336–#338` `#346–#348` · 漏斗不变 · **停英新冷邮** | ✅ |
| 📅 | 2026-09-22 | 「发邮件」15/15 `#386–#400` · 英 Contacted **112** · **停英新冷邮** | ✅ |
| 📅 | 2026-09-22 | 回信户 v2 跟进：实发 3（`#285` `#169` `#342`）· `#369` 暂缓 · 澳禁催维持（`#132` `#147` `#41` 未发） | ✅ |
| 📅 | 2026-09-22 | `#369` Atom 补发 18"+21" EN1860-1（精简 · 无报价）msg `1a0c9261602e10d1` | ✅ |
| 📅 | 2026-09-21 | 「今天发」15/15 `#371–#385` · 英 Contacted **97** · 英 A Lead **4**（Bounce） | ✅ |
| 📅 | 2026-09-20 | 「补A并发冷邮」15/15 `#356–#370` · 英 Contacted **82**（Bounce 后）· 英 A **92** · `#369` Replied | ✅ |
| 📅 | 2026-09-19 | 「今日发」15/15 冷7+跟进8 · 英 Contacted **71** · 英 A Lead **2** | ✅ |
| 📅 | 2026-09-18 | 「发信」15/15 P4+/P4 · 英 Contacted **66** · 英 A Lead **8** | ✅ |
| 📅 | 2026-09-16 | 收件箱 `#285` Replied · `#280` Lost · 英 Contacted **48** · 英 Replied **1** | ✅ |

### Co-founder 今日说明

**9/22：** 「发邮件」**15/15** `#386–#400`（hero+onepager）。英 Contacted **112** · 英 A Lead **20**（16 可发 + 4 Bounce）· **英 Contacted≥100 → 停英新冷邮**。次日改跟进 / 热线索；`#369` 回信仍待授权。

**9/21：** 「今天发」**15/15** `#371–#385`（hero+onepager）。英 Contacted **97** · 英 A Lead **4**（仅 Bounce）· 英 Replied **3**。

**9/20：** 「补A并发冷邮」**15/15** `#356–#370`。`#369` Atom→Replied。`#364` `#370` Bounce。
---

## 今日排期（2026-08-13 · 周四）⏳ 续冷 #179–#183 + A 跟进 #145–#154 · 停扩

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 对齐后「今天发」冷邮 `#179–#183`（5）+ A 跟进 `#145–#154`（10） | ✅ Sales 对齐 · ⏳ 待本机 |
| **P1** | **Sales** | **停扩**（A Lead=20≥20） | ✅ |

---

## 上日排期（2026-08-12 · 周三）✅ Sales 对齐 · ⏳ 本机未投递 → 今日续同批

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 对齐后「今天发」冷邮 `#179–#183`（5）+ A 跟进 `#145–#154`（10） | ✅ Sales 对齐 · ⏳ 本机未发 |
| **P1** | **Sales** | **停扩**（A Lead=20≥20） | ✅ |

---

## 上上日排期（2026-08-11 · 周二）✅ Sales 对齐 · ⏳ 本机未投递

| 优先级 | 谁 | 任务 | 状态 |
|:---:|------|------|:---:|
| **P0** | **Sales → 本机** | 对齐后「今天发」冷邮 `#179–#183`（5）+ A 跟进 `#145–#154`（10） | ✅ Sales · ⏳ 本机未发 |
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
| P0 | **问叔叔：YUEFU 出口史 / FOB** | Co-founder | ✅ **2026-09-21 已拿到** 厂报价表（FOB 盐田 18" US$150 / 21" US$186）+ 样品价 + 出口史（无英国客户）· 见 `supplier-inquiry.md` · 仍缺柜下试单量价、付款方式 |
| P0 | 市场研究，定第一个目标国 | Research | ✅ **英国**（2026-09-09 确认；取代 7/10 澳） |
| P1 | 积满 **50 英国 A** | Sales | ✅ **50**（2026-09-10）；现 **52**（+`#329–#330` Wave-1） |
| P1 | 外联草稿备齐 | Sales | ✅ 英 `#279–#328` 首封草稿齐 · **未发** |
| P1 | 补联系人 A 级 | Sales | 持续补 |
| P1 | 外联 100（定价话术见 `product.md` 定价策略） | Co-founder 本机 + Sales 草稿 | 🔄 **`W3_OUTREACH`** · 等本机「今天发」（建议自 `#279`） |
| P2 | 有回复后 → 向 YUEFU 要针对性 FOB | Supplier + Co-founder | ✅ 厂 FOB 已有（9/21）；有 Qualified 后再问柜下试单量价、付款方式 |
| P3 | 正式报价单 | Quoting | 有需求 + 厂价后 |

---

## 待 Co-founder 决策 / 回答

> 发信规则：本机 `今天发`；**英国 Contacted≥300** 停英新冷邮（2026-10-09 由 100 改为 300；澳 256 归档）。账本 SSOT=本机 pipeline。

| # | 问题 | 影响 | 状态 |
|---|------|------|------|
| 1 | 搭建 Gmail MCP / 发信账号连接 | 解锁 W3 外联 | ✅ 2026-07-15 |
| 2 | #41 Martin | 曾 Replied；暂不催 | ✅ 暂不催（2026-08-03） |
| 3 | **#17 / #126 Bounce** | 救 ICP | ⏳ #17 待定；**#126 无可用邮箱**（公开邮箱=死域名；仅电话 03 9889 6542 / 0418 551 520）· 2026-08-04 查毕 · 不改发 |
| 4 | Research Reset / 是否换英 | 第一市场 | ✅ **2026-09-09 确认换英**；2026-09-10 英 A **50/50** → **`W3_OUTREACH`** |
| 5 | 8/4 日配额 | A Lead `#139–#154` | ✅ 15/15 已发（2026-08-04） |
| 6 | **企业域名邮箱**（2026-10-20 评估） | 送达率 / 可信度 | ⏳ 待拍板。`yuefubbq.com` MX = **阿里云企业邮**，SPF 已配、**无 DMARC**。① **推荐** 请厂开 `kit@yuefubbq.com`，在 Gmail「以其他地址发送」挂阿里云 SMTP —— 与厂站/目录/TÜV 主体一致，现有 Gmail MCP 流程基本不变；需厂配合（顺带建议厂加 DMARC `p=none`）。② 自购域名 + Google Workspace（约 US$7/人·月）—— 自主可控，但新域名需 2–4 周预热，且与厂站不同名。③ 维持 `leewingqi16@gmail.com`。**任一切换都不再发「换邮箱通知」**；改 `cofounder.md` 发信政策须 Co-founder 拍板 |

---

## 子代理调度日志

| 日期 | 调度 | 任务 | 结果写回 |
|------|------|------|----------|
| 2026-10-20 | **Founder复盘** | 英线 9/09–10/20 复盘（见下「每周复盘」）；Co-founder 拍板：维持 Qualified 后才问厂试单价；起草 `#369` `#285` `#357` 最后一触（**未发**）；评估域名邮箱（待决策 #6）；`_send_payload/` 进 `.gitignore`；本机 9/14 起积压改动一次 commit + push | `lessons.md` · `founder.md` · `outreach-drafts.md` · `.gitignore` |
| 2026-10-04 | **Co-founder 拍板** | 新邮 From / 署名改回 `leewingqi16@gmail.com`；`user-gmail` 实发；`plugin-gmail`（claire）不再发新信。历史已发不回改。one-pager PDF 页脚仍印 claire | `cofounder.md` · `templates/outreach.md` |
| 2026-10-09 | **Co-founder 本机** | 英新冷邮 **10/10** `#415–#424` From `leewingqi16@gmail.com` · hero + one-pager · 英 A Contacted 123→**133** · 英 A Lead **101** · 今日 15/15 用满 · `#420` 审批拦 + 网络中断，核实未发后重发 | `pipeline.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-09 | **Co-founder 本机** | 「跟进吧」热线索回访 **5/5** `#369` `#285` `#298` `#357` `#342` From `leewingqi16@gmail.com` · 附 hero + 4 张实拍 · Stage 保持 Replied · `#298` 首发网络中断、确认未发后重发 | `pipeline.md` · `outreach-drafts.md` · `sales.md` |
| 2026-10-09 | **Co-founder 拍板** | **切 `W4_FOLLOWUP`**（英 Replied 5 达标）：英新冷邮为主并行至英 Contacted≥300 + 热线索带新理由回访（须授权）；**更正**：厂 FOB/出口史 9/21 已拿到（原「问叔叔暂缓」过时）；起草 5 家热线索回访草稿（未发） | `phases.md` · `cofounder.md` · `product.md` · `sales.md` · `buyer-class-summary.md` · `outreach-drafts.md` |
| 2026-10-09 | **Co-founder 拍板** | **恢复英新冷邮**：停止门槛英 Contacted ≥100 → **≥300**（现 123，余 177）；日配额仍 15，周日不发冷邮；可发冷池 `#415–#521`（107 可发） | `cofounder.md` · `phases.md` · `strategy.md` · `customers.md` · `outreach-playbook.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-09 | **Co-founder 本机** | **数字更正**：英 A Contacted 124→**123**（`#400` 改 Bounce · 10/07 首跟实际送达 14/15）；英 Replied 3→**5**（补 `#298` `#357`）；全库 Contacted **379** · Replied **9**；历史行不回改 | `sales.md` · `buyer-class-summary.md` · `founder.md` |
| 2026-10-09 | **Co-founder 本机** | **补A** `#507–#521`（15 · 全英 A · **未发信**）；英 A 228→**243**；全库 **521**；停英新冷邮维持 | `pipeline.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-08 | **Co-founder 本机** | 英 A 第 3 触 **6** `#279` `#283` `#284` `#286` `#287` `#288` From `leewingqi16@gmail.com` · 新理由 2027 季采购+先拿样 · 同附 `email-hero-kamado.jpg` · Co-founder 授权；破停冷邮 `#415` 被审批拦下未发 | `pipeline.md` · `sales.md` |
| 2026-10-08 | **Co-founder 本机** | 英 A 首跟 **3** `#412` `#413` `#414` From `leewingqi16@gmail.com` · 新写法 · 同附 `email-hero-kamado.jpg` 原图 · Stage 保持 Contacted · 首跟队列清空 | `pipeline.md` · `sales.md` |
| 2026-10-08 | **Co-founder 本机** | **补A** `#492–#506`（15 · 全英 A · **未发信**）；英 A 213→**228**；全库 **506**；停英新冷邮维持；英 A Contacted 仍 **124** | `pipeline.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-07 | **Co-founder 本机** | 英 A 首跟 **15/15** `#392–#400` `#402` `#403` `#407` `#408` `#410` `#411` From `leewingqi16@gmail.com` · 新写法 · 同附 `email-hero-kamado.jpg` 原图 · 跳过 `#401`（禁补附件包）与 `#404` `#405` `#406` `#409`（9/26 冷邮重复两封）· Stage 保持 Contacted | `pipeline.md` · `sales.md` |
| 2026-10-07 | **Co-founder 本机** | **补A** `#477–#491`（15 · 全英 A · **未发信**）；英 A 198→**213**；全库 **491**；停英新冷邮维持；英 A Contacted 仍 **124** | `pipeline.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-06 | **Co-founder 本机** | 英 A 首跟 **15/15** `#377–#391` From `leewingqi16@gmail.com` · 新写法（短正文+一句对方业务方向+一个 YES）· 同附 `email-hero-kamado.jpg` 原图 · Stage 保持 Contacted | `pipeline.md` · `sales.md` · `cofounder.md` |
| 2026-10-06 | **Co-founder 本机** | **补A** `#462–#476`（15 · 全英 A · **未发信**）；英 A 183→**198**；全库 **476**；停英新冷邮维持；英 A Contacted 仍 **124** | `pipeline.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-10-05 | **Co-founder 本机** | 英 A 首跟 **15/15** From `leewingqi16@gmail.com`（`#359–#363` `#365–#368` `#371–#376`）· 同附闭盖图（240×180 压缩版）· Stage 保持 Contacted | `pipeline.md` · `sales.md` |
| 2026-10-04 | **Co-founder 本机** | **补A** `#447–#461`（15 · 全英 A · **未发信**）；英 A 168→**183**；全库 **461**；周日不发；停英新冷邮维持；英 A Contacted 仍 **124** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` |
| 2026-09-25 | **Co-founder 本机** | **补A** `#417–#431`（15 · 全英 A · **未发信**）；英 A 138→**153**；英 A Lead 20→**35**；全库 **431**；停英新冷邮维持 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-24 | **Co-founder 本机** | **中秋祝福 117/117**（英A+澳询盘；前34旧邮不管；后83 claire 已校验）；Stage 不变 | `pipeline.md` · `today.md` · `cofounder.md` |
| 2026-09-24 | **Co-founder 拍板** | 旧邮又能用 → **选项 1**（**2026-10-04 已取代**）：当时发信仍 `claireleebalance`；`leewingqi16` 只收不发 | `cofounder.md` |
| 2026-09-23 | **Co-founder 本机** | **澳实拍+报价** `#147` `#132` `#169` **3/3**（破禁催 · +JPG · 跳过 `#41`）；Stage 保持 Replied | `pipeline.md` · `outreach-drafts.md` · `today.md` · `sales.md` |
| 2026-09-23 | **Co-founder 本机** | 痛点跟进 **15/15**（选项1 · `#293 #294 #295 #299 #288 #291 #301 #307 #314 #323 #287 #302 #308 #312 #313`）；不发新补A；停英新冷邮维持 | `pipeline.md` · `outreach-drafts.md` · `today.md` done |
| 2026-09-23 | **Co-founder 本机** | 「发邮」英 Contacted 跟进 **15/15**（`#290 #296–#298 #300 #303–#305 #279 #281 #283 #284 #286 #289 #292`）；From `claireleebalance`；漏斗 Contacted 不变；停英新冷邮维持 | `pipeline.md` · `outreach-drafts.md` · `today.md` done |
| 2026-09-23 | **Co-founder 本机** | **补A** `#401–#416`（16 · 全英 A · **未发信**）；英 A 122→**138**；英 A Lead 4→**20**；全库 **416**；停英新冷邮维持 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-22 | **Co-founder 本机** | 「发邮件」**15/15** `#386–#400`；英 Contacted 97→**112**；英 A Lead 19→**4**（Bounce）；全库 Contacted **368**；**英 Contacted≥100 → 停英新冷邮** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-22 | **Co-founder 本机** | **回信户 v2 跟进**（非日配额）：实发 3 封 `#285` `1a0c909d565731c1` · `#169` `1a0c90a9267ebe18`（**显式授权破「#169 不催」**）· `#342` `1a0c90b229030f8f`；Stage 全保持 Replied、**漏斗数不变**；`#369` 暂缓；澳 `#132` `#147` `#41` 未发。改法=**反转谁先动**（依 `lessons.md` 4 条热线索全死在「请你先选」）+ **LCL 最低计费 1 CBM → 默认 2 台**。同日读 TÜV 报告发现 **工厂实为肇庆福宝、悦富为佛山销售名（同一老板）**，`our own plant in Foshan` 口径作废 | `pipeline.md` · `outreach-drafts.md` · `today.md` · `lessons.md` · `templates/outreach.md` · `product.md` · `product-summary.md` · `supplier-inquiry.md` done |
| 2026-09-21 | **Co-founder 本机** | 「今天发」**15/15** `#371–#385`；英 Contacted 82→**97**；英 A Lead 19→**4**（Bounce）；全库 Contacted **353**；可发冷池空 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-20 | **Co-founder 本机** | 「补A并发冷邮」**15/15** `#356–#370`；英 Contacted 70→**85**；英 A 77→**92**；全库 **370** / Contacted **341**；冷池空 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-19 | **Co-founder 本机** | 「今日发」**15/15**：冷 7 + 跟进 8；英 Contacted 66→**71**；英 A Lead 7→**2**（`#282` `#341` Bounce）；`#342` Replied；全库 Contacted **327**；冷池空 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-15 | **Co-founder 本机** | 「今日发」**15/15**：P3 冷 9 + 首跟 6；英 Contacted 41→**50**；英 A Lead 10→**1**（仅 `#282`）；全库 Contacted **306** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-14 | **Co-founder 本机** | 「今天发」**15/15** Wave-1 P2：冷 10（hero+one-pager）+ 跟进 5；英 Contacted 31→**41**；英 A Lead 20→**10**；全库 Contacted **297**；护栏改为首封 2 附件 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `cofounder.md` · `today.md` done |
| 2026-09-12 | **Co-founder 本机** | 「按方案发」**15/15** Wave-1：冷 `#329 #330 #315`（+hero）+ 跟进 12；英 Contacted 28→**31**；英 A Lead 23→**20**；全库 Contacted **287** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-12 | **Sales Wave-1** | 入账 `#329` Kama Gear · `#330` HEX · 重排英发信序 · 英 A **52** · 全库 **330** | `pipeline.md` · `outreach-drafts.md` · `buyer-class-summary.md` · `sales.md` · `uk-buyer-pool-wave1-*.md` |
| 2026-09-11 | **Co-founder 本机** | 「今天发」**15/15** 英冷 `#294–#308`（+已锁定 hero.jpg）；英 Contacted 14→**29**；英 A Lead 36→**21**；全库 Contacted **285** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-10 | **Co-founder 本机** | 「今天发」**15/15** 英冷 `#279–#293`（+hero.jpg）；英 Contacted 0→**15**；英 A Lead 50→**35**；全库 Contacted **271** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-10 | **开启 Sales Day5** | 英 A `#319–#328`（10）· 英国 A **50/50** · 切 **`W3_OUTREACH`** · 未发信 · 全库 **328** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `phases.md` · `today.md` done |
| 2026-09-10 | **开启 Sales Day4** | 英 A `#309–#318`（10）· 英国 A **40/50** · 禁发 · 全库 **318** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `buyer-class-summary.md` · `today.md` done |
| 2026-09-10 | **Founder / Co-founder** | **澳 WA 试点选项 A**：仅澳 A + 公开号；禁催 Brad/Martin/Angela/Alex；不扩澳、不重启澳冷邮 | `cofounder.md` · `customers.md` · `outreach-playbook.md` · `founder.md` |
| 2026-09-09 | **Founder / Co-founder** | **确认换英**：第一市场英国生效；切 `W2_COLLECT`；积 50 英 A；澳停新冷邮 | `customers.md` · `phases.md` · `strategy.md` · `founder.md` · `cofounder.md` · `sales.md` · `today.md` · `lessons.md` |
| 2026-09-09 | **Research 正式Research** | 短名单重评：英 **3.85** > 澳 **3.75**；推荐换英 → **已确认** | `country-scoring.md` · `research.md` · `customers.md` · `lessons.md` |
| 2026-09-09 | **Founder / Co-founder** | **选 C 落盘**：切入 `W3_RESEARCH_RESET`；授权 **正式Research**；暂停日配新冷邮与补 A | `strategy.md` · `phases.md` · `customers.md` · `founder.md` · `cofounder.md` · `workflows/sales.md` · `today.md` · `lessons.md` |
| 2026-09-09 | **Founder复盘** | 提前于 9/16：Contacted 256 / Replied 4；出三选一；**Co-founder 选 C** | `lessons.md` · `founder.md` |
| 2026-09-09 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#278`（1）+ 跟进 `#191–#193 #199–#203 #176 #178 #180 #181 #204 #205`（14）；A Lead 13→**12**；Contacted **256**；可发冷邮已空 | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-07 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#271–#277`（7）+ 跟进 `#198 #170–#174 #189 #190`（8）；`#278` 留次日；A Lead 20→**13**；Contacted **255** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-04 | **Founder / Co-founder** | **补做 8/30 软切复评落盘**：续 A 软切+选项 2 至 **9/16**；不切 W4；不硬切；不正式 Research；日配跟进≥新冷邮；Brad 静默至约 9/16 | `strategy.md` · `phases.md` · `customers.md` · `founder.md` · `cofounder.md` · `workflows/sales.md` · `lessons.md` · `buyer-class-summary.md` |
| 2026-09-04 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#263–#270`（8）+ 跟进 `#156 #157 #159 #194–#197`（7）；A Lead 20→**12**；Contacted **248** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-03 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#255–#262`（8）+ 跟进 `#154 #4 #10 #20 #64 #92 #155`（7）；A Lead 20→**12**；Contacted **240** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-09-02 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#247–#254`（8）+ 跟进 `#146 #148–#153`（7）；A Lead 20→**12**；Contacted **232** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
| 2026-08-26 | **Co-founder 本机** | 「今天发」**15/15**：冷 `#239–#246`（8）+ 跟进 `#182–#185 #187 #144 #145`（7）；补A `#247–#254`（8 · 待发）；A Lead→**20**；Contacted **224** | `pipeline.md` · `outreach-drafts.md` · `sales.md` · `today.md` done |
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

### 2026-10-20 · Founder复盘（英线 9/09–10/20 · W4 第 2 周）

- **漏斗:** 英首封投递约 **141** · 真人回复 **8**（有兴趣 5 + 拒 3 · 约 5.7%；澳 1.6%）· Qualified **0** · 报价单 **0** · 英 A Lead 库存 **101**
- **热线索:** `#369` Atom（最深询盘 · 9/20 后未再回）· `#285` Vision（要 1–2 台 21" 样品 · 9/16 FOB 报价后沉默）· `#357` Stone Bake（软兴趣）· `#298` Urban（仅说进垃圾箱）· `#342` Inferno（佣金代卖）
- **本周结论:**
  1. 换英正确 —— 获客端达合格线；卡点在 Replied → Qualified
  2. 主因是报价结构（FOB + 1×40HQ + 自找货代）与英国小厂体量不匹配，非文案
  3. 热线索过度触达、发信身份频繁切换、Git 5 周未提交、10/10 起账本断档
- **决策（已拍板 2026-10-20）:** 维持「Qualified 后才问厂试单量价」；热线索最后一触（春节前排产截止 · 不报新价 · 待授权发）后停追；域名邮箱待拍板（待决策 #6）；复盘落盘 + push
- **下两周唯一指标:** Qualified 数
- **写入 lessons:** `lessons.md` 2026-10-20

### 2026-09-09 · Founder复盘（提前于 9/16）

- **漏斗:** 买家 **278** · Contacted **256** · Replied **4** · A Lead **12&lt;20** · 回复率约 **1.6%**
- **热线索:** `#132` Alex（Yes · 未选尺寸）· `#169` Brad（样品方案后静音 · 9/2 轻跟无回）· `#147` Angela · `#41` Martin 凉
- **本周结论:**
  1. **不切 W4**（回复仍 &lt;5）
  2. **发信量已足够**；瓶颈是转化与渠道单一（Gmail 为主，LI 未跑）
  3. **A 软切有信号但未闭环** — 4 条真回后无 Qualified
  4. **可提前复盘** — 不必等到 9/16
- **待 Co-founder 拍板（三选一）:** ✅ **已选 C — `正式Research`**（2026-09-09）
  - ~~A — 续软切强化（至 9/23）~~
  - ~~B — 硬切 `W3_RESEARCH_RESET` 仅暂停~~
  - **C — `正式Research`** ← 已拍板；同步切入 `W3_RESEARCH_RESET`；短名单 ≥3 国重评澳
- **Founder 原推荐：** A（未采纳）
- **写入 lessons:** `lessons.md` 2026-09-09 |

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
