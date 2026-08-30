# Co-founder（人类合伙人）

> **这是你（人）的档案。** Founder Agent 读此文件了解你能做什么、不能做什么。
> 你不需要每周维护；只在有新区块或 Founder 提问时更新。

---

## 我是谁

- **角色：** Co-founder（人类合伙人）— **Lee Wing Kit**
- **所在地：** 中国
- **语言：** 中文母语；英文能读，外联邮件由 **AI 起草**（发信政策见下方[分工原则](#分工原则与-founder-agent-的边界)，2026-07-10 确认，档 B）

## 我贡献什么

- ✅ **核心资源：** 国内烤炉供应商渠道，可对接出口
- ✅ **当前已知供应商：** YUEFU BBQ（佛山），已提供 2025 Kamado 目录
- ✅ **与 YUEFU 关系：** 父亲朋友开的厂；对方允许我拿货去卖
- ✅ **定价策略：** 见 [`product.md`](product.md) 定价策略（先找买家、再谈厂价）

## 我愿意 / 能做什么

| 动作 | 能否 |
|------|------|
| 向供应商发微信 / 打电话询价 | **能**（父亲朋友关系，沟通门槛低） |
| 发海外 cold email | AI 起草并可自动发送；我也可自己发（发信政策见分工原则） |
| 处理付款、报关、物流实操 | <!-- 待确认 --> |
| 每天投入时间 | **约 2 小时/天**（2026-07-10 确认） |

## 我的背景（待补充）

- 外贸经验：**无，第一次做出口**（2026-07-10 确认，档 A）
- 行业人脉：<!-- -->
- 其他工作是否占用大部分时间：<!-- -->

## 对外身份

- 联系买家用的名字 / 品牌：**Kit Lee**（对外署名，2026-07-15 更新；护照拼音 Lee Wing Kit）
- 是否注册公司：<!-- 待填 -->

---

## 分工原则（与 Founder Agent 的边界）

```text
Founder Agent（AI）     →  研究、策略、排期、派发 Sales 任务、写邮件草稿、维护 company/
Co-founder（你）        →  供应商人脉、拍板、微信/电话、付款、验货、Automation 开关
Sales / 其他子代理（AI） →  见 workflows/ 各角色边界；**不**替你做真人动作
```

### Co-founder 角色边界（人类）

| 职责内（只有你能做） | 不负责（交给 AI 子代理） |
|---------------------|-------------------------|
| 微信/电话问 YUEFU、询价、索证 | 写 pipeline / 外联草稿 |
| 付款、报关、验货、签约 | 选市场研究、排期 |
| 战略拍板、回答 Founder 待决策 | 维护 `founder.md` 排期 |
| 启用/关闭 Cursor Automation | 代替 Sales 找买家（除非手动 `启动 Sales`） |
| 可选：外联发信前复核 | 写正式 FOB 报价（Quoting） |

**写回：** 真人动作 → 本文件「真人动作记录」；**不写** `workspace/dispatch/today.md`（那是 Founder↔Sales 交接）。

### 发信政策（全公司唯一来源）

> 本节是外联邮件发送政策的**唯一归属**。其他文档（`workflows/sales.md`、`workflows/founder.md`、`workflows/models.md` 等）需要时**只指向此处**，不得另行规定。

- **AI 可起草并自动发送外联邮件**（**不禁止自动发信**）。
- Co-founder **可选**在发送前复核；W3 **默认不复核**。
- **执行拓扑（2026-07-16 确认）：**
  - **云端 Sales Automation：禁止 Gmail 实发**（无本机 MCP）。只允许：扩买家、对齐/补草稿、更新 `pipeline`/`sales.md`、写 `today.md` 完成回写。
  - **Gmail 实发：仅本机**，由 **Co-founder 每日触发**：对话说 **`今天发`**。Agent 按配额连发，发完只回摘要（禁止广搜 Gmail 已发送对账；以 `pipeline` 为账本）。
- **日配额：** 固定 **15 封/工作日**（周一至周六；周日不发冷邮）。`今天发` = 发满当日剩余额度至 15；`今天发 N` 时 N≤15（除非 Co-founder 显式提高上限）。
- **停止条件：** `sales.md` / `pipeline` 中 **Contacted（成功投递）≥ 100** → **默认停止日配额新冷邮件**。**A 软切选项 2 例外（2026-08-03）：** 允许对 **`buyer_class: A` 且 Stage=Lead** 发首封冷邮（仍禁 B/C 冷邮；禁 Sales 日扩新名）。已 Contacted 的跟进与回信处理可继续。进入 `W4_FOLLOWUP` 仍须另满足 **回复 ≥5**（见 `phases.md`）。
- **Bounce：** 只记账（Stage 保持 Lead 或 Notes 标 Bounce）；**不自动**改备用邮箱补发。仅当 Co-founder 明确说「改发备用 / 改发 #N」时才重发。Bounce **不计入** Contacted。
- **逐封串行 + 即时写回（防重复）：** 每调用一次 Gmail send 成功后，**立即**更新 `pipeline.md`（Stage→Contacted + Notes 写 msg ID），确认写回后才发下一封。**禁止**同一轮 tool call 并行多封。断线恢复后**不自动重发**——先报告「断在第 N 封，最后成功 #X」，等 Co-founder 确认再继续。
- **护栏：** 跳过无邮箱 / 已 Contacted（新冷邮）/ 已 Bounce 且未下令改发 / 队列标明跳过（#3、#13、#15 电话脚本）/ **`buyer_class: C`** / **A 软切期间跳过 B** / **#41 Martin 暂不催**；署名 **Kit Lee** · Export — YUEFU BBQ, Foshan, China；首封无附件；W3 可用 indicative market FOB（见 `product.md`）。
- **买家分层：** 见 [`customers.md`](customers.md)。**A 软切 + 选项 2：** 日配额优先 **A Lead 首封**；可穿插 A Contacted 跟进；**暂停日扩 +5**；C 停联；B 不跟不扩。
- 仅以下动作**必须真人**：微信/电话、付款、报关、验货、签约；每日说一次 **`今天发`**；以及 LinkedIn 手发后说 **`LinkedIn 发出去`**（见下方 LinkedIn 触达政策）。
- **Agent 不假装是真人身份**——署名用 `Kit Lee`，不冒充其他身份。

### LinkedIn 触达政策（全公司唯一来源）

> 本节是 **LinkedIn 客源触达**（连接请求 / InMail / DM）政策的**唯一归属**。与上方「发信政策」（邮件）并列，**不得**混进邮件节。其他文档需要时**只指向此处**。字段写法 → [`../workspace/buyers/pipeline.md`](../workspace/buyers/pipeline.md)；Sales 职责 → [`../workflows/sales.md`](../workflows/sales.md)。买家分层 → [`customers.md`](customers.md)。

- **与邮件并行，不互相替代。** LinkedIn **不计入** `Contacted`、**不占** Gmail 日配额 15、**不触发** Contacted≥100 停冷邮；仍受 A 软切 / 选项 2 / C 停联约束。
- **触发词：** 本机 Co-founder 说 **`LinkedIn 发出去`**（≠ `今天发`）。默认只起草；未说触发词前不得记为已触达。
- **执行拓扑：**
  - **云端 Sales Automation：禁止 LinkedIn 实发**；只允许补决策人 URL、对齐连接/InMail 草稿、写 `pipeline` Notes。
  - **实发：仅 Co-founder 本人**在 LinkedIn 手点；Agent 列目标 + 草稿，发出后按触发词写 Notes。
  - **禁止**把账号交给外部代发私信；Agent **不**假装是真人身份（署名 Kit Lee · Export — YUEFU BBQ, Foshan）。
- **日量：** 连接请求 **3–5**/工作日（周一至周六）；InMail **0–2**（有额度再用）。数字只在本小节规定。
- **不进日配 P0：** LinkedIn **不写入** `today.md` P0，**不进** Founder 09:00 邮件日配；由本机触发词或明确「启动 Sales」LI 任务执行。
- **账本（同一 `pipeline.md`，不另开 LI 账本）：**
  - 触达只追加 Notes：`YYYY-MM-DD LI connect @Name` 或 `YYYY-MM-DD LI InMail @Name`。
  - **禁止**因 LinkedIn 改 `Stage` 或 `Last Contact`（`Last Contact` = 最近一次 Gmail 成功投递）。
  - 连接成功、InMail 已送、LinkedIn 系统通知 **都不是** `Replied`。
  - **任一渠道真人采购回复**（邮件正文或 LI 消息）→ 可标 `Replied`（见 [`sales.md`](sales.md)）。
- **9/6 前范围（线 A）：** 只对 **`pipeline.md` 已有行** 且 **`buyer_class: A`**；**禁止因 LinkedIn 新增公司行**（≠ 日扩例外；选项 2「不找新公司名」仍有效）。禁 **B**；禁 **C** / Do-not-contact；禁催 **`#169` Brad**、**`#41` Martin**。
- **优先序（少与当日冷邮抢同一批）：** A Contacted 静默（已有个人 URL）> 无邮箱 / Bounce 的 A Lead > 有可用邮箱的 A Lead（后者不堵当日 `今天发` 队列）。
- **话术：** 补位/不替代；不编造 MOQ / 样品价；连接备注短（≤300 字符）。草稿 → `workspace/buyers/outreach-drafts.md`。

---

## 待答问题收件箱

> 从 `founder.md` 移入已答项。 Founder Agent 提问 → 你在此回答 → Agent 更新其他文件。

### 开放问题

（暂无）

### 已回答

| 日期 | 问题 | 回答 |
|------|------|------|
| 2026-08-03 | Martin 凉后是否开发新客户 | **选项 2**：不找新名；对库存 **A Lead** 开冷邮（放宽 ≥100 停冷邮例外） |
| 2026-08-02 | Research Reset 路径 A/B/C | **A 软切**：保持 W3+澳；停日扩；跟进仅 buyer_class A；8/9 再评估正式 Research |
| 2026-07-10 | 每天投入时间 | **约 2 小时/天** |
| 2026-07-10 | 英文水平 | **B：能读，AI 起草**（发信政策见分工原则：不禁止自动发信） |
| 2026-07-10 | 外贸经验 | **A：无，第一次** |
| 2026-07-10 | 对外署名 | **Lee Wing Kit** → **2026-07-15 改为 Kit Lee** |
| 2026-07-10 | YUEFU 关系 & 询价 | **父亲朋友开的厂；未报价；先找买家再谈价，帮工厂开市场** |
| 2026-07-10 | 何时问叔叔 | **先找潜在买家，有询盘/Qualified 后再问**出口史与厂价 |

---

## 真人动作记录

> 只有人能做的事，记一笔，方便 Founder Agent 掌握进度。

| 日期 | 动作 | 结果 |
|------|------|------|
| 2026-07-10 | 提供 YUEFU 2025 目录 PDF | 已归档至 `workspace/suppliers/yuefu-bbq/` |
| 2026-07-11 | 启用 Cursor Automation「Kamado 找买家 — 澳洲」 | **已取代** → 见下行 |
| 2026-07-12 | 初始化 GitHub 仓库 + 改 Public | https://github.com/leeyongjielife-eng/china-oven-export |
| 2026-07-12 | 启用 **「Kamado 每日 Founder — 澳洲」** | **Active**；每天 09:00 · `main` |
| 2026-07-12 | 启用三 Automation + `phases.md` 阶段机 | Founder/Sales/Research · GPT-5.5 Medium |
| 2026-07-16 | 搭建并验证 **Gmail MCP** | ✅ 已连接；本机实发 |
| 2026-07-16 | 确认日配额自动发信规则 | 触发 `今天发`；配额 **15**/工作日；**Contacted≥100** 停新冷邮；Bounce **只记账不自动补**；云端 Sales **禁止** Gmail |
| — | 向 YUEFU 要正式报价 / 问出口史 | **暂缓**，等有潜在买家询盘或 Qualified 后再问（2026-07-10 战略决定） |
