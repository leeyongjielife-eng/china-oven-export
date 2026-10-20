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
| **phase_id** | `W4_FOLLOWUP` |
| **名称** | 跟进 / Qualified（英新冷邮并行） |
| **起始** | 2026-10-09（英国 Replied 5 达标；Co-founder 拍板） |
| **下一 phase_id** | 有 ≥1 Qualified → 触发 Quoting/Supplier；英国 Contacted≥300 → 停英新冷邮（2026-10-09 由 100 改为 300） |
| **本期唯一指标** | **Qualified 数**（2026-10-20 → 2026-11-03 · Co-founder 拍板）；Contacted / 补A 数不作为进度 |
| **补A** | **暂停**（2026-10-20 起 · 英 A Lead 101）；英 A Lead &lt;20 时才恢复 |
| **最后更新** | 2026-10-20 |

---

## 阶段定义与切换门槛

| phase_id | 名称 | Sales 日常 P0 | 发信 | 切换条件（满足 **全部**） |
|----------|------|---------------|------|---------------------------|
| `W2_COLLECT` | 积 50 买家 | +10 **英国 A**/天 | **禁止**（英名单未齐；澳停新冷邮） | **英国 A** ≥50 → 进入 `W3_OUTREACH` |
| `W3_OUTREACH` | 外联 100 | **外联 15/工作日**（本机）+ 新买家 5/天（须英国 A） | **允许**（仅本机 Gmail；**只打英国**） | **英国回复 ≥5** → `W4_FOLLOWUP`；**英国 Contacted≥300** → 停英新冷邮（澳 256 不计入） |
| `W4_FOLLOWUP` | 跟进 / Qualified | 英新冷邮为主 + 热线索带新理由回访 + 跟进 Contacted | 允许（仅本机 Gmail；**只打英国**；英新冷邮至英 Contacted≥300） | 有 ≥1 Qualified → 触发 Quoting/Supplier |
| `W3_RESEARCH_RESET` | 市场复核（异常） | 暂停扩 buyer，等 Research 结论 | 暂停扩量 | 仅当 **连续 3 周回复率 &lt;5%** 时 Founder 手动切入 |

### 切换时 Founder 必须做

1. 更新上表「当前阶段」`phase_id`
2. 写 `founder.md` 新阶段排期 + 调度日志
3. 下一日 `today.md` 按新阶段 P0 派发
4. 在摘要中列出 **Co-founder 待办**（见下表）

### Co-founder 阶段待办

| 切换到 | Co-founder 必须 / 建议 |
|--------|------------------------|
| `W2_COLLECT` | 积名单期间不发英冷邮；澳热线索仅回信。英国 A 满 50 后 Automation 自动切 W3 |
| `W3_OUTREACH` | ✅ Gmail MCP 已通；**每日本机说 `今天发`**（15 封，**只打英国**）；云端 Sales **不实发** |
| `W4_FOLLOWUP` | 每日本机说 `今天发`（15 封，冷邮与跟进共用）；热线索回访须点名授权。厂 FOB/出口史 **2026-09-21 已拿到**；有 Qualified 时再问叔叔柜下试单量价、付款方式 |
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
| `W2_COLLECT`（**已完成 2026-09-10** · 英 A 50/50） | — | — |
| `W3_OUTREACH`（**已完成 2026-10-09** · 英 Replied 5） | 对齐草稿 / 标明今日应发英 #N→#M（**勿 Gmail 实发**；跟进仅 **英国 A+B**，跳过 **C**；**不**跟进澳静默户） | +5 新买家（**必须 100% 英国 A**） |
| `W3_OUTREACH` + **A 软切 + 选项 2**（**已结束 2026-09-09**） | — | — |
| `W4_FOLLOWUP`（**当前** · 2026-10-09 起） | 英新冷邮（英国 A Lead，从 `#425` 起）+ 跟进 Contacted 未回复（仅英 A+B） | 推进 Replied → Qualified（热线索回访带新理由，须授权）；**补A 暂停**（2026-10-20 起，英 A Lead &lt;20 才恢复） |
| `W3_RESEARCH_RESET`（**已结束 2026-09-09 确认换英**） | — | — |

**硬约束（全阶段 until Co-founder 改 phases）：** 厂 FOB/出口史已于 2026-09-21 拿到；再问叔叔（试单量价、付款方式）仅限 `W4` 且 Qualified；**`buyer_class: C` = Do-not-contact**；新扩 **仅英国 A**；澳停新冷邮。**英 Contacted 从 0 起算**（澳 256 归档，不挡英线）。`W3`/`W4` 实发仅本机「今天发」。

---

## Research 定期执行

| 类型 | 频率 | 谁跑 | 产出 |
|------|------|------|------|
| **轻量复核** | **每周日 09:00** | Research Automation | `research.md` 周日志 + 关键词微调 |
| **正式选市场/换市场** | 事件触发 | 你说 **`正式Research`** | 填满 scoring + `customers.md` |

### 轻量复核清单（30 分钟）

- [ ] 英零售锚点是否变化 → 更新或确认 [`competitor-benchmark.md`](../workspace/markets/competitor-benchmark.md)
- [ ] 补 3–5 个关键词 → [`keywords.md`](../workspace/markets/keywords.md)
- [ ] 写 5 行本周研究日志 → `research.md`
- [ ] 若**英线**外联回复率连续 3 周 &lt;5% → 在日志建议 Founder 切换 `W3_RESEARCH_RESET`

**轻量复核 ≠ 正式Research**；不重选国家，除非触发异常门槛。

---

## 防「永远找买家」规则

| 条件 | Founder Automation 行为 |
|------|-------------------------|
| `phase_id=W2_COLLECT` 且 **英国 A** ≥50 | **自动**更新为 `W3_OUTREACH`，P0 改为英外联 |
| `phase_id=W3_OUTREACH` | P0 **不得**再是「+10 买家」；以发信为主；P1 新买家 **100% 英国 A** |
| **A 软切**（**已结束 2026-09-09**） | — |
| **选项 2** | 已结束 |
| `英国 A Lead < 20`（`W3_OUTREACH` / `W4_FOLLOWUP`）或本周扩量净增英 A=0 | 必须补英 A |
| `phase_id=W3_RESEARCH_RESET` | **禁止**派 Sales 日扩 / 日配新冷邮；等正式Research 结论 |
