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

### Week 3 周日轻量复核（2026-07-19）

- **日期**：2026-07-19；执行 Research 轻量复核，不做正式选市场，不改 `customers.md`。
- **竞品观察**：澳洲 Kamado 价格锚点仍合理；BGE Large 澳洲约 AUD $2,500–2,900，KJ Classic III 约 AUD $2,859–3,399，高端/数字款可到 AUD $4,000+。
- **已更新**：`workspace/markets/competitor-benchmark.md` 已补澳洲本地 BGE/KJ/BBQ Spit Rotisseries 价格与本周验证日期。
- **关键词补充**：`workspace/markets/keywords.md` 新增 5 个词，重点覆盖 trade account、ceramic smoker、outdoor kitchen showroom、BBQ wholesaler、LinkedIn company 搜索。
- **Sales 信号**：`sales.md` 当前显示 Contacted 0、Replied 0，但没有连续 3 周回复率历史；尚未满足自动建议切换 `W3_RESEARCH_RESET` 的证据条件。
- **建议**：Founder 继续保持澳洲单市场验证；若未来连续 3 个周日确认回复率 <5%，再在周日志中明确建议切换 `W3_RESEARCH_RESET`。

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
