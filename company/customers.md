# Customers

## 理想买家画像（第一阶段）

**主目标：Kamado 烤炉海外买家**（根据 YUEFU 实际产品调整）

### Top 买家类型（待 Week 2 验证排序）

1. **BBQ / 户外厨具分销商** — 进口 Kamado 转售给零售店
2. **庭院 / 户外生活 (outdoor living) 零售商** — 家装、园艺渠道
3. **电商平台卖家** — Amazon、eBay 卖家（13"/16" 轻小件适合）
4. **餐厅户外用餐区** — 需烟熏、披萨、烧烤的餐厅
5. **现有 Kamado 品牌 OEM/白标客户** — 工厂支持定制

### 买家关心什么（假设，用真实对话验证）

| 关注点 | 重要性 | 我们怎么回应 |
|--------|--------|--------------|
| 价格 vs Big Green Egg 等 | 高 | FOB 价 + 对比零售价空间 |
| EN1860-1 / FDA 认证 | 高 | 备好证书扫描件 |
| 陶瓷质量 / 开裂率 | 高 | 工厂质检流程 + 包装方案 |
| 运输 / 包装（易碎） | 高 | 陶瓷特殊包装，运费按毛重算 |
| 保修 / 备件（垫片、烤网） | 中 | 确认供应商条款 |
| MOQ | 中 | 13"/16" 可试 1-2 台，大柜 MOQ 问工厂 |
| OEM / 贴牌 | 中 | 工厂支持定制，可谈 |

## 目标市场

### 候选国家（2026-07-10 Research 结论）

| 国家 | 加权分 | 竞争 | 认证 | 优先级 |
|------|:---:|------|------|:---:|
| **澳大利亚** | 4.30 | BGE/KJ 占高端，中国有空间 | 炭烤免 AS/NZS 燃气证；ChAFTA | ⭐ **首选** |
| 英国 | 3.85 | 强 | EN1860-1 对口 | 第二 |
| 南非 | 3.45 | KJ 独家 | 待问叔叔 | 第三 |
| 美国 | 2.75 | 极强 | Prop 65 | 后期 |
| 菲律宾 | 3.30 | 低 | RCEP | 需求弱 |

### 第一个目标市场（2026-07-10 确定）

**国家：澳大利亚**

**选择理由：**
1. **关税与合规最友好** — ChAFTA + 原产地证可 0% 关税；纯炭烤避开 AS/NZS 燃气强制认证；EN1860-1/FDA/LFGB 作质量背书
2. **与 Lee 能力匹配** — 全英语；中小 BBQ 分销/专营店可 cold email（AI 起草→确认），符合 2h/天
3. **工厂已验证 + 运费可控** — YUEFU 目录已列出口澳洲；佛山→悉尼/墨尔本航线短；BGE Large 澳零售约 AUD $2,000+ 证明溢价空间

**First niche：** mid-size BBQ equipment distributors / specialty outdoor retailers (5–50人) — 主推 18"/21"

## 非目标客户（暂不碰）

- 大型工业烘焙工厂（订单复杂、认证要求高）
- 只要最低价、不在乎质量的买家
- 要求本地安装+维修打包的买家（现阶段做不了）
- **`buyer_class: C`** — Weber Store / Weber Specialist / Barbeques Galore 加盟等**无海外工厂采购权**的品牌专营/加盟店（**任何渠道均不联系**）

## 采购权分层 `buyer_class`（2026-08-02）

> **不同于** `contact-ready: A/B/C`（联系人完整度）。本字段表示**能否自主采购中国工厂货**。

| buyer_class | 含义 | 联系策略（本阶段） |
|-------------|------|-------------------|
| **A** | 进口商 / 批发分销 / 独家分销 / 自有品牌 OEM·制造商 | **可联系**；**新扩买家只收 A** |
| **B** | 独立多品牌专营/电商，有自采可能 | **默认可跟进**；**暂不新扩 B** |
| **C** | Weber/BBQG 加盟或品牌专营店等，店面无海外工厂采购权 | **`Do-not-contact`**：邮件/LinkedIn/电话/表单**全停** |

**判定优先序：** 先认 C 信号（Weber Store/Specialist、Barbeques Galore 加盟等）→ 再认 A 信号（importer/distributor/OEM/own-brand/ICP）→ 其余默认 B。兼有 C 与 A 信号时：若主体是 **加盟店/品牌专营店** 且 A 仅是笔记推测（如 “importer potential”），仍标 **C**；若确有自有品牌/OEM/批发采购权（如 Ziegler、Firehawk），标 **A**。

**闸门（Sales / Founder）：**

1. **质量：** 新扩必须 **100% 为 A**；出现 B/C → 违例，立刻改找买家策略  
2. **库存：** **`A Lead < 20` → 必须补 A**；或本周已派 Sales 扩量但 **净增 A = 0 → 也必须补 A**

账本写法（Notes）：`buyer_class: A|B|C · procurement: yes|unknown|no`；C 另加 `Do-not-contact`。

## 已接触买家

明细 → [`../workspace/buyers/pipeline.md`](../workspace/buyers/pipeline.md)  
分层摘要 → [`../workspace/buyers/buyer-class-summary.md`](../workspace/buyers/buyer-class-summary.md)
