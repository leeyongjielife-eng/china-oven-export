# Research Log

> **Core:** find WHO buys → WHERE they buy → WHAT pain they have.
>
> | 文档 | 用途 |
> |------|------|
> | [`workflows/research.md`](../workflows/research.md) | 子代理工作流 |
> | [`markets/research-playbook.md`](../workspace/markets/research-playbook.md) | 分步手册 |
> | [`markets/country-scoring.md`](../workspace/markets/country-scoring.md) | 国家评分 |
> | [`markets/competitor-benchmark.md`](../workspace/markets/competitor-benchmark.md) | 竞品锚点 |

## 当前阶段

- [x] **阶段 A — 研究设计**
- [x] **阶段 C — 正式选市场**（2026-07-10，未问叔叔）
- [ ] 阶段 B 轻量补充（可选）

## 研究待办

- [x] 哪些国家从中国进口 Kamado / 陶瓷炭烤炉
- [x] 各目标国主要买家类型
- [x] 买家最关心：价格、认证、易碎运输、保修、MOQ
- [x] 主要竞争对手（BGE、KJ、中国出口商）
- [x] 新手最适合的第一个市场 → **澳大利亚**

---

## 研究结果摘要

### Top 3 目标国家

| 排名 | 国家 | 加权分 | 一句话 |
|:---:|------|:---:|--------|
| 1 | **澳大利亚** | 4.30 | 关税友好、英语、工厂已出口、BBQ 文化成熟 |
| 2 | **英国** | 3.85 | EN1860-1 对口，但运费远、竞争强 |
| 3 | **南非** | 3.45 | braai 文化强，但运费/关税高，待问叔叔 |

### Top 3 买家类型（验证后排序）

1. **BBQ / outdoor cooking 分销商或批发商** — 决策人少、邮件节奏慢，适合 Lee + AI 起草
2. **庭院/户外厨具 specialty 零售商**（有进口经验）— 澳市场大量存在
3. **电商卖家** — 暂缓作首攻（比价凶、响应要快）

### 推荐第一个细分 niche

```text
Australia — mid-size BBQ equipment distributors / specialty outdoor retailers
(约 5–50 人，有进口或批发经验) — 主推 18" 与 21" Kamado
```

### 20 个搜索关键词

见 [`../workspace/markets/keywords.md`](../workspace/markets/keywords.md)（已按澳大利亚填完）

### 小单物流结论

- 21" 外箱 ≈0.36 CBM / 82kg，LCL 常按 **1 CBM 起收**
- 试单优先 **18"** 或 **13"/16"**；21" 适合确认意向后 2–4 台拼箱

### HS 编码（待叔叔核实）

- 暂按 **7321**（非电炭烤炉）；美国海关判例有 **6912**（陶瓷家用器具，6%）
- 问叔叔报关单确认后再查 UN Comtrade

---

## 每周研究记录

### Week 1（2026-07-10）

- **做了什么**：Research 体系设计 + 独立审核 + 8 条优化；正式 Research（Grok）六国评分
- **结论**：首市场锁定 **澳大利亚**；美国留后期；叔叔出口史仍待补

### Week 2

- **待做**：按澳关键词找 10 买家入 pipeline；可选问叔叔验证 HS/南非

### Week 3 周日轻量复核（2026-07-19）· **已合入本仓 2026-07-20（来自 PR #5）**

- **日期**：2026-07-19；执行 Research 轻量复核，不做正式选市场，不改 `customers.md`。
- **竞品观察**：澳洲 Kamado 价格锚点仍合理；BGE Large 澳洲约 AUD $2,500–2,900，KJ Classic III 约 AUD $2,859–3,399，高端/数字款可到 AUD $4,000+。
- **已更新**：`workspace/markets/competitor-benchmark.md` 已补澳洲本地 BGE/KJ/BBQ Spit Rotisseries 价格与本周验证日期。
- **关键词补充**：`workspace/markets/keywords.md` 新增 5 个词，重点覆盖 trade account、ceramic smoker、outdoor kitchen showroom、BBQ wholesaler、LinkedIn company 搜索。
- **Sales 信号（复核当日云端读数）**：Automation 当时见 Contacted 0 / Replied 0（云端不实发）；**本机实发账本另计**（2026-07-20：已联系 **57** · 回复 **1**）。无连续 3 周回复率历史 → **不触发** `W3_RESEARCH_RESET`。
- **建议**：Founder 继续保持澳洲单市场验证；若未来连续 3 个周日确认回复率 <5%，再在周日志中明确建议切换 `W3_RESEARCH_RESET`。
- **外联侧观察（本机）**：#41 BBQ Republic 已 Replied；indicative FOB 口径可用；继续堆 Contacted。

### Week 3 周日轻量复核（2026-07-26）· **本机补做**（Automation 未产出 Research 提交）

- **日期**：2026-07-26；执行 Research 轻量复核，不做正式选市场，不改 `customers.md`。
- **Automation 观察**：同日约 09:00 云端有 **Founder/Sales Day 13** 提交，但 **无** `research.md` / 竞品 / 关键词相关 commit → 周日 Research Automation **未落盘或未跑**；由本机按 `phases.md` 清单补做。
- **竞品观察**：BGE Large AU 套装仍约 **AUD $2,500–2,999**；KJ Classic III 可见 **AUD $2,979**（挂牌约 $3,399）。相对 7/19 **无结构性变价**；indicative FOB USD $255–316 仍合理。
- **已更新**：`workspace/markets/competitor-benchmark.md`（验证日 2026-07-26）；`workspace/markets/keywords.md` 新增 **5** 词（#26–#30），偏向分销商 / 进口商 / OEM / 决策人搜索。
- **Sales 信号（本机 SSOT）**：已联系 **84** · 回复 **1** · 回复率约 **1.2%**。本周动作：冷邮收尾 + 两轮跟进（7/22、7/24）+ 战略改为「跟进 > 堆首封」+ ICP 收紧。
- **Research Reset 门槛**：连续 **3** 个周日回复率 &lt;5% 才建议切换。计数：**第 2 个周日**（7/19、7/26）均 &lt;5% → **暂不**建议 `W3_RESEARCH_RESET`；若 **2026-08-02** 仍 &lt;5%，再明确建议 Founder 切换。
- **建议**：保持澳洲单市场；周一继续跟进 `#34–#48` + 冷邮优先 ICP `#93–#98`；云端合入 `#100–#119`（多为 BBQG/Weber 区域店）发信优先级低于 ICP。

### Week 3/4 交界 周日轻量复核（2026-08-02）· **本机 Founder复盘补做**

- **日期**：2026-08-02；执行 Research 轻量复核 + Founder 周复盘；不做正式换市场，不改 `customers.md`（待 Co-founder 拍板）。
- **Automation 观察**：同日有 Founder/Sales（跟进派发 + `#155–#159`）提交，**无** Research 竞品/关键词 commit → 周日 Research Automation 再次未落盘；本机补周日志。
- **竞品观察**：沿用 7/26 锚点（BGE Large AU ≈ AUD $2,500–2,999；KJ Classic III ≈ AUD $2,979–3,399）。本周日未做全网重爬；indicative FOB USD $255–316 仍可用。**无证据显示定价是零回复主因。**
- **Sales 信号（本机 SSOT）**：买家 **159** · Contacted **113** · Replied **1** · 已联系 **114** · 回复率约 **0.9%**。已停新冷邮；今日本机跟进 `#34–#51` 批 15 封。
- **结构观察**：Contacted 中大量为 Weber/BG 区域零售；ICP 批 `#93–#98` + `#120–#123` 已触达但 **0 真回复**；唯一 Replied 仍是 `#41` Martin（kamado 专营）。`#101` 回 **Stop**。
- **Research Reset 门槛**：连续 **3** 个周日回复率 &lt;5% → **今日满足**（7/19、7/26、8/2）。
- **决策（同日晚 Co-founder）**：✅ **A 软切** — 保持 `W3_OUTREACH` + 澳；停 Sales 日扩；跟进仅 `buyer_class A`；**2026-08-09** 再评估是否 `正式Research` / 硬切。**未**改 `phase_id`。
- **建议（已执行）**：软切优先于立刻换国；1 周内盯第 2 条真回复与 Martin。

### Week 5 周日轻量复核（2026-08-16）· **Research Automation**

- **日期**：2026-08-16；执行周日轻量复核，**不是正式 Research**；不重选目标国，不改 `customers.md`。
- **竞品观察**：澳洲高端 Kamado 价格锚点仍合理；BGE Large 官方/零售约 **AUD $2,600–2,999**，KJ Classic III 约 **AUD $2,799–3,599**。相对 7/26 无结构性变价，indicative 21" FOB USD $255–316 仍可作为市场参考。
- **已更新**：`workspace/markets/competitor-benchmark.md` 验证日更新至 2026-08-16；`workspace/markets/keywords.md` 新增 **5** 个 A 类采购权关键词（#31–#35）。
- **Sales 信号（读 `sales.md`）**：买家 **188** · 已联系 **163** · 回复 **2**，当前回复率约 **1.2%**，仍明显低于 5%。
- **连续低回复判断**：7/19、7/26、8/2 已连续触发；8/9 复评仍低于 5%，本周 8/16 仍低于 5% → 满足并延续「连续 3 周回复率 <5%」异常门槛。
- **建议**：日志建议 Founder 切换或至少正式评估 `W3_RESEARCH_RESET`；在 Founder 手动改 `phase_id` 前，本次 Research 只记录建议，不替 Founder 改阶段。
- **边界**：不写 pipeline / 外联 / today.md；不新增买家；不问叔叔；不扩国家，只保留澳洲单市场验证结论供 Founder 决策。

---

## 数据来源

| 来源 | 用途 | 备注 |
|------|------|------|
| **UN Comtrade / WITS** | 进口量（智利等） | 免费；HS 待核实 |
| BGE/KJ 官网 | 零售价锚点 | 已填 competitor-benchmark |
| Alibaba/ImportYeti | 中国 FOB 参考 | $155–460/21" |
| 澳零售商网站 | 渠道验证 | BBQ Republic, The BBQ Store 等 |
| ChAFTA / UKGT 公开资料 | 关税 | 澳 0%、英 1.7% |
| **叔叔（待问）** | HS、南非/南美客户类型 | 成本最低验证 |

## 审核后必查项

- [ ] HS 编码核实（问叔叔）
- [x] 关税：澳 ChAFTA 0%、美复杂、英 1.7%
- [x] 小单物流：21" LCL 按 1CBM 起收，试单改 18"/16"
- [ ] 南非/南美：待问叔叔
