# 子代理模型分工 + 额度节省策略

> **原则：默认中等模型；只有点名高级场景时才切高级模型。**
>
> 写进文档不耗额度。实际调用哪个模型，才扣哪个模型的配额。

---

## 额度节省策略

### 两档模型

| 档位 | 何时用 | 额度 |
|------|--------|------|
| **默认（Standard）** | 日常聊天、轻量任务、批量草稿 | 省 — 中等模型池 |
| **高级（Premium）** | 仅当 Co-founder **点名触发词** | 贵 — thinking / fast-high 池 |

### 默认聊天

- Cursor 窗口保持 **中等模型**（推荐 `gpt-5.5-medium` 或 `composer-2.5-fast`）
- 未点名高级场景时，即使说「启动 Founder」，也按 **Founder 默认模型** 执行

### 高级场景触发词（仅此两种默认升档）

| 场景 | 你说 | 子代理 | 升档模型 |
|------|------|--------|----------|
| 每周战略复盘 | `Founder复盘` / `每周复盘` | Founder | `claude-opus-4-8-thinking-high` |
| 正式市场调研、选定第一市场 | `正式Research` / `选市场` | Research | `grok-4.5-fast-xhigh` |

其他子代理**一律用默认档**，不自动升高级。

### 每周额度预算建议（2h/天）

| 频率 | 任务 | 档位 |
|------|------|------|
| 每天 | 闲聊、排期、写邮件草稿、找买家 | 默认 |
| 每周 1 次 | Founder 复盘 | 高级 |
| Week 2 集中 1 次 | 正式 Research 选市场 | 高级 |
| 有 Qualified 买家时 | 正式 Quoting | 默认（terra 够用） |

---

## 模型映射表

| 子代理 | 默认模型 | 高级模型 | 高级触发词 | 工作特点 |
|--------|----------|----------|------------|----------|
| **Founder** | `gpt-5.5-medium` | `claude-opus-4-8-thinking-high` | `Founder复盘` `每周复盘` | 日常排期用默认；跨文件战略合成用高级 |
| **Research** | `gpt-5.5-medium` | `grok-4.5-fast-xhigh` | `正式Research` `选市场` | 轻量查关键词用默认；联网选国用高级 |
| **Supplier** | `gpt-5.6-terra-medium` | — | — | 核验、询价，结构化即可 |
| **Offer** | `gpt-5.5-medium` | — | — | 改 Offer 频率低，默认够用 |
| **Sales** | `gpt-5.5-medium` | — | — | 邮件起草+发送（发信政策见 `company/cofounder.md`） |
| **Quoting** | `gpt-5.6-terra-medium` | `gpt-5.3-codex` | `正式报价`（发给买家前） | 草稿 terra；最终 PI 可升 codex |
| **Content** | `gpt-5.5-medium` | — | — | LinkedIn 短文，默认够用 |

---

## 当前聊天窗口推荐

| 你的状态 | 窗口顶部选 |
|----------|------------|
| **日常默认** | `gpt-5.5-medium` 或 `composer-2.5-fast` |
| Founder 复盘日 | 切 `claude-opus-4-8-thinking-high`，说 `Founder复盘` |
| 选市场那天 | 开 Task + `grok-4.5-fast-xhigh`，说 `正式Research` |

---

## Cursor Task 启动语法

```text
# 默认档（省额度）
Task(model: "gpt-5.5-medium", ...)

# 高级档（仅点名后）
Task(model: "claude-opus-4-8-thinking-high", ...)  # Founder复盘
Task(model: "grok-4.5-fast-xhigh", ...)             # 正式Research
```

---

## 备选降级（模型不可用时）

| 子代理 | 默认备选 | 高级备选 |
|--------|----------|----------|
| Founder | `composer-2.5-fast` | `claude-sonnet-5-thinking-high` |
| Research | `composer-2.5-fast` | `gpt-5.5-medium` |
| Supplier / Quoting | `gpt-5.5-medium` | `gpt-5.6-terra-medium` |
| Offer / Sales / Content | `composer-2.5-fast` | — |

---

## 维护规则

1. 新增子代理：默认必须用 **中等模型**，高级需写明触发词
2. 禁止把高级模型设为默认（除非有充分理由并记录）
3. 各 `workflows/<agent>.md` 的 `## 模型` 须同步本表
