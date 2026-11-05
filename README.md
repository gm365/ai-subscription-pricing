# AI 订阅比价与会员价格对比指南（2026 实时更新）

**穿透渠道溢价与引流虚标，查清主流 AI 会员与 API 的真实到手价。**

[![数据实时更新于：shuita.xyz](https://img.shields.io/badge/数据实时更新于-shuita.xyz-0066FF?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shuita.xyz/)
[![MCP Server](https://img.shields.io/badge/MCP_Server-ai--price--mcp-8B5CF6?style=for-the-badge)](https://mcpservers.org/servers/gm365/shuita-ai-price)
[![收录店铺](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fshuita.xyz%2Fdata%2Fmeta.json&query=%24.stats.shops&label=%E5%AE%9E%E6%97%B6%E5%B7%A1%E6%A3%80%E5%BA%97%E9%93%BA&suffix=%2B%20%E5%AE%B6&color=10B981&style=for-the-badge)](https://shuita.xyz/)
[![在售方案](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fshuita.xyz%2Fdata%2Fmeta.json&query=%24.stats.items&label=%E7%8E%B0%E8%B4%A7%E5%9C%A8%E5%94%AE%E5%95%86%E5%93%81&suffix=%20%E4%BB%B6&color=F59E0B&style=for-the-badge)](https://shuita.xyz/)

> **核心导流提示**：AI 订阅渠道价格与库存随汇率及风控政策每日波动。本仓库提供基准参照，**早晚两次更新的现货底价、单店手续费明细与 30 天价格走势，请直接访问主站：[水獭 AI 订阅比价](https://shuita.xyz/)（shuita.xyz）。**

本仓库致力于提供客观、透明的 **AI 订阅比价**、**AI 会员价格对比**、**ChatGPT/Claude 订阅价格** 及 **AI API 价格对比** 索引。数据聚合自[水獭](https://shuita.xyz/)（shuita.xyz）每日两次对全网 133+ 家公开卡网、独立小铺及 Telegram 商店的实盘巡检，仅统计公开有货的店内实付价（标价 + 支付手续费），剔除 `¥0.1` 等虚假引流标价。

## 目录导航

* [主流 AI 会员订阅价格对比表](#主流-ai-会员订阅价格对比表)
* [常见规格深度拆解：直充、成品号与拼车](#常见规格深度拆解直充成品号与拼车)
* [主流大模型 API 价格对比（按百万 Tokens 计费）](#主流大模型-api-价格对比按百万-tokens-计费)
* [在 Cursor / Claude Code 中接入实时比价 MCP](#在-cursor--claude-code-中接入实时比价-mcp)
* [AI 订阅常见问题与避坑指南（FAQ）](#ai-订阅常见问题与避坑指南faq)
* [贡献与价格纠错指引](#贡献与价格纠错指引)

## 主流 AI 会员订阅价格对比表

以下表格汇总[水獭](https://shuita.xyz/)全网比价看板的实盘现货底价、全网均价以及各厂商官方美元定价。点击产品名称可直接跳转对应实时库存看板：

| 产品与订阅档位 | 官方定价（美区） | 官方折合人民币估算 | 水獭现货底价（含手续费） | 全网均价 / 在售规模 | 核心额度与并发限制 | 推荐使用场景 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **[ChatGPT Plus](https://shuita.xyz/sku/gpt_plus_topup)**（月付直充） | [$20 / 月](https://www.ai-toolbox.co/chatgpt-models/chatgpt-pricing) | 约 ¥135 ~ ¥145 / 月 | **¥104.96 起**（[菲区卡充](https://shuita.xyz/sku/gpt_plus_topup)） | 均价 ¥126（57 家有货 / 96 家在售） | 包含 GPT-6 Sol 日常对话、Deep Research 及 Codex 基础额度，保留个人历史记录 | 长期自用的主力对话、文档分析与日常轻度编程 |
| **[ChatGPT Plus](https://shuita.xyz/c/gpt)**（半价直充） | [$10 / 首月优惠](https://www.ai-toolbox.co/chatgpt-models/chatgpt-pricing) | 约 ¥72 / 月 | **¥56.00 起** | 价格带 ¥56 ~ ¥79.31（14 家有货） | 额度与正价 Plus 一致；仅限带有官方首月半价资格的账号充值，次月恢复正价 | 账号符合官方半价资格、希望低成本体验整月 Plus 的用户 |
| **[ChatGPT Pro](https://shuita.xyz/c/gpt)**（5X / 20X） | [$100 ~ $200 / 月](https://www.ai-toolbox.co/chatgpt-models/chatgpt-pricing) | 约 ¥720 ~ ¥1,440 / 月 | **¥575.00 起**（5X）/ **¥899.00 起**（20X） | 56 家有货（5X）/ 50 家有货（20X） | 解锁 GPT-6 Pro 与高倍 Codex 并发配额；需留意新开账号 20X 降额为 10X 的政策 | 每天长时间运行 Codex、高频触达 Plus 上限的重度研发人员 |
| **[ChatGPT Team / Business](https://shuita.xyz/c/gpt)** | [$25 / 席位 / 月](https://www.ai-toolbox.co/chatgpt-models/chatgpt-pricing)（年付 $20） | 约 ¥145 ~ ¥180 / 月 | **¥41.00 起**（正规席位） | 价格带 ¥41 ~ ¥144.2（10 家有货） | Standard 席位 Codex 额度同 Plus，Premium 席位（$125/月）为 5 倍且无 5 小时窗口限制 | 需要更高问答配额或团队工作区隔离、但预算低于 Pro 的用户 |
| **[Claude Pro](https://shuita.xyz/sku/claude_pro)**（直充 / 成品号） | [$20 / 月](https://claude.com/pricing)（年付 $17/月） | 约 ¥135 / 月（巴基斯坦区约 ¥119） | **¥131.86 ~ ¥134.00 起** | 均价 ¥156 / 中位价 ¥153.9（24 家有货） | 每 5 小时与每周额度为免费版 5 倍，支持 Claude Opus/Sonnet、Claude Code 与 Projects | 代码工程架构、长文本深度写作、Artifacts 原型构建 |
| **[Claude Max](https://shuita.xyz/sku/claude_pro)**（5X / 20X） | [$100 / 月](https://claude.com/pricing)（Ultra 为 $200/月） | 约 ¥720 ~ ¥1,440 / 月 | **¥759.22 起**（5X）/ **¥1,581.37 起**（20X） | 8 家有货（5X）/ 7 家有货（20X） | 5X 享 5 倍 Pro 额度并赠 $100 API 额度；Ultra 取消 5 小时限制并享 10 倍周额度 | 全天候使用 Claude Code 进行大型代码库重构的独立开发者 |
| **[Claude Team](https://shuita.xyz/sku/claude_pro)**（标准/高级席位） | [$25 / 席位 / 月](https://claude.com/pricing)（Premium $125/月） | 约 ¥180 ~ ¥900 / 月 | **¥1,240.00 起** | 2 家在售 | 支持高达 1M 上下文窗口、企业级权限控制及最高 $500/月共享 API 额度池 | 多人协作研发团队、对数据隐私默认不训练有合规要求的机构 |
| **[Gemini Pro](https://shuita.xyz/sku/gemini_pro)**（Google AI Pro） | $19.99 / 月 | 约 ¥144 / 月 | **¥4.00 起**（3 个月链接）/ **¥14.50 起**（18 个月成品号） | 均价 ¥36（14~18 家有货 / 55 家报价） | 含超大上下文窗口与 Google One 云端空间；低价货多为 Pixel / Jio 6~18 个月优惠渠道 | 超长文档/视频多模态解析、Google Workspace 重度办公用户 |
| **[Gemini Ultra](https://shuita.xyz/)** | 依地区与套餐定价 | 约 ¥200+ / 月 | **¥68.00 起**（个人）/ **¥197.93 起**（家庭席位） | 5 家有货（个人）/ 2 家有货（家庭） | Google 旗舰推理与多模态配额拉满，优先体验最新实验模型 | 需要高并发多模态创作与深度研究能力的专业用户 |
| **[SuperGrok / Grok Heavy](https://shuita.xyz/)** | $30 / 月起 | 约 ¥215 / 月 | **¥50.00 起**（Plus）/ **¥51.50 起**（SuperGrok）/ **¥560.00 起**（Heavy） | SuperGrok 29 家有货 / Heavy 14 家有货 | 实时接入 X（Twitter）全量信息流，SuperGrok 15x（¥336 起）与 Heavy 提供极高推理配额 | 实时舆情追踪、金融加密市场动态分析、无审查风格交互 |
| **[Cursor](https://cursor.com/pricing)**（X 订阅体系） | Plus $8 / Premium $30 / Super $100 / Ultra $200（[官方定价](https://www.aieatingtheworld.com/articles/cursor-pricing)） | 约 ¥58 ~ ¥1,440 / 月 | 实时比价见 **[水獭](https://shuita.xyz/)** | 覆盖独享成品与代充渠道 | 内置最新 Grok 编程模型与 Cloud Agents；调用 Claude、GPT 与 Gemini 模型按 API 列表价另计 | AI 辅助全栈开发、多文件自动补全与代码审查 |
| **[Midjourney](https://docs.midjourney.com/hc/en-us/articles/27870484040333-Comparing-Midjourney-Plans)**（Basic ~ Mega） | Basic $10 / Standard $30 / Pro $60 / Mega $120（[官方定价](https://docs.midjourney.com/hc/en-us/articles/27870484040333-Comparing-Midjourney-Plans)） | 约 ¥72 ~ ¥860 / 月 | 实时比价见 **[水獭](https://shuita.xyz/)** | 支持官方年付 8 折（$8~$96/月） | Basic 含 3.3 小时 Fast GPU；Standard 及以上享无限量 Relax 模式生图；Pro 解锁隐私模式（Stealth） | 视觉设计师、电商素材生成、游戏概念原画与 AI 视频创作 |

## 常见规格深度拆解：直充、成品号与拼车

在[水獭](https://shuita.xyz/c/gpt) ChatGPT 比价页与 [Claude Pro](https://shuita.xyz/sku/claude_pro) 比价页选购时，同一模型的不同交付形态差价可达数倍。下单前请先核对以下规格边界：

| 交付形态 | 运作机制与归属权 | 代表产品与价格区间 | 售后保障与潜在风险 |
| :--- | :--- | :--- | :--- |
| **月付直充 / 自助卡密（CDK）** | 会员直接开通在你自己的账号上，历史对话、自定义 GPTs/Projects 与设置完整保留 | [ChatGPT Plus](https://shuita.xyz/sku/gpt_plus_topup) 直充（¥104.96 ~ ¥210.89）、[Claude Pro](https://shuita.xyz/sku/claude_pro) iOS 卡密（¥134 ~ ¥189） | **最稳妥的长期方案**；优先选发 CDK 兑换码自助充值或明确标注“美区/菲区官方账单、质保 30 天”的店铺 |
| **独享成品号** | 商家预先注册并开通好订阅的现成账号，买断后直接拿到账号密码登录使用 | [ChatGPT Plus](https://shuita.xyz/c/gpt) 月付成品号（¥62 ~ ¥210）、[Gemini Pro](https://shuita.xyz/sku/gemini_pro) 18 个月成品号（¥14.5 ~ ¥42.23） | 省去注册与绑卡门槛；但原始邮箱归商家控制，务必确认是“质保 30 天订阅”还是“仅保首登” |
| **团队席位 / 轮换拼车** | 将你的账号拉入商家的 Business/Team 工作区，或多人在镜像站共享同一车位 | [ChatGPT Team](https://shuita.xyz/c/gpt) 席位（¥41 ~ ¥144.2）、[ChatGPT Plus](https://shuita.xyz/c/gpt) 拼车（¥50 起） | 工作区管理员拥有随时移出成员的权限；轮换车位按小时或天计费，不适合存放私密商业代码 |
| **短效号 / 临时体验号** | 有效期仅几小时至几天的临时会员账号 | [ChatGPT Plus](https://shuita.xyz/c/gpt) 短效号（¥19.89 ~ ¥98）、[ChatGPT Team](https://shuita.xyz/c/gpt) 短效号（¥3 起） | 据[水獭](https://shuita.xyz/c/gpt) 2026 年 10 月统计，超四成短效号仅保首次登录，掉会员不赔，仅适合临时应急 |

## 主流大模型 API 价格对比（按百万 Tokens 计费）

除包月会员外，开发者在接入 [Cursor](https://cursor.com/pricing)、[Claude Code](https://claude.com/pricing) 或自建 Agent 时常需对比 API 成本。需要注意的是，**ChatGPT Plus 与 Claude Pro 等个人订阅均不包含独立 API 调用额度**（[Claude Max](https://claude.com/pricing) 5X 赠送 $100/月 API 额度，Ultra 赠送 $200/月）：

| 模型与服务商 | 输入价格（缓存命中 / 1M Tokens） | 输入价格（缓存未命中 / 1M Tokens） | 输出价格（1M Tokens） | 上下文 / 最大输出 | 计费特色与并发限制 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[DeepSeek-V4.1-Flash](https://api-docs.deepseek.com/zh-cn/quick_start/pricing/)（`deepseek-flash`）** | 闲时 **¥0.02** / 忙时 **¥0.04** | 闲时 **¥1.00** / 忙时 **¥2.00** | 闲时 **¥4.00** / 忙时 **¥8.00** | 1M 上下文 / 384K 输出 | 并发上限 2,500；支持图像理解、思考模式与 Anthropic API 格式；闲时（北京时间周末及工作日非高峰）享 5 折 |
| **[DeepSeek-V4-Pro](https://api-docs.deepseek.com/zh-cn/quick_start/pricing/)（`deepseek-v4-pro`）** | 闲时 **¥0.15** / 忙时 **¥0.30** | 闲时 **¥4.50** / 忙时 **¥9.00**（[$1.32](https://api-docs.deepseek.com/quick_start/pricing/)） | 闲时 **¥13.50** / 忙时 **¥27.00**（[$1.98~$3.96](https://api-docs.deepseek.com/quick_start/pricing/)） | 1M 上下文 / 384K 输出 | 并发上限 500；旗舰推理与代码生成能力，支持 OpenAI 与 Anthropic 双格式直接接入 Claude Code |
| **[OpenAI API](https://openai.com/api/pricing/)（GPT 系列）** | 支持 Prompt Caching 折扣 | 按具体模型阶梯计费（详见[官方定价页](https://openai.com/api/pricing/)） | 按具体模型阶梯计费（Batch API 享异步折扣） | 依模型而定 | 另提供实时语音 [GPT-Live-1](https://openai.com/api/pricing/)（$0.05/分钟）与实时转写 [GPT-Live-Transcribe](https://openai.com/api/pricing/)（$0.017/分钟） |
| **[Claude API](https://claude.com/pricing)（Opus / Sonnet / Haiku）** | 支持 Prompt Caching | 按模型等级计费（可由 Max/Ultra/Team 赠送额度抵扣） | 按模型等级计费 | 最高 1M 上下文 | [Claude Team](https://claude.com/pricing) 计划最高可共享 $500/月 API 信用池，适合团队混合调用 |

## 在 Cursor / Claude Code 中接入实时比价 MCP

[水獭](https://mcpservers.org/servers/gm365/shuita-ai-price)开源了官方 MCP 服务 `ai-price-mcp`（源码仓库：[gm365/shuita-ai-price](https://github.com/gm365/shuita-ai-price)），无需配置 API Key，即可在 AI 编程助手中直接查询 70+ 款 AI 订阅的实时最低价、店铺手续费与 30 天价格趋势。

### 1. 一键安装 MCP Server

在 **Claude Code** 终端中运行：
```bash
claude mcp add ai-price -- npx -y ai-price-mcp
```

或在 **Cursor / Windsurf / Claude Desktop** 的 MCP 配置文件中加入：
```json
{
  "mcpServers": {
    "ai-price": {
      "command": "npx",
      "args": ["-y", "ai-price-mcp"]
    }
  }
}
```

### 2. 支持的自然语言查询指令
* `Claude Pro 现在最低多少钱？多少家店有货？`（调用 `get_lowest_price` 与 `get_offers`）
* `ChatGPT Plus 直充哪家店最便宜？含手续费到手价多少？`
* `最近 30 天 ChatGPT Plus 的价格是涨还是跌？`（调用 `get_price_trend`）

## AI 订阅常见问题与避坑指南（FAQ）

### Q1：哪个 AI 订阅性价比最高？日常办公和写代码怎么选？
* **综合主力首选**：如果你只订一个会员，[ChatGPT Plus](https://shuita.xyz/sku/gpt_plus_topup) 月付直充（水獭底价 ¥104.96 起）兼顾日常对话、联网搜索、画图与 Codex 编程，适用面最广。
* **重度代码开发**：首选 [Claude Pro](https://shuita.xyz/sku/claude_pro)（水獭底价 ¥131.86~¥134 起）配合 Claude Code；若每天高频重构大型项目且频繁触发 5 小时限额，可升级至 [Claude Max](https://shuita.xyz/sku/claude_pro) 5X（¥759.22 起）或搭配 [DeepSeek-V4-Pro](https://api-docs.deepseek.com/zh-cn/quick_start/pricing/) API 混合使用以大幅压降 Token 成本。
* **超低预算尝鲜**：[Gemini Pro](https://shuita.xyz/sku/gemini_pro) 优惠链接/成品号（¥4 ~ ¥25 起）提供了极低门槛的长文本处理方案，但需注意优惠渠道货的标称时长不等于质保时长。

### Q2：为什么卡网上的直充价格比美区官网 $20 更便宜？
官方在不同国家与地区的定价存在汇率差。根据[水獭](https://shuita.xyz/sku/claude_pro)官方原价对比数据，以 Claude Pro 为例，美区官网定价为 `$20/月`（约 ¥135），而巴基斯坦区 App Store 定价为 `PKR 4,900/月`（约 ¥119）、埃及区为 `EGP 999.99/月`（约 ¥126）、日本区为 `JPY 3,000/月`（约 ¥127）。同理，[ChatGPT Plus](https://shuita.xyz/sku/gpt_plus_topup) 直充大量正规卡商采用菲律宾区（菲区）官方卡付或 App Store 礼品卡批量采购，因此能在保留官方正规账单的前提下做到 `¥105` 左右的到手价。

### Q3：国内支付、代充与成品号有哪些风控风险？下单前如何避坑？
根据[水獭](https://shuita.xyz/c/gpt)防踩坑核对清单，下单前请重点核查三件事：
1. **优先保留账号控制权**：个人长期使用务必选择**直充**或**自助充值卡密（CDK）**，避免将主用邮箱密码直接交给人工代充客服。
2. **认准“质保订阅 30 天”而非“仅保首登”**：部分低价成品号或优惠链接标注“仅质保首登 / 质保 1 小时”，一旦后续因发卡方支付方式风控掉订阅或封号将无法获赔。
3. **算清支付通道手续费**：部分发卡网标价极低，但在结算页会加收 3%~8% 的通道手续费。[水獭](https://shuita.xyz/)比价看板已默认将人民币渠道手续费计入“到手价”，并单独标注更划算的 USDT 报价。

### Q4：个人版（Plus / Pro）与团队版（Team / Business）有什么本质区别？
* **官方团队版**：[ChatGPT Business](https://www.ai-toolbox.co/chatgpt-models/chatgpt-pricing)（原 Team，年付 $20/席位/月，2 席位起售）与 [Claude Team](https://claude.com/pricing)（年付 $20/席位/月）提供独立管理后台，且默认承诺不使用工作区数据训练模型。
* **卡网拆售席位风险**：卡网上单卖的 `¥41 ~ ¥144` Team 席位，本质是将你拉入商家的企业工作区。工作区管理员可随时移出成员，若商家母号违规被封，整个工作区席位会连带失效，购买前请务必确认店铺销量与满月质保条款。

## 贡献与价格纠错指引

本仓库与[水獭](https://shuita.xyz/)（shuita.xyz）共同维护开放、透明的 AI 订阅价格索引：
1. **价格变动与失效反馈**：如发现表格内某项官方定价调整或卡网渠道规则变更，欢迎直接提交 [GitHub Issue](https://github.com/gm365/shuita-ai-price) 或发起 Pull Request 更新对应条目。
2. **优质店铺提交收录**：如果你发现货源稳定、售后透明的独立小铺或发卡网，可前往[水獭](https://shuita.xyz/)的提交页提交入驻巡检。
3. **引用与署名规范**：欢迎开发者、博客作者与 AI 助手引用本仓库数据，引用请署名 **「[水獭](https://shuita.xyz/) shuita.xyz」** 并附带原文链接。
