# Founder → Sales 任务交接（Dispatch）

> **本目录唯一归属**：Founder 向 Sales 派发的**当日可执行任务单**（操作层 SSOT）。
>
> | 需要的信息 | 读取 |
> |-----------|------|
> | 战略排期、周计划、明日计划 | [`company/founder.md`](../../company/founder.md)（Founder 维护，**不复制到本目录**） |
> | 周节奏日历 | [`plan/week-0X.md`](../../plan/) |
> | Sales 角色边界与写法 | [`workflows/sales.md`](../../workflows/sales.md) |
> | 发信政策 | [`company/cofounder.md`](../../company/cofounder.md) 发信政策 |

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

## Founder 步骤（09:00 Automation）

1. 读 `company/` 8 文件 + `founder.md` 今日/明日排期。
2. 从排期提取**仅 Sales 可执行**的 P0/P1 → 写入 `today.md`（`status: pending`）。
3. 更新 `founder.md` 调度日志一行：`Founder → Sales · 已派发 today.md`。
4. **禁止**写 `pipeline.md` / 外联草稿。
5. `git commit && git push`。

## Sales 步骤（09:15 Automation）

1. 读 `today.md`：若 `status` 不是 `pending`，停止。
2. 改为 `in_progress`；读 [`workflows/sales.md`](../../workflows/sales.md)。
3. 执行 P0/P1 → 写 `pipeline.md`、`outreach-drafts.md`、同步 `company/sales.md`。
4. 填 `today.md`「Sales 完成回写」；`status: done`。
5. **禁止**改 `founder.md` 排期。
6. `git commit && git push`。

## Founder 签收（可选 · 次日或同日第二次 Run）

1. 读 `today.md` 完成回写 + `sales.md` 漏斗。
2. 在 `today.md`「Founder 签收」填 ✅/备注。
3. 更新 `founder.md`：今日完成态、明日排期、调度日志。
