# 阶段状态机（Phase SSOT）

> **本文件唯一归属**：当前处于哪一阶段、切换条件、各阶段 Founder 应派发什么任务。
> Founder Automation **必须先读**本文件，再写 `today.md`。
>
> | 需要的信息 | 读取 |
> |-----------|------|
> | 周计划细节 | [`../plan/week-0X.md`](../plan/) |
> | 漏斗数字 | [`sales.md`](sales.md) |
> | Research 怎么做 | [`../workflows/research.md`](../workflows/research.md) |
> | 派发格式 | [`../workspace/dispatch/today.md`](../workspace/dispatch/today.md) |

---

## 当前阶段（Founder 维护）

| 字段 | 值 |
|------|-----|
| **phase_id** | `W3_OUTREACH` |
| **名称** | Week 3 — 外联 100 |
| **起始** | 2026-07-14 |
| **下一 phase_id** | `W4_FOLLOWUP` |
| **最后更新** | 2026-07-16 |

---

## 阶段定义与切换门槛

| phase_id | 名称 | Sales 日常 P0 | 发信 | 切换条件（满足 **全部**） |
|----------|------|---------------|------|---------------------------|
| `W2_COLLECT` | 积 50 买家 | +10 买家/天 | **禁止** | 买家 ≥50 → 进入 `W3_OUTREACH` |
| `W3_OUTREACH` | 外联 100 | **外联 15/工作日**（本机 Co-founder 触发）+ 新买家 5/天（云端可做） | **允许**（仅本机 Gmail） | 已联系 ≥100 **且** 回复 ≥5 → `W4_FOLLOWUP`；**Contacted≥100 即停日配额发信** |
| `W4_FOLLOWUP` | 跟进 / Qualified | 跟进 + Qualified 对话 | 允许 | 有 ≥1 Qualified → 触发 Quoting/Supplier |
| `W3_RESEARCH_RESET` | 市场复核（异常） | 暂停扩 buyer，等 Research 结论 | 暂停扩量 | 仅当 **连续 3 周回复率 &lt;5%** 时 Founder 手动切入 |

### 切换时 Founder 必须做

1. 更新上表「当前阶段」`phase_id`
2. 写 `founder.md` 新阶段排期 + 调度日志
3. 下一日 `today.md` 按新阶段 P0 派发
4. 在摘要中列出 **Co-founder 待办**（见下表）

### Co-founder 阶段待办

| 切换到 | Co-founder 必须 / 建议 |
|--------|------------------------|
| `W3_OUTREACH` | ✅ Gmail MCP 已通；**每日本机说 `今天发`**（15 封）；云端 Sales **不实发** |
| `W4_FOLLOWUP` | 有 Qualified 时 **问叔叔** YUEFU FOB/出口史 |
| `W3_RESEARCH_RESET` | 说 **`正式Research`** 或确认 Founder 调度 Research |

---

## Founder 每日派发规则（Automation 09:00）

```text
1. 读 phases.md「当前阶段」+ sales.md 漏斗
2. 检查切换条件 → 若满足，更新 phase_id 并写 founder.md
3. 按当前 phase_id 写 today.md（仅 Sales 可执行项）
4. 禁止写 pipeline / 草稿
5. git push
```

| phase_id | today.md P0 模板 | today.md P1 模板 |
|----------|------------------|------------------|
| `W2_COLLECT` | +10 澳洲买家 → 目标 X/50 | 补外联草稿（若排期有） |
| `W3_OUTREACH` | 对齐草稿 / 标明今日应发 #N→#M（**勿 Gmail 实发**） | +5 新买家 |
| `W4_FOLLOWUP` | 跟进 Contacted 未回复 | 推进 Replied → Qualified |
| `W3_RESEARCH_RESET` | **不派 Sales 扩量**；today 可写「暂停，等 Research」 | — |

**硬约束（全阶段 until Co-founder 改 phases）：** 不问叔叔（除非 `W4` 且 Qualified）；`W2` 不发信。

---

## Research 定期执行

| 类型 | 频率 | 谁跑 | 产出 |
|------|------|------|------|
| **轻量复核** | **每周日 09:00** | Research Automation | `research.md` 周日志 + 关键词微调 |
| **正式选市场/换市场** | 事件触发 | 你说 **`正式Research`** | 填满 scoring + `customers.md` |

### 轻量复核清单（30 分钟）

- [ ] 澳洲 Kamado 竞品零售价是否变化 → 更新或确认 [`competitor-benchmark.md`](../workspace/markets/competitor-benchmark.md)
- [ ] 补 3–5 个关键词 → [`keywords.md`](../workspace/markets/keywords.md)
- [ ] 写 5 行本周研究日志 → `research.md`
- [ ] 若外联回复率连续 3 周 &lt;5% → 在日志建议 Founder 切换 `W3_RESEARCH_RESET`

**轻量复核 ≠ 正式Research**；不重选国家，除非触发异常门槛。

---

## 防「永远找买家」规则

| 条件 | Founder Automation 行为 |
|------|-------------------------|
| `phase_id=W2_COLLECT` 且 买家 ≥50 | **自动**更新为 `W3_OUTREACH`，P0 改为外联 |
| `phase_id=W3_OUTREACH` | P0 **不得**再是「+10 买家」；以发信为主 |
| 漏斗长期无回复 | 周日 Research 日志提醒；Founder 周复盘考虑 `W3_RESEARCH_RESET` |
