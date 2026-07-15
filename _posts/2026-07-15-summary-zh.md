---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> 从 33 条内容中筛选出 8 条重要资讯。

---

1. [Stripe 与 Advent 出价 530 亿美元收购 PayPal](#item-1) ⭐️ 9.0/10
2. [睡眠规律性比时长更能预测死亡风险](#item-2) ⭐️ 8.0/10
3. [Claude 的 web\_fetch 工具被利用泄露用户隐私记忆](#item-3) ⭐️ 8.0/10
4. [Lobste.rs 从 MariaDB 迁移至 SQLite](#item-4) ⭐️ 8.0/10
5. [研究者感叹会议社区聚焦不再](#item-5) ⭐️ 8.0/10
6. [DeepSeek 年化收入逼近 5 亿美元，V4 API 毛利率超 50%](#item-6) ⭐️ 8.0/10
7. [谷歌与 Epic 撤回动议，第三方应用商店入驻 Play](#item-7) ⭐️ 8.0/10
8. [DeepSeek 首次融资，腾讯成最大外部股东](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe 与 Advent 出价 530 亿美元收购 PayPal](https://www.cnbc.com/2026/07/15/stripe-advent-offer-to-buy-paypal-for-more-than-53-billion-reuters.html) ⭐️ 9.0/10

支付公司 Stripe 与私募股权机构 Advent International 联合提出以每股 60.50 美元收购 PayPal，交易估值超过 530 亿美元，双方将各持一半股权。 这笔收购将重塑数字支付格局：Stripe 的现代基础设施结合 PayPal 庞大的用户基础，有望打造一个金融科技巨头，并引发行业重大变革。 该报价较 PayPal 周二收盘价溢价约 28%，收购方已获得约 500 亿美元的银行承诺融资。交易不会分拆 PayPal，目前讨论仍属保密，尚无定论。

telegram · zaihuapd · 7月15日 07:49

**背景**: Stripe 是一家以开发者友好 API 著称的领先在线支付处理平台，而 PayPal 是历史最悠久、规模最大的数字支付公司之一，拥有广泛的消费者和商家网络。Advent International 是一家专注于大规模收购的全球私募股权公司。此次合并将把 Stripe 的技术驱动方法与 PayPal 既有的用户基础和品牌认知结合起来。

**标签**: `#fintech`, `#acquisition`, `#payments`, `#Stripe`, `#PayPal`

---

<a id="item-2"></a>
## [睡眠规律性比时长更能预测死亡风险](https://academic.oup.com/sleep/article/47/1/zsad253/7280269) ⭐️ 8.0/10

2023 年发表在《睡眠》杂志上的一项研究发现，睡眠规律性（作息时间的一致性）比睡眠时长更能预测全因死亡风险。 这挑战了传统上只关注睡眠时长的观念，表明保持规律的作息时间可能对长寿更为关键。 该研究使用了超过 6 万名参与者的数据，并考虑了轮班工作和就业状态，但未将职业作为变量纳入，可能会引入混杂因素。

hackernews · bilsbie · 7月15日 11:46 · [社区讨论](https://news.ycombinator.com/item?id=48919363)

**背景**: 睡眠规律性指每日入睡和起床时间的一致性。以往研究多关注睡眠时长作为健康风险因素。这项研究表明，不规律的睡眠模式可能扰乱昼夜节律和代谢过程，导致不良健康后果。

**社区讨论**: 评论讨论混杂变量如生活方式和职业，有人认为规律性可能是整体生活稳定性的标志，而非直接因果因素。一位评论者分享通过补充镁改善睡眠的个人经验。

**标签**: `#sleep health`, `#mortality risk`, `#epidemiology`, `#health research`, `#sleep regularity`

---

<a id="item-3"></a>
## [Claude 的 web\_fetch 工具被利用泄露用户隐私记忆](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

安全研究员 Ayush Paul 发现 Claude 的 web\_fetch 工具中存在一个漏洞，可导致私密用户记忆数据泄露。Anthropic 已通过禁止 web\_fetch 跟随获取内容中的链接来修复此漏洞。 该漏洞证明了 Claude 数据泄露防护措施存在关键绕过风险，对数百万用户的隐私数据构成威胁。这凸显了结合私有数据访问与网络工具的 AI 智能体系统持续面临的安全挑战。 该漏洞使 web\_fetch 能访问已获取页面中嵌入的 URL，攻击者通过蜜罐站点利用一系列生成链接提取用户数据。攻击仅针对带有 &\#x27;Claude-User&\#x27; 用户代理的客户端，以避免被察觉。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的“致命三要素”攻击涉及将私有数据（如用户记忆）的访问能力与可遵循恶意指令的网络工具相结合。web\_fetch 工具原本设计为仅获取用户直接输入或来自配套 web\_search 工具的 URL。Claude 的记忆功能会保存过去对话中的信息，以个性化未来的交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted ...</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>
<li><a href="https://support.claude.com/en/articles/11817273-use-claude-s-chat-search-and-memory-to-build-on-previous-context">Use Claude ’s chat search and memory to build on previous context</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#Claude`, `#data-exfiltration`, `#vulnerability`

---

<a id="item-4"></a>
## [Lobste.rs 从 MariaDB 迁移至 SQLite](https://simonwillison.net/2026/Jul/14/lobsters-sqlite/#atom-everything) ⭐️ 8.0/10

Lobste.rs 本周末成功从 MariaDB 迁移到 SQLite，降低了 CPU 和内存使用量，并通过移除独立的 MariaDB VPS 将托管成本减半。 这一实际迁移案例表明，SQLite 可以作为中等流量 Rails 应用程序的生产数据库，可能简化许多类似社区网站的架构并降低成本。 该 Rails 应用现在运行在单个 VPS 上，主 SQLite 数据库大小为 3.8GB，另有独立的缓存数据库（1.1GB）、队列数据库（218MB）和 Rack::Attack 限流数据库（555MB）。迁移拉取请求在 30 个提交中新增了 735 行代码，删除了 593 行。

rss · Simon Willison · 7月14日 19:44

**背景**: Lobste.rs 是一个类似 Hacker News 的社区驱动链接聚合网站，基于 Ruby on Rails 构建。SQLite 是一种嵌入式 SQL 数据库引擎，传统上用于小型或单用户应用，但最近的改进使其适用于中等规模的 Web 工作负载。该网站自 2018 年起就计划进行数据库迁移，最初考虑 PostgreSQL，后来改为使用 SQLite。

**标签**: `#SQLite`, `#migration`, `#performance`, `#Rails`

---

<a id="item-5"></a>
## [研究者感叹会议社区聚焦不再](https://www.reddit.com/r/MachineLearning/comments/1uwy25k/does_anyone_else_miss_the_old_conference/) ⭐️ 8.0/10

一位研究者（Reddit 用户 Sep29493919）发帖反思 BMVC、ACCV、FG、ICIP、ICASSP 等小型专业会议的衰落，这些会议曾拥有强大的社区，如今优秀论文却被少数旗舰会议吸纳。 这种情绪揭示了机器学习生态中的系统性问题：随着投稿集中到少数顶级会议，评审质量、社区碎片化以及优秀论文的命运令人担忧。 帖子特别指出 FG 曾是面部分析的权威会议，ICASSP 是信号处理的阵地，并认为投稿数量激增、容纳能力有限以及评审不一致导致许多好论文变成非存档投稿或从未公开。

reddit · r/MachineLearning · /u/Sep29493919 · 7月15日 06:47

**背景**: 过去十年间，机器学习会议经历了爆炸式增长，NeurIPS、ICML 和 CVPR 等顶级会议吸引了绝大多数投稿。这种集中化边缘化了小型专题会议，减少了聚焦社区建设的机会，并增加了作者只投最高影响力会议的压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://publica.fraunhofer.de/entities/mainwork/04a8a70e-cd07-4e2d-aab6-392a193768b1">The 35th British Machine Vision Conference , BMVC 2024</a></li>
<li><a href="https://fg2024.ieee-biometrics.org/">The 18th IEEE International Conference on Automatic Face and Gesture Recognition – 27-31 May 2024 SDKM, ITU Campus, Istanbul, Turkey</a></li>

</ul>
</details>

**标签**: `#conferences`, `#research community`, `#ML ecosystem`, `#peer review`, `#academia`

---

<a id="item-6"></a>
## [DeepSeek 年化收入逼近 5 亿美元，V4 API 毛利率超 50%](https://www.theinformation.com/articles/deepseeks-annualized-revenue-nears-500-million-boosting-fundraise-ipo-plans) ⭐️ 8.0/10

DeepSeek 的年化收入已达到 4 亿至 5 亿美元，主要来自企业和开发者通过 API 调用模型，其 V4 API 毛利率超过 50%。该公司计划融资 500 亿元人民币，估值约 740 亿美元，引入中东等海外投资者。 这一快速收入增长和高毛利率表明，DeepSeek 有能力与 OpenAI、Anthropic 等主要 AI 提供商竞争，同时价格远低于对方。大规模融资和高倍数估值表明投资者信心强劲，可能重塑 AI 模型市场格局。 年化收入是按近期收入速度折算的，并非已实现的全年收入。V4 API 通过优化基础设施减少所需的芯片数量，从而降低成本。计划估值约 740 亿美元，约为年化收入上限的 148 倍。

telegram · zaihuapd · 7月15日 07:04

**背景**: DeepSeek 是一家中国人工智能公司，开发大语言模型并提供 API 服务。年化收入是基于当前月收入推算的年度数值，常被快速增长的公司用来展示发展势头。毛利率衡量的是扣除计算基础设施等直接成本后收入的留存比例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/">Your First API Call | DeepSeek API Docs</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#funding`, `#revenue`, `#API`

---

<a id="item-7"></a>
## [谷歌与 Epic 撤回动议，第三方应用商店入驻 Play](https://www.theverge.com/policy/965792/google-epic-withdraw-injunction-third-party-app-stores-coming-google-play) ⭐️ 8.0/10

谷歌与 Epic Games 共同撤回修改永久禁令的动议，迫使谷歌自 2024 年 7 月 22 日起在 Google Play 中托管竞争对手的第三方应用商店。 这是一次重大的反垄断转变，向竞争对手开放了 Google 的应用商店，可能改变移动应用分发格局，为开发者和用户带来更多选择。 除非开发者选择退出，谷歌将自动向第三方商店提供应用列表，且第三方商店需支付每年 5000 美元的费用并满足特定要求。在美国以外，谷歌计划通过侧载采用不同的“注册应用商店”方案。

telegram · zaihuapd · 7月15日 11:15

**背景**: Epic Games 诉谷歌反垄断案的裁决要求谷歌在其平台上托管第三方应用商店。Google Play 一直是安卓应用的主要分发渠道，这一变化挑战了其垄断地位。该裁决旨在增加竞争，减少谷歌对应用分发的控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.androidauthority.com/android-changes-third-party-app-stores-3613409/">Google &#x27;s proposed Android changes won&#x27;t save... - Android Authority</a></li>
<li><a href="https://www.justice.gov/atr/case/epic-games-inc-v-google-llc">Antitrust Division | Epic Games, Inc. v. Google LLC | United States Department of Justice</a></li>

</ul>
</details>

**标签**: `#Google Play`, `#Epic Games`, `#antitrust`, `#app store policy`, `#third-party app stores`

---

<a id="item-8"></a>
## [DeepSeek 首次融资，腾讯成最大外部股东](https://www.cls.cn/detail/2427193) ⭐️ 8.0/10

DeepSeek 完成了首轮融资，腾讯通过持股平台成为第一大外部股东，并计划于本月推出完整版 DeepSeek-V4 模型。公司还启动了大规模招聘，涵盖 Agent、代码智能体和底层算力框架等岗位。 此次融资显示出投资者对 DeepSeek 高性价比、开放权重 AI 模型的强烈信心，这些模型已挑战了美国在该领域的主导地位。腾讯、宁德时代等主要玩家的参与凸显了 AI 基础设施在中国的战略重要性。 腾讯通过杭州程砺间接持有超过 33%的股份（杭州程砺持有 DeepSeek 约 8.52%），宁德时代、网易、京东和 IDG 也持有股份。国家人工智能产业基金直接持股约 0.28%。DeepSeek-V4 预览版已在 Hugging Face 发布，参数量高达 1.6 万亿。

telegram · zaihuapd · 7月15日 12:56

**背景**: DeepSeek 是 2023 年由梁文峰创立的中国 AI 公司，最初由对冲基金幻方量化资助。该公司因以远低于美国竞争对手的成本开发高性能大语言模型而备受关注，并在出口限制下使用性能较弱的芯片。其 R1 和 V3 等开放权重模型因高效和性能而受到赞誉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://deepseek.com/en/index.html">DeepSeek</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#DeepSeek`, `#Tencent`, `#large language models`

---