# Founder → Sales 任务交接（Dispatch）

> **本目录唯一归属**：Founder 向 Sales 派发的**当日可执行任务单**（操作层 SSOT）。
>
> | 需要的信息 | 读取 |
> |-----------|------|
> | 战略排期、周计划、明日计划 | [`company/founder.md`](../../company/founder.md)（Founder 维护，**不复制到本目录**） |
> | 周节奏日历 | [`plan/week-0X.md`](../../plan/) |
> | Sales 角色边界与写法 | [`workflows/sales.md`](../../workflows/sales.md) |
> | 发信政策 | [`company/cofounder.md`](../../company/cofounder.md) 发信政策 |
| 阶段与派发规则 | [`company/phases.md`](../../company/phases.md) |

## 与现有文件的分工（避免重复）

| 文件 | 层级 | 谁写 | 存什么 | 不是 |
|------|------|------|--------|------|
| `plan/week-XX.md` | 周 | 人/Founder | 本周日历与指标 | 当日任务单 |
| `company/founder.md` | 战略 | **Founder** | 阶段判断、今日/明日排期、调度**日志** | Sales 执行清单 |
| **`dispatch/today.md`** | **操作** | **Founder 派发 / Sales 回写** | **当日 Sales 唯一任务单 + 状态** | 战略、Co-founder 任务 |
| `company/sales.md` | 摘要 | **Sales** | 漏斗数字 | 任务明细 |
| `workspace/buyers/pipeline.md` | 数据 | **Sales** | 买家明细 | 任务单 |

**硬规则：**

1. **Co-founder 任务**（微信、付款、Automation 开关等）→ 只写在 `founder.md` 或 `cofounder.md`，**不进** `today.md`。
2. **Founder 不写** `pipeline.md` / `outreach-drafts.md`（除非 Founder 会话且尚未派发 Sales）。
3. **Sales 不改** `founder.md` 排期 / `strategy.md`；只读 `today.md` 并回写本文件「完成态」+ 业务文件。
4. 战略内容用**指针**（见 `founder.md` §…），不在 `today.md` 复制大段排期。

## 状态机

```text
empty → pending → in_progress → done
  ↑        │           │           │
Founder   Founder     Sales       Sales
清空/等待  写入任务    开始执行    填完成回写
```

| status | 含义 | Sales Automation 行为 |
|--------|------|------------------------|
| `empty` | 尚未派发 | **停止**，不执行 |
| `pending` | 已派发 | 读取任务 → 改为 `in_progress` → 执行 |
| `in_progress` | 执行中 | 继续或完成 |
| `done` | 已完成 | **停止**，不重复执行 |

## Research 步骤（周日 09:00 Automation）

> **轻量复核**，不是 `正式Research`。切换/深研见 [`company/phases.md`](../../company/phases.md)。

1. 读 `company/` 8 文件 + `phases.md` + `sales.md`（回复率）
2. 执行 [`company/phases.md`](../../company/phases.md)「轻量复核清单」
3. 写 `research.md` 周日志（≥5 行）
4. 若回复率连续 3 周 &lt;5% → 日志建议 Founder 考虑 `W3_RESEARCH_RESET`
5. **禁止**写 pipeline / 外联 / 改 `customers.md` 目标国（除非 Founder 显式触发正式Research）
6. git commit && git push

## Founder 步骤（09:00 Automation · 周一至周六）

1. 读 `company/` 8 文件 + **`company/phases.md`** + `founder.md` 排期 + `sales.md` 漏斗
2. 检查阶段切换门槛 → 若满足，更新 `phases.md` + `founder.md`
3. 按 `phases.md` 当前 `phase_id` 写 `today.md`（`status: pending`；仅 Sales 任务）
4. 更新 `founder.md` 调度日志；**禁止**写 pipeline / 草稿
5. 若刚切换阶段 → 摘要列出 Co-founder 待办（如 Gmail MCP）
6. `git commit && git push`

## Sales 步骤（10:00 Automation · 周一至周六）

> Cursor 定时器仅支持整点，Sales 排在 Founder **1 小时后**，确保 `today.md` 已 push。
>
> **硬约束（2026-07-16）：云端本步骤禁止 Gmail 实发。** 实发仅本机 Co-founder 触发 `今天发`（见 `company/cofounder.md`）。

1. 读 `today.md`：若 `status` 不是 `pending`，停止。
2. 改为 `in_progress`；读 [`workflows/sales.md`](../../workflows/sales.md)。
3. 执行 **可云端完成** 的 P0/P1：扩买家、对齐/补草稿、同步漏斗。**不要**调用 Gmail MCP / 发送外联。
4. 在完成回写中注明「今日应发序号 → 待 Co-founder `今天发`」。
5. `status: done`；`git commit && git push`。
6. **禁止**改 `founder.md` 排期。

## Founder 签收（可选 · 次日或同日第二次 Run）

1. 读 `today.md` 完成回写 + `sales.md` 漏斗。
2. 在 `today.md`「Founder 签收」填 ✅/备注。
3. 更新 `founder.md`：今日完成态、明日排期、调度日志。
