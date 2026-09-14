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
- [x] **阶段 C — 正式选市场**（2026-07-10）→ **2026-09-09 正式Research 完成** → **Co-founder 确认换英（已生效）**
- [ ] 阶段 B 轻量补充（可选）

## 研究待办

- [x] 哪些国家从中国进口 Kamado / 陶瓷炭烤炉
- [x] 各目标国主要买家类型
- [x] 买家最关心：价格、认证、易碎运输、保修、MOQ
- [x] 主要竞争对手（BGE、KJ、中国出口商）
- [x] 新手最适合的第一个市场 → **英国**（2026-09-09 确认；替换澳）

---

## 研究结果摘要（2026-09-09 正式Research）

> 完整打分见 [`../workspace/markets/country-scoring.md`](../workspace/markets/country-scoring.md)。

### Top 3 目标国家

| 排名 | 国家 | 加权分 | 一句话 |
|:---:|------|:---:|--------|
| 1 | **英国** | **3.85** | EN1860-1 对口；自华固体燃料炉具进口件数约为澳 2 倍；独立进口商/白标渠道可冷邮 |
| 2 | **澳大利亚** | **3.75** | 关税/运费仍最优，但 256 冷邮实证 B 维失败（回复率 1.6%、0 Qualified） |
| 3 | **新西兰** | **3.55** | FTA+英语；TAM 太小，不作第一市场（南非 2.95 未进 Top 3） |

### 第一市场推荐

**换英。** 不是因为英国「更好看」，而是澳线 **B（冷邮可进入性）已用 256 封证伪**：结构优势（ChAFTA、短航线）挡不住「本地制造商 + 品牌加盟 + BGE/KJ 独家」墙。英国价值带已被中国 OEM 占领（Aldi/Lidl/B&Q/独立白标），YUEFU 的 EN1860-1 在那里是入场券不是空话。

### Top 3 买家类型（2026-09-09 重排，对英国）

1. **独立 BBQ / garden equipment 进口商与批发商**（已有中国货或自有品牌）— 决策人少、邮件节奏慢；排除 BGE/KJ 独家
2. **多店 garden centre / BBQ specialist 采购**（非超市全国总部）— 英国 DIY/garden 约占户外烹饪 40–45% 价值
3. **自有品牌电商 / 白标站**（Quinta / Kamado Kings 类）— 已知在进中国克隆；比餐厅/OEM 更适合 2h/天

暂缓：超市总部（Aldi/Lidl/B&Q 已有 Auplex 链）、餐厅、纯 Amazon 比价卖家。

### 推荐第一个细分 niche

```text
United Kingdom — independent BBQ / garden equipment importers & wholesalers
(已有中国货或 private label，非 BGE/KJ 独家) — 主推 18" Kamado
```

### 20 个搜索关键词

见 [`../workspace/markets/keywords.md`](../workspace/markets/keywords.md)（已按**英国**重填；澳词归档）

### 小单物流结论

- 21" 外箱 ≈0.36 CBM / 82kg，LCL 常按 **1 CBM 起收**；佛山→Felixstowe 公开参考约 **USD 507–675 / 1 CBM**、航程约 49–66 天（高于澳线）
- 试单优先 **18"** 或 **13"/16"**；21" 适合确认意向后 2–4 台拼箱
- 陶瓷按重量计费风险仍在（W/M 取大）

### HS 编码（待叔叔核实 — 未问）

- **主假设 7321.19**（固体燃料家用炉具）；本轮进口额用 WITS **732113**（HS1988/92 固体燃料对应码）
- **备选 6914.90**（陶瓷制品；美 CBP 陶土烤炉判例）
- **禁用 8514**
- 问叔叔报关单确认后，若实报 6914，须重跑 Comtrade，不得沿用本轮 7321 进口额

---

## 每周研究记录

### 2026-09-09 正式Research（选市场重评）

- **触发**：Co-founder 选 C；`W3_RESEARCH_RESET`；澳 Contacted 256 · Replied 4 · 回复率约 1.6% · 0 Qualified。
- **短名单**：澳大利亚、英国、南非 + 对照美国、新西兰。
- **WHERE（HS 7321.19 / WITS 732113，2024 自华进口）**：
  - 英 **USD 34.6M / 113 万件**；澳 **USD 32.6M / 54 万件**（金额接近，英件数约 2× → 更吃中国 OEM/低单价）；
  - 南非 **USD 3.3M / 22.5 万件**；新西兰 **USD 4.7M / 7.3 万件**；美 **USD 685M**（对照，不进）。
  - 不用 732112（液体燃料）当 Kamado 代理指标。
- **WHO**：
  - 澳：A 软切后名单偏本地制造商（Ziegler/Heatlie/Everdure）与不锈钢户外厨加工户，外加 BGE/KJ/Weber 墙 → 冷邮对象根本不买中国工厂货。
  - 英：Kamado Kings（B2B 批发）、Que Fresco（进口批发 Monolith 等）、独立白标（Quinta/Bono 类）、garden centre；B&Q GoodHome Sagami ~£500、Aldi/Lidl 季采 ~£250–300 证明中国陶瓷 Kamado 已进主流。
  - 南非：NF Importing = Kamado Joe **独家**；braai 文化强但真正陶瓷进口商薄。
- **PAIN**：价格空间仍在（英 BGE Large £1,495 vs indicative FOB USD 255–316）；认证英最匹配；运费英/南非差于澳；关税澳 0%、英 ~2%+VAT20%、南非约 15%+VAT15%。
- **竞品**：英价值带 = 中国克隆红海；澳高端被 BGE/KJ + 本地厂占满。我们的缝：给**尚未锁定独家工厂**的英进口商做 18" EN1860-1 补位，不跟 Aldi 拼 £250。
- **结论**：**换英为第一市场**（3.85 vs 澳 3.75）。**2026-09-09 Co-founder 已确认生效。** 未问叔叔。

### 2026-09-09 补评加拿大（Co-founder 追问）

- **为何原短名单没有加拿大：** 7/10 与 9/09 都按「英语 + 工厂已出口 + 关税友好」筛；加拿大 **无中加 FTA**（中国 2015 退出 GPT → MFN 8%），且北美渠道与美国高度同构（BGE 独家分销、本土大牌已从中国 OEM），先验上更像「缩小的美国」而不是「第二个澳洲」。
- **WHERE：** 2024 自华 732113 **USD 14.3M / 32.1 万件**（英 34.6M/113 万；澳 32.6M/54 万）。需求真实但规模约英的一半金额、三分之一件数。
- **WHO：** BGE Canada = Northwinds Marketing 全国分销、300+ 授权店；KJ 走独立专营店；**Broil King（Onward）、Napoleon、Pit Boss/Dansons 是加拿大品牌**——他们自己向中国下 OEM，不会买 YUEFU 补位线。未找到英式「Kamado Kings」批发进口商。
- **PAIN：** 炭烤一般不需 CSA 燃气证；须英/法双语 + Quebec；EN1860-1 在加不是入场券。佛山→温哥华 LCL 可行（约 16–25 天），好于英线。
- **打分：** A4 B2 C3 D4 E2 F3 → **加权 3.15**。**不改为第一市场**（换英已确认）。

### 2026-09-09 扩评：中东 / 日韩 / 墨西哥 / 荷德北欧 / 东南亚

- **触发**：Co-founder 要求除欧洲外这些区域都打分。同一权重；HS 仍 7321.19 假设；未问叔叔。
- **中东：** 阿联酋 **3.55**（英语贸易商、Jebel Ali 再出口、GCC ~5%）> 沙特 **2.90**（TAM 更大但 SABER/SASO+阿语）。kamado 文化弱于别墅燃气 BBQ；适合当**第二市场/再出口**，不适合第一枪。
- **荷德北欧：** 荷兰 **3.55** / 德国 **3.30** / 北欧 **3.15**。EN1860 与英同档，但 **BGE Europe HQ 在荷兰 De Lier**，花园中心价值带已是中国 OEM 红海。英比荷德更合适：英语决策 + 已点名独立批发商，且尚未被 BGE 欧洲总部压在同一国。
- **日韩：** 各 **3.10**。航线/RCEP 最好之一；日文/韩文 + 标签/PSC·KC 食品接触把新手冷邮打低。日本 2024 固体燃料器具进口量大但均价极低（大量非 kamado 炉具），不能当陶瓷 kamado TAM。
- **墨西哥：2.55（本表最低之一）。** 西语；中墨无 FTA；2026-01 对非协定国加税。不进。
- **东南亚：** 新加坡 **3.50**（转口/城邦）· 马来 **3.30** · 菲 3.30 · 泰 3.05 · 印尼 2.95 · 越 2.80。运费全胜，**A 需求弱**；越南更像竞品产地。
- **结论：** 扩评 **不推翻换英**。换英已确认；这些国仍不开线。

### 2026-09-09 确认换英（Co-founder 拍板）

- **决定：** 第一市场 = **英国**（`customers.md` 生效）。
- **阶段：** 退出 `W3_RESEARCH_RESET` → **`W2_COLLECT`**，积 **50** 英国 A（独立进口商/批发/白标）。
- **发信：** 满 50 前禁止英新冷邮；澳停新冷邮；澳热线索仅回信。英 Contacted 从 0 起算。
- **未做：** 不问叔叔；不开中东/日韩/荷德/东南亚/加拿大。

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

---

## 数据来源

| 来源 | 用途 | 备注 |
|------|------|------|
| **UN Comtrade / WITS** | 进口量 | 2024：732113 自华 英 34.6M / 澳 32.6M / 南非 3.3M / 新西兰 4.7M；**禁用 8514** |
| BGE/KJ 官网 + 英零售评测 | 零售价锚点 | 英 Large £1,495；澳仍 AUD ~2,500–3,400 |
| Alibaba/公开 OEM | 中国 FOB 参考 | $155–460/21"；Auplex 已供 B&Q/Homebase/Metro |
| 英 B2B 站 | 渠道验证 | Kamado Kings、Que Fresco、独立白标 |
| ABF / UK Trade Tariff / SARS | 关税 | 澳 ChAFTA 0%；英 UKGT ~2%+VAT20%；南非 7321.19 类约 15% |
| GCC / EU TARIC / 墨 2026 加税公告 | 扩评关税 | GCC 成品约 5%；EU 7321.19 ~2.7%；墨对非 FTA 2026 加征（7321 须逐码核） |
| **叔叔（仍未问）** | 实报 HS、南非清关、历史客户类型 | 有 Qualified 后再问 |

## 审核后必查项

- [ ] HS 编码核实（问叔叔；假设 7321.19 / 备选 6914）
- [x] 关税：澳 0%、英 ~2%（修正旧 1.7%）、美复杂、南非约 15%
- [x] 小单物流：21" LCL 按 1CBM 起收；英线 1CBM 公开参考 >USD 500
- [ ] 南非清关文件：待问叔叔
- [x] Co-founder 确认是否采纳「换英」 → **2026-09-09 确认**；切入 `W2_COLLECT`
