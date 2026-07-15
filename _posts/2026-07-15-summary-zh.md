---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> 从 32 条内容中筛选出 7 条重要资讯。

---

1. [Stripe 与 Advent 出价 530 亿美元收购 PayPal](#item-1) ⭐️ 10.0/10
2. [马斯克：X 将无条件开源全部代码并接受第三方审查](#item-2) ⭐️ 9.0/10
3. [Claude web\_fetch 漏洞导致数据泄露](#item-3) ⭐️ 8.0/10
4. [通过 Hadamard 积分解卷积神经元](#item-4) ⭐️ 8.0/10
5. [DeepSeek 收入接近 5 亿美元，V4 API 毛利率超 50%](#item-5) ⭐️ 8.0/10
6. [Google 与 Epic 撤回动议，第三方商店将入驻 Play](#item-6) ⭐️ 8.0/10
7. [DeepSeek 完成首轮融资，腾讯成第一大外部股东](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe 与 Advent 出价 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 10.0/10

据消息人士透露，支付公司 Stripe 与私募股权机构 Advent International 联合出价超过 530 亿美元收购 PayPal。若成功，这将合并两个最大的在线支付平台。 这笔潜在合并将造就在线支付领域的绝对巨头，引发严重的反垄断担忧，并可能削弱金融科技行业的竞争。这可能导致商户费用上升和消费者选择减少。 报价将 PayPal 估值超过 530 亿美元，合并后的实体将拥有 PayPal、Venmo、Braintree 和 Xoom 以及 Stripe。然而，由于在非面对面交易中的市场集中度，该交易面临巨大的监管障碍。

hackernews · rvz · 7月15日 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: Stripe 是领先的在线支付处理商，深受初创企业和数字业务欢迎；PayPal 则是面向消费者和商家的成熟支付平台。合并将结合 Stripe 对开发者友好的基础设施与 PayPal 庞大的用户群和银行牌照，可能开启新的金融服务。

**社区讨论**: 评论者普遍反对这笔交易，担心竞争减少和费用上升。有人指出，Stripe 对某些行业（如大麻、成人内容）的严格限制会损害目前依赖 PayPal 更宽松政策的商家。其他人则提出反垄断担忧，认为合并后的实体将主导在线结账领域。

**标签**: `#fintech`, `#acquisitions`, `#payments`, `#antitrust`

---

<a id="item-2"></a>
## [马斯克：X 将无条件开源全部代码并接受第三方审查](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 9.0/10

马斯克在 X 上宣布，在完成安全漏洞审查后，X 平台将无条件开源全部代码，并邀请第三方审查者验证正在运行的代码与开源代码一致。 此举旨在为社交媒体平台建立前所未有的透明度，可能为信任和责任确立新标准。如果实施，将允许独立验证 X 的算法和安全实践，影响整个科技行业。 马斯克明确表示开源是无条件的，涵盖整个代码库，第三方审计员将检查正在运行的系统是否与开源代码一致。但尚未提供实施细节和时间表。

telegram · zaihuapd · 7月15日 13:32

**背景**: 开源代码是指将源代码公开，任何人都可以查看、使用和修改。第三方代码审计是由独立专家审查软件的安全漏洞，并验证编译后的二进制文件是否与源代码一致，通常依赖于可复现构建（reproducible builds）——一种确保相同源代码总是生成相同二进制文件的做法。这些措施通过防止隐藏后门或被篡改的代码来建立信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducible_builds">Reproducible builds</a></li>
<li><a href="https://sslinsights.com/code-integrity/">Code Integrity : Definition, Purpose, Benefits &amp; Best Practices</a></li>
<li><a href="https://anadea.info/blog/what-is-code-audit/">What is Code Audit : All Your Questions Answered + CASE STUDIES</a></li>

</ul>
</details>

**标签**: `#open source`, `#social media`, `#transparency`, `#Elon Musk`, `#X`

---

<a id="item-3"></a>
## [Claude web\_fetch 漏洞导致数据泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Ayush Paul 发现，Claude 的 web\_fetch 工具可被诱骗通过跟随恶意站点的嵌套链接泄露用户记忆，从而绕过 Anthropic 的 URL 来源限制。 该漏洞凸显了 LLM 代理安全中的关键缺陷，表明即使是精心设计的机制也可能被绕过，并强调了在 AI 系统中防止数据泄露的持续挑战。 攻击利用蜜罐页面提示 Claude 按字母顺序浏览 URL，以窃取用户姓名、城市和雇主信息；Anthropic 内部已发现此问题，并通过阻止 web\_fetch 跟随获取内容中的链接进行了修复。

rss · Simon Willison · 7月15日 14:21

**背景**: Claude 的 web\_fetch 工具设计为仅获取用户明确提供或 web\_search 工具返回的 URL，以防止通过隐藏指令进行数据泄露。然而，该工具还会跟随获取页面中嵌入的链接，从而产生漏洞。这是“致命三重奏”攻击的一个例子，即 LLM 能够访问私有数据、不受信任的内容并具备泄露能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#LLM security`, `#prompt injection`, `#data exfiltration`

---

<a id="item-4"></a>
## [通过 Hadamard 积分解卷积神经元](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

一位研究人员提出了一种方法，利用感受野与权重的 Hadamard 积来分析 Inceptionv1 中的 1x1 卷积神经元，发现了单语义簇（如汽车、猫、狗），并揭示了像字母这样的低值概念中，其依赖神经元的正负权重均匀分布，从而压低总和。 这项工作为卷积神经网络的机械可解释性提供了一种新技术，揭示了网络如何表示和压制低值概念。它可能激发对卷积层理解的进一步研究，并通过提高模型透明度促进更安全的 AI。 该分析聚焦于 Inceptionv1 中的 1x1 卷积神经元，利用其感受野与权重矩阵的 Hadamard 积来识别模式。该方法在高激活概念上产生了清晰单语义簇，而低激活簇（如字母）的下游神经元正负权重均匀分布，表明梯度下降有意进行了压制。

reddit · r/MachineLearning · /u/narang\_27 · 7月15日 06:59

**背景**: 机械可解释性旨在通过分析神经网络内部结构和电路来逆向工程其工作原理。Hadamard 积是一种逐元素乘法操作，用于 GRU、注意力机制等神经网络架构。单语义性是指神经元或特征对单个可解释概念做出响应，这是可解释性研究中的一个关键目标，旨在超越多语义神经元。本文将这些思想应用于卷积网络，而该领域相比 Transformer 探索较少。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://arxiv.org/html/2504.13112v1">Hadamard product in deep learning: Introduction, Advances and Challenges</a></li>
<li><a href="https://medium.com/data-science/take-a-look-under-the-hood-24e40281c900">Take a Look Under the Hood. Using Monosemanticity to... | Medium</a></li>

</ul>
</details>

**标签**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#Inceptionv1`, `#monosemanticity`

---

<a id="item-5"></a>
## [DeepSeek 收入接近 5 亿美元，V4 API 毛利率超 50%](https://www.theinformation.com/articles/deepseeks-annualized-revenue-nears-500-million-boosting-fundraise-ipo-plans) ⭐️ 8.0/10

DeepSeek 的年化收入已达 4 亿至 5 亿美元，主要来自企业和开发者通过 API 调用模型，其 V4 API 毛利率超过 50%。公司还计划募资 500 亿元人民币，估值约 5000 亿元人民币（合 740 亿美元）。 这一里程碑表明 DeepSeek 的商用进展和盈利能力，尽管其定价远低于 OpenAI 和 Anthropic 等竞争对手，但仍实现了盈利，显示出投资者对 AI 行业的强烈信心。高估值倍数（年化收入的 148 倍）反映了市场对持续增长的预期。 年化收入是根据近期收入速度折算的，并非已实现的全年收入。DeepSeek 通过优化基础设施，减少了运行每个模型所需的芯片数量，从而实现了 V4 API 超过 50% 的毛利率。这轮募资瞄准中东等海外投资者，并允许使用美元投资。

telegram · zaihuapd · 7月15日 07:04

**背景**: DeepSeek 是一家中国 AI 公司，开发大型语言模型并提供 API 服务。其 V4 API 兼容 OpenAI 和 Anthropic 的格式，并于 2026 年 4 月 23 日上线。毛利率是指扣除 API 服务直接成本（如硬件和能源成本）后剩余收入所占的百分比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/">Your First API Call | DeepSeek API Docs</a></li>
<li><a href="https://apidog.com/blog/how-to-use-deepseek-v4-api/">How to Use the DeepSeek V 4 API ?</a></li>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek AI: R1 Reasoning, API &amp; Local Deployment 2026</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#Revenue`, `#Fundraising`, `#Gross Margin`

---

<a id="item-6"></a>
## [Google 与 Epic 撤回动议，第三方商店将入驻 Play](https://www.theverge.com/policy/965792/google-epic-withdraw-injunction-third-party-app-stores-coming-google-play) ⭐️ 8.0/10

Google 与 Epic Games 已共同撤回修改永久禁令的动议，导致 Google 自 2026 年 7 月 22 日起允许第三方应用商店入驻 Google Play。 这标志着 Android 应用分发生态的重大转变，可能增加竞争，为开发者和用户提供更多选择，同时影响 Google 对其平台的控制。 Google 将通知美国开发者，其应用将自动提供给第三方商店，除非选择退出。第三方商店需每年支付 5,000 美元的安全审查费，并满足不得在美国以外分发、有明确的信任与安全政策等要求。

telegram · zaihuapd · 7月15日 11:15

**背景**: Android 上的侧载（sideloading）允许用户不使用官方 Google Play 商店安装应用，但 Google 一直在加强控制。新的“Registered App Stores”计划是一种灵活的侧载方式，为安装达到一定质量基准的应用商店引入了 UI。这一法律和解源于 Epic 针对 Google Play 商店政策的反垄断诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sideloading">Sideloading - Wikipedia</a></li>
<li><a href="https://www.androidauthority.com/google-epic-changes-registered-app-stores-3646743/">Android&#x27;s getting a flexible new approach to sideloading with Registered App Stores</a></li>

</ul>
</details>

**标签**: `#反垄断`, `#Google Play`, `#Epic Games`, `#应用商店`, `#数字市场`

---

<a id="item-7"></a>
## [DeepSeek 完成首轮融资，腾讯成第一大外部股东](https://www.cls.cn/detail/2427193) ⭐️ 8.0/10

DeepSeek 完成了首轮外部融资，腾讯通过持股平台成为其第一大外部股东。该公司还计划于本月中旬推出完整版 DeepSeek-V4 模型，并已启动大规模招聘。 本轮融资标志着 DeepSeek 的重要里程碑，吸引了中国主要科技和投资公司的支持，这将加速其大语言模型（包括即将推出的 V4）的开发和部署。同时，这也表明了 AI 模型领域日益激烈的竞争。 腾讯间接持有杭州程砺（持有 DeepSeek 约 8.52%股份）超过 33%的份额，从而成为第一大外部股东。其他投资者包括宁德时代、网易、京东、IDG、Monolith 等。DeepSeek 正在招聘 Agent、代码智能体和底层算力框架等岗位。

telegram · zaihuapd · 7月15日 12:56

**背景**: DeepSeek 是一家专注于大语言模型开发的中国 AI 公司。据报道，DeepSeek-V4 模型是一个 1 万亿参数的混合专家（MoE）模型，支持 100 万 token 的上下文窗口，专为高效的编码和推理任务设计。本轮融资还包括国家人工智能产业投资基金，显示出政府的支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek AI: R1 Reasoning, API &amp; Local Deployment 2026</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/ DeepSeek - V 4 -Pro · Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#DeepSeek`, `#Tencent`, `#large language models`

---