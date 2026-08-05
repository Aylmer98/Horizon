---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 31 条内容中筛选出 13 条重要资讯。

---

1. [谷歌 DeepMind 高管变动：哈萨比斯任董事长，杰夫·迪恩离职](#item-1) ⭐️ 10.0/10
2. [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](#item-2) ⭐️ 9.0/10
3. [杰夫·迪恩创办 Discovery Loop，推动科学实验自动化](#item-3) ⭐️ 8.0/10
4. [Castform Neon 以百倍低成本在检索任务上击败 GPT-5.6 Sol](#item-4) ⭐️ 8.0/10
5. [Meta 广告中出现 AI 生成的儿童性虐待图像](#item-5) ⭐️ 8.0/10
6. [Cloudflare OS：面向智能体、应用与工作的开放平台](#item-6) ⭐️ 8.0/10
7. [Claude Fable 5 将旧推文变成可玩的《浣熊大劫案》游戏](#item-7) ⭐️ 8.0/10
8. [LLM 0.32 新增推理轨迹、服务端工具与更智能日志](#item-8) ⭐️ 8.0/10
9. [Monodratic：为稀疏因果注意力引入学习式乘积哈希路由](#item-9) ⭐️ 8.0/10
10. [马斯克宣布 SpaceX 将独家采用英伟达 AI 架构](#item-10) ⭐️ 8.0/10
11. [DeepSeek 重启第二轮融资 投前估值 5000 亿元](#item-11) ⭐️ 8.0/10
12. [字节 SeedRealtime 原生全双工模型上线豆包 App](#item-12) ⭐️ 8.0/10
13. [FFmpeg 9.0 发布：新增动画 WebP、Vulkan 滤镜与 Claude 辅助开发](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌 DeepMind 高管变动：哈萨比斯任董事长，杰夫·迪恩离职](https://blog.google/company-news/inside-google/message-ceo/next-chapter-ai-momentum/) ⭐️ 10.0/10

2026 年 8 月 5 日，谷歌 DeepMind 宣布领导层变动：德米斯·哈萨比斯将从 CEO 转任董事长，杰夫·迪恩和桑杰·格玛沃特将离开谷歌，创办一家独立的公共利益公司。 此次重组标志着谷歌 AI 领导层一个时代的结束，并可能预示着顶尖研究人员流失的“人才外流”。它可能重塑谷歌的 AI 发展轨迹，并加剧 AI 行业的竞争。 杰夫·迪恩已在谷歌任职 27 年，并在 Alphabet 担任高级技术领导职务；桑杰·格玛沃特是谷歌高级研究员。两人将共同创办一家独立的公共利益公司，以加速机器学习、科学和工程领域的发现。

hackernews · colesantiago · 8月5日 16:05 · [社区讨论](https://news.ycombinator.com/item?id=49184755)

**背景**: 公共利益公司（PBC）是一种由州法律承认的营利性法律实体，必须追求特定的公共利益，并在决策时考虑对所有利益相关者（而不仅仅是股东）的影响。PBC 融合了传统营利性公司和非营利组织的特点，使企业能够在创造回报的同时应对社会或环境挑战。谷歌 DeepMind 一直是 AI 研究的核心参与者，而杰夫·迪恩等基础工程师的离开意义重大，因为他们对谷歌的基础设施和机器学习系统做出了长期贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Benefit_corporation">Benefit corporation - Wikipedia</a></li>
<li><a href="https://uslawexplained.com/public_benefit_corporation">Public Benefit Corporation (PBC): The Ultimate Guide</a></li>
<li><a href="https://www.britannica.com/money/what-is-a-public-benefit-corporation">Public Benefit Corporations (PBCs): Meaning, Examples ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映出对谷歌人才流失的深切担忧：评论者强调杰夫和桑杰的离开是真正的损失，有人列出近期众多知名 AI 研究人员的离职，并指出没有相应的高调引进。还有人称这是“黄金时代”的终结，并调侃杰夫·迪恩的离开导致股价下跌，显示出市场反应。

**标签**: `#Google DeepMind`, `#AI Leadership`, `#Jeff Dean`, `#Demis Hassabis`, `#Tech Industry News`

---

<a id="item-2"></a>
## [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

名为 ChainDrop 的自我传播蠕虫已攻陷 npm 上逾 1,300 个包，包括 Keyv、Cacheable 等热门缓存库，合计月下载量达 20 亿次。攻击始于 Keyv 维护者 GitHub 账号被攻破，并通过正常的 GitHub Actions 流程发布恶意版本，波及 Deliveroo、Qlik、ServiceTitan 等机构相关包。 这是迄今规模最大的 npm 供应链攻击之一，威胁无数下游项目的软件供应链。安装过受影响版本的开发者必须将环境视为已被攻破，轮换所有凭证并审计日志，因此这是一起迫切需要应对的生态级安全事件。 恶意包内含 setup.mjs 投放器和 Math\_Symbol.js 窃密脚本，会在 npm install 时自动运行，窃取 GitHub、npm、AWS、Kubernetes 等凭证。多家安全厂商报告的数字不一，少则 4 小时内 444 个包被投毒，多则 868 个包、1,381 个版本受影响；npm-cache\[.\]com 域名可作为失陷指标（IoC）。

telegram · zaihuapd · 8月5日 03:04

**背景**: npm 是 Node.js 的默认包管理器，热门包中的恶意代码会自动传播到所有安装它的项目。近年来供应链攻击日益增多，Shai-Hulud 蠕虫家族此前在 2025 年 9 月就曾攻陷超 500 个 npm 包；ChainDrop 似乎是这一波攻击中的新变种。更多细节可参阅 BleepingComputer 文章及多家安全厂商的分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/">Massive ChainDrop npm supply-chain attack infects hundreds of packages</a></li>
<li><a href="https://www.stepsecurity.io/blog/chaindrop-npm-worm">ChainDrop npm Worm: Bun-loaded CI/CD credential harvester with Ethereum dead-drop C2 - StepSecurity</a></li>
<li><a href="https://socket.dev/blog/popular-npm-packages-in-the-keyv-and-cacheable-namespaces-compromised-in-active-supply-chain">Popular npm Packages in the keyv and Cacheable Namespaces ...</a></li>

</ul>
</details>

**标签**: `#Security`, `#Supply Chain Attack`, `#npm`, `#Malware`, `#Credential Theft`

---

<a id="item-3"></a>
## [杰夫·迪恩创办 Discovery Loop，推动科学实验自动化](https://www.discoveryloop.com/) ⭐️ 8.0/10

由包括杰夫·迪恩在内的前 Google AI 负责人创办的初创公司 Discovery Loop 已启动，目标是在科学和工程领域实现实验循环的自动化，首先从 ML 研究与工程入手。Google 是其创始投资方和云合作伙伴，Khosla Ventures 和 Radical Ventures 也参与了投资。 这标志着一次备受关注的尝试：不仅要自动化机器学习编码，还要自动化整个研究-实验循环，从而可能加速芯片设计、生物学、药物发现和材料设计等领域的探索。这也表明顶尖 AI 研究者认为自主实验是 AI 领域下一个重要范式。 据杰夫·迪恩介绍，这种方法面向美国国家工程院（NAE）十四大工程挑战问题中几乎所有重要子问题，但初期重点是 ML 研究与工程。融资金额和估值尚未披露，Discovery Loop 计划将自己的平台作为第一个客户。

hackernews · xtreak29 · 8月5日 16:19 · [社区讨论](https://news.ycombinator.com/item?id=49184960)

**背景**: 自动化科学发现是一种通过迭代循环和智能体方法自主生成、测试并完善科学知识的计算框架。Karpathy 的开源项目 AutoResearch 使自主实验循环的概念广为人知，而 Discovery Loop 似乎是该概念在机构化、大规模协作层面上的延伸，强调 AI 智能体之间的异步协作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/jeff-dean-google-discovery-loop-startup/">Google’s Top AI Brains Are Leaving to Launch Discovery Loop | WIRED</a></li>
<li><a href="https://aiwiki.ai/wiki/discovery_loop">Discovery Loop | AI Wiki</a></li>
<li><a href="https://www.emergentmind.com/topics/automated-scientific-discovery">Automated Scientific Discovery</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Discovery Loop 与 Karpathy 的 AutoResearch 高度相似，称其为机构化、类似 SETI@home 的规模化协作版本。也有人开玩笑说，Google 是在给资深工程师提供“养老院”以免他们被竞争对手挖走；还有人质疑，在需要真实物理载体和劳动的实验中，自动化实验循环究竟如何实现。

**标签**: `#AI research`, `#Machine learning`, `#Automation`, `#Research infrastructure`, `#Experimental loop`

---

<a id="item-4"></a>
## [Castform Neon 以百倍低成本在检索任务上击败 GPT-5.6 Sol](https://neon.com/blog/how-castform-neon-beats-frontier-models-on-price-and-efficiency) ⭐️ 8.0/10

Neon 的一篇博客文章展示了其专用系统 Castform Neon 在检索任务上击败了 OpenAI 的 GPT-5.6 Sol，而成本大约只有后者的百分之一。这一结果突出表明，在特定工作负载上，专用开源模型可以胜过通用前沿模型。 这挑战了“前沿模型越大越好”的假设，表明可组合的任务专用 LLM 能以极低的成本获得更好的结果。这可能推动更多团队构建专用检索栈，而不是依赖单个庞大的通用模型。 该对比聚焦于检索增强生成（RAG）类任务，在这类任务中，成本和延迟与准确性同等重要。Castform Neon 似乎是故意组合开放权重组件和路由，而不是单一规模的模型，这篇博客文章标题为《Castform Neon 如何在价格和效率上击败前沿模型》。

hackernews · moonikakiss · 8月5日 18:18 · [社区讨论](https://news.ycombinator.com/item?id=49186762)

**背景**: 检索增强生成（RAG）是一种让 LLM 在生成答案前先从外部文档中检索相关文本的技术，有助于减少幻觉并利用最新信息。开放权重模型会公开发布最终权重，任何人都可以下载、研究并针对特定任务进行微调。前沿模型是训练于海量数据的最先进、最昂贵的通用 AI 系统，但在狭窄任务上并不总是最高效的选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**社区讨论**: 评论者对专用模型的想法反应积极，多人指出用于检索、重排序等任务的专用 LLM 很有意义，还有人将其比作“使用正确的数据结构”。少数人提出疑问：这类检索在更大规模文档集上表现如何；一位实测者证实，小型模型在文档事实检索上可以胜过更大的同门模型，他认为大型模型可能对简单查找“想得太多”。

**标签**: `#LLM`, `#retrieval`, `#open-source`, `#efficiency`, `#specialized models`

---

<a id="item-5"></a>
## [Meta 广告中出现 AI 生成的儿童性虐待图像](https://www.wired.com/story/meta-ran-ads-that-contained-ai-generated-child-sexual-abuse-imagery/) ⭐️ 8.0/10

据报道，Meta 投放了包含 AI 生成的儿童性虐待图像的广告。这一事件凸显了 Meta 内容审核系统的系统性缺陷。 这引发了关于平台责任以及当前 AI 内容审核局限性的紧迫问题，尤其是在生成式工具使此类图像的制作更加容易和廉价的背景下。这影响到 Meta 数十亿用户、广告商以及期望平台阻止非法内容传播的儿童安全倡导者。 报道指出，PhotoDNA 等为已知儿童性虐待材料创建感知哈希的现有工具，可能难以应对新生成的 AI 材料。社区反馈还提到 Meta 各平台响应时间缓慢且政策执行不一致。

hackernews · malshe · 8月5日 19:47 · [社区讨论](https://news.ycombinator.com/item?id=49187977)

**背景**: PhotoDNA 是微软与达特茅斯学院于 2009 年开发的感知哈希技术，旨在帮助查找和删除已知的儿童剥削图像。随着生成式 AI 的发展，检测 AI 生成的儿童性虐待材料已成为调查人员的优先事项，因为这些图像可能无法匹配现有的哈希数据库，并可能以新方式描绘受害者。Wired 关于 Meta 广告的报道表明，当前检测能力与通过广告系统流动的 AI 生成虐待图像规模之间存在差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PhotoDNA">PhotoDNA</a></li>
<li><a href="https://www.microsoft.com/en-us/photodna">PhotoDNA | Microsoft</a></li>
<li><a href="https://www.cameraforensics.com/blog/2025/12/23/detecting-ai-csam--a-vital-investigative-capability/">Detecting AI CSAM – a vital investigative capability | CameraForensics</a></li>

</ul>
</details>

**社区讨论**: 评论者对平台审核表示不满，有人提到 YouTube 上也有类似问题，还有人指出 Meta 未能阻止暗示对政客施暴的广告。多人认为罚款被视为经商成本，而有人质疑算法审核是否比传统编辑监督更好。

**标签**: `#AI safety`, `#content moderation`, `#Meta`, `#child safety`, `#ethics`

---

<a id="item-6"></a>
## [Cloudflare OS：面向智能体、应用与工作的开放平台](https://blog.cloudflare.com/cloudflare-os/) ⭐️ 8.0/10

Cloudflare 发布了 Cloudflare OS——一个基于 Cloudflare Workers 构建的开源智能体工作空间，允许企业创建文档、构建应用并在组织上下文中运行智能体。该平台现已在 GitHub 的 cloudflare/cloudflare-os 仓库中开源。 这一公告表明大型基础设施厂商正进入以智能体为中心的平台领域，可能重塑企业构建和部署内部 AI 工具的方式。通过以 AI 原生方式重拾 Sandstorm 愿景，Cloudflare OS 也可能影响行业中新出现的“智能体操作系统”趋势。 根据社区分析，该平台是开源的，并且直接使用 pi-agent，而非 Cloudflare 自家的 Agents SDK、Think 或 Flue 框架。一些评论者质疑“OS”品牌命名，并担心采用 Cloudflare 生态会带来供应商锁定问题。

hackernews · speckx · 8月5日 13:58 · [社区讨论](https://news.ycombinator.com/item?id=49182996)

**背景**: Cloudflare 是美国主要的互联网基础设施公司，以 CDN 服务、安全防护、通过 Workers 提供的边缘计算以及日益增多的 AI 服务而闻名。Cloudflare OS 延续了 Sandstorm 的愿景，Sandstorm 是 Kenton Varda 约十年前创建的开源自托管 Web 应用平台，如今在 Workers 之上重建并深度集成 AI。这里的“工作操作系统”并非传统操作系统，而是指智能体和应用在共享工作空间中运行并能访问组织知识的平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-os/">Cloudflare OS: an open platform for agents, apps, and work</a></li>
<li><a href="https://github.com/cloudflare/cloudflare-os">GitHub - cloudflare/cloudflare-os: Agent workspace built on ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cloudflare,_Inc.">Cloudflare, Inc.</a></li>

</ul>
</details>

**社区讨论**: 整体情绪是审慎关注与怀疑并存。评论者赞赏 Kenton Varda 的解读，询问为何使用 pi-agent 而非 Cloudflare 自研的智能体框架，并对命名和供应商锁定提出担忧。也有人认为“OS”不过是流行语。

**标签**: `#cloudflare`, `#agents`, `#platforms`, `#ai`, `#open-source`

---

<a id="item-7"></a>
## [Claude Fable 5 将旧推文变成可玩的《浣熊大劫案》游戏](https://simonwillison.net/2026/Aug/5/raccoon-heist/#atom-everything) ⭐️ 8.0/10

西蒙·威利森（Simon Willison）使用 Claude Code for web 中的 Claude Fable 5，仅凭一条含截图的提示，便从他在 2022 年发的推文构建出一款完整可玩的《浣熊大劫案》游戏。该游戏已部署到 GitHub Pages 并可以在线游玩。 这展示了 AI 编程助手的快速进步：单个提示现在就能生成完整可玩的游戏，大大降低了软件开发的门槛。同时，它也展现了新的 Claude Code for web 工作流——模型在 Anthropic 托管的云端基础设施上自主迭代项目。 威利森借助 GitHub Pages 来解决 Claude Code for web 无法实时预览的问题，让 Claude 先提交一个 index.html。原始推文包含 GPT-3 的文本生成和 DALL-E 的概念图；新游戏沿用了“浣熊抢劫”主题，代码已开源在 GitHub 上。

rss · Simon Willison · 8月5日 19:42

**背景**: Claude Fable 5 是 Anthropic 功能最强大的通用模型，专为长时间、异步的任务（如自主编程）而设计。Claude Code on the web 是一个研究预览功能，用户可把编程任务交给 Claude 处理，任务在 Anthropic 托管的云端基础设施上运行，且会话在浏览器或应用间持续保存。《浣熊大劫案》源于 2022 年一次用 GPT-3 和 DALL-E 进行的实验：用户让模型描述并绘制一款关于一群偷窃浣熊的游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://code.claude.com/docs/en/claude-code-on-the-web">Use Claude Code on the web - Claude Code Docs</a></li>
<li><a href="https://claude.com/blog/claude-code-on-the-web">Claude Code on the web | Claude by Anthropic</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#Claude`, `#game development`, `#AI agents`, `#software engineering`

---

<a id="item-8"></a>
## [LLM 0.32 新增推理轨迹、服务端工具与更智能日志](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

西蒙·威利森发布了 LLM 0.32，这是该项目自推出以来最重要的更新。新版本增加了可见的推理轨迹、服务端提供方工具、重新设计的内容可寻址 SQLite 日志，并支持 OpenAI Responses API 和新的 GPT-5.6 模型。 此次更新通过在 stderr 上展示模型的思维链，让开发者更容易使用推理模型，并通过代码执行、网页搜索等服务端工具扩展了 LLM 的能力。重新设计的日志和 OpenAI Responses API 支持，使 LLM 成为 AI 生态中更强大且更具前瞻性的命令行工具。 推理轨迹默认显示到标准错误输出，并可通过 -R/--hide-reasoning 隐藏。新增的服务端工具包括 OpenAI 的 CodeInterpreter 和 WebSearch；llm-anthropic 插件增加了 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP 支持；新的 &\#x27;llm openai endpoint&\#x27; 命令可对任何兼容 OpenAI 的端点执行一次性提示，且不记录日志。

rss · Simon Willison · 8月4日 23:58

**背景**: LLM 是西蒙·威利森开发的一款命令行工具，可对多种大语言模型运行提示。推理轨迹是模型在回答之前生成的内部思维链步骤，展示这些步骤有助于用户理解模型行为。OpenAI 于 2025 年 3 月发布的 Responses API 将聊天补全和工具调用统一到一个接口中。重新设计的 SQLite 日志采用内容可寻址存储，即根据内容的哈希值存储数据，从而支持去重和高效缓存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/reference/overview">API Overview | OpenAI API Reference</a></li>
<li><a href="https://www.emergentmind.com/topics/reasoning-traces">Reasoning Traces : Analysis &amp; Applications</a></li>
<li><a href="https://grokipedia.com/page/OpenAI_Responses_API">OpenAI Responses API</a></li>

</ul>
</details>

**标签**: `#LLM`, `#OpenAI`, `#CLI`, `#developer-tools`, `#AI`

---

<a id="item-9"></a>
## [Monodratic：为稀疏因果注意力引入学习式乘积哈希路由](https://www.reddit.com/r/MachineLearning/comments/1vg3jda/monodratic_learned_producthash_routing_for_sparse/) ⭐️ 8.0/10

一位独立研究者发布了 Monodratic，这是一种稀疏因果注意力架构，利用学习式乘积哈希路由来选择固定数量的远程源块。在合成联想回忆测试中，仅选择两个远程块就达到了 99.35% 的平均准确率，代码和验证报告已在 GitHub 上公开。 这项工作为在不牺牲准确率的前提下降低注意力的计算成本提供了一种实用方法，而这正是长上下文语言模型面临的核心挑战。其出色的实证结果和无状态设计可能会影响未来机器学习社区中的稀疏注意力和路由研究。 学习式路由在 768 次联想回忆查询中正确回答了 763 次，而同等宽度的未训练路由为 425/768，纯局部注意力仅为 151/768。稀疏选择集注意力与独立的稠密选择掩码基准的最大绝对误差为 1.43e-6；打包式 CPU 路由在 4,096 到 32,768 个 token 上的拟合时间指数为 0.993；所有学习式路由和扩展运行均报告零发布溢出。

reddit · r/MachineLearning · /u/dttdrv · 8月5日 10:28

**背景**: 稀疏注意力旨在通过只计算一部分 token 之间的交互来降低标准注意力的二次方开销。常见方法包括固定模式（如局部窗口）、学习式路由（如 Routing Transformers）以及基于哈希的稀疏化（如 Reformer 的局部敏感哈希）。Monodratic 是一种无状态注意力混合器，它将 RoPE 后的查询和键几何结构映射到有界的因果发布列表中，选择固定数量的源块，并对这些选中的 token 执行精确的 softmax。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Misul-Computing/Monodratic">GitHub - Misul-Computing/Monodratic: Learned product - hash routing ...</a></li>
<li><a href="https://www.academia.edu/170001736/Monodratic_proof_report_Misul_Computing_Monodratic_A_Sparse_Attention_Architecture_with_Learned_Product_Hash_Routing_Misul_Computing">(PDF) Monodratic proof report Misul Computing Monodratic: A Sparse ...</a></li>

</ul>
</details>

**标签**: `#sparse attention`, `#machine learning`, `#architecture`, `#efficiency`, `#routing`

---

<a id="item-10"></a>
## [马斯克宣布 SpaceX 将独家采用英伟达 AI 架构](https://wccftech.com/elon-musk-commits-spacex-exclusively-to-nvidia-gpus-citing-theyre-the-best/) ⭐️ 8.0/10

8 月 4 日，在 SpaceX 首次财报电话会上，马斯克宣布 SpaceX 的 AI 服务将独家基于英伟达系统运行，并称 Vera Rubin 架构是“最佳 AI 计算架构”。公司计划在全球地面数据中心和太空部署英伟达 Vera Rubin NVL72 机架，目标是在今年年底前实现超过 2 吉瓦的 AI 计算能力，到 2027 年底前接近 10 吉瓦。 此次合作巩固了英伟达在 AI 基础设施领域的主导地位，并验证了其机架级架构在地面及轨道数据中心的适用性。同时，这推动了 SpaceX 的 Starmind 计划，即建设轨道 AI 数据中心，未来可能将 AI 算力转移到太空，减少地球上的能源和水资源消耗。 Vera Rubin NVL72 机架集成了 36 颗 Vera CPU 和 72 颗 Rubin GPU，单个机架可提供高达 3.6 exaFLOPS 的 NVFP4 推理性能和 75 TB 的快速内存。SpaceX 的 Starmind 卫星预计将于明年开始发射，利用英伟达的太空级模块，通过高带宽激光链路构建轨道 AI 数据中心网络。

telegram · zaihuapd · 8月5日 02:04

**背景**: 英伟达的 Vera Rubin 平台是一套机架级 AI 系统，将整个数据中心视为一个统一的计算单元，集成了 Rubin GPU、Vera CPU、NVLink 6 等六款协同设计的芯片。作为 Blackwell 的继任者，Rubin 提供高达 50 稀疏 petaflops 的 FP4 性能，而 Rubin Ultra 将翻倍。SpaceX 的 Starmind 项目计划部署多达一百万个 AI 卫星，在轨道上运行计算任务，由太阳能供电，并通过激光链路与地球连接，有望降低 AI 的用水和用电需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/rubin/">Infrastructure for Scalable AI Reasoning | NVIDIA Vera Rubin Platform</a></li>
<li><a href="https://servers.asus.com/glossary/What-is-NVIDIA-Vera-Rubin-NVL72">What is NVIDIA Vera Rubin NVL72? | ASUS Servers</a></li>
<li><a href="https://techstartups.com/2026/08/04/nvidia-partners-with-spacex-to-build-starmind-ai-orbital-data-centers-in-space/">Nvidia partners with SpaceX to build Starmind AI orbital data ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#SpaceX`, `#AI infrastructure`, `#Satellite computing`

---

<a id="item-11"></a>
## [DeepSeek 重启第二轮融资 投前估值 5000 亿元](https://finance.sina.com.cn/wm/2026-08-05/doc-inimfmyv1554159.shtml) ⭐️ 8.0/10

DeepSeek 已重启第二轮融资，计划募资 500 亿元，投前估值约 5000 亿元，预计 8 月下旬完成签约。本轮融资曾在 7 月底暂停，现已重启；若顺利完成，两轮合计募资将超 1000 亿元。 这是 AI 领域头部公司 DeepSeek 的重大融资事件，估值较首轮提升约 43%，反映出资本市场对 AI 的高热度以及行业竞争格局的变化，对行业具有重要影响。 本轮融资据称至少在 7 月中旬就已开启，但因创始人梁文锋对网上流传的疑似泄露的“投资者会议实录”言论不满而在 7 月底暂停。部分此前积极接触的机构表示尚未接到重启消息，通道仍处于暂缓状态。

telegram · zaihuapd · 8月5日 02:46

**背景**: DeepSeek 是一家 AI 公司，今年 4 月开启首轮融资，6 月完成交割，金额为 500 亿元、估值超 3500 亿元。本轮投前估值约 5000 亿元，较首轮提升约 43%。融资的暂停与低调重启，反映出在高关注度的 AI 融资交易中，内部因素也可能影响交易执行。

**标签**: `#AI`, `#融资`, `#DeepSeek`, `#科技投资`, `#人工智能`

---

<a id="item-12"></a>
## [字节 SeedRealtime 原生全双工模型上线豆包 App](https://seed.bytedance.com/zh/blog/seedrealtime-%E9%9F%B3%E8%A7%86%E9%A2%91%E5%85%A8%E5%8F%8C%E5%B7%A5%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%8F%91%E5%B8%83-%E8%B5%B0%E5%90%91%E5%85%A8%E6%A8%A1%E6%80%81%E8%87%AA%E7%84%B6%E4%BA%A4%E4%BA%92) ⭐️ 8.0/10

2026 年 8 月 5 日，字节跳动发布原生音视频全双工大模型 SeedRealtime，并已在豆包 App 全量上线。该模型以统一架构融合音频、视频与文本，支持边看、边听、边说的实时端到端交互。 其意义在于将实时语音/视频 AI 从 ASR-VLM-TTS 级联管线转向端到端模型，显著降低延迟和信息损耗，并将“话未说完被抢断”等对话节奏问题减少一半。该进展可能推动消费级应用中的自然人机交互，并为全双工多模态助手树立新标杆。 字节端到端人工评测显示，SeedRealtime 的对话节奏问题较级联模型减少一半，且无需外部 VAD 模块判断说话轮次。它属于原生音视频全双工大模型，可联合理解音频、视觉与时间信息。

telegram · zaihuapd · 8月5日 04:42

**背景**: 传统实时语音助手依赖级联模块：ASR 把语音转成文字，VLM 或 LLM 生成回复，TTS 再朗读出来。这条管线会引入延迟、丢失语气和视觉信息，而且通常需要独立的 VAD 来判断说话轮次。全双工模型则在同一神经网络内同时完成听与说，OpenAI 的 GPT-Live 和 NVIDIA 的 PersonaPlex 等近期发布也体现了这一趋势。字节跳动 Seed 团队成立于 2023 年，研究领域包括大语言模型、语音、视觉与下一代 AI 交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seed.bytedance.com/en/models">Seed Models - seed.bytedance.com</a></li>
<li><a href="https://technode.com/2026/08/05/bytedance-launches-seedrealtime-full-duplex-audio-video-model/">ByteDance launches SeedRealtime full-duplex audio-video model</a></li>
<li><a href="https://www.technology.org/2026/07/09/openai-gpt-live-full-duplex-voice-models/">OpenAI Launches GPT-Live Voice AI Models - Technology Org</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#Multimodal`, `#Real-time Interaction`, `#ByteDance`, `#SeedRealtime`

---

<a id="item-13"></a>
## [FFmpeg 9.0 发布：新增动画 WebP、Vulkan 滤镜与 Claude 辅助开发](https://news.ycombinator.com/item?id=49166202) ⭐️ 8.0/10

FFmpeg 9.0 正式发布，新增动画 WebP 解码器与分离器、v360\_vulkan 滤镜、Playdate 视频编码器及封装器、DAB+ 用的 HE-AAC 960 解码、transpose\_cuda 滤镜、AMF 帧率转换器滤镜，以及 ONNX Runtime DNN 后端。开发团队还通过 Anthropic 的 Claude for Open Source Program 帮助查找缺失的向后移植。 这是 FFmpeg 的一次重要版本发布，带来了多项期待已久的功能，包括 DAB+ 解码和 GPU 加速的 360 度视频转换。同时，这次发布也是 AI 辅助开源维护的一次值得关注的尝试，可能会影响其他项目将 AI 工具集成到工作流中的方式。 在新增功能中，v360\_vulkan 滤镜支持等距柱状投影和立方体贴图（包括 3x2、6x1、1x6 布局），并通过 Vulkan 计算着色器实现。动画 WebP 解码器/分离器和 Playdate 编码器扩展了 FFmpeg 对细分格式的支持，而 ONNX Runtime 后端为运行基于机器学习的 DNN 滤镜提供了新途径。

telegram · zaihuapd · 8月5日 10:32

**背景**: FFmpeg 是一个广泛使用的开源多媒体框架，能够对大量音视频格式进行解码、编码、转码和滤镜处理。v360 系列滤镜用于处理 360 度视频转换，而 DAB+ 数字广播使用 960 采样帧大小的 HE-AAC，这一格式此前在 FFmpeg 中不受支持。Playdate 是一款带有独特曲柄输入的手持游戏机，其视频格式主要由社区逆向工程实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.ffmpeg.org/FFmpeg/FFmpeg/pulls/22725">#22725 - lavfi/v360: add a Vulkan-compute based filter ...</a></li>
<li><a href="https://trac.ffmpeg.org/ticket/1407">#1407 ( HE - AAC (v2): 960 /120 MDCT window is not implemented)...</a></li>
<li><a href="https://github.com/hteumeuleu/playorama">A cranky video player for the Playdate - GitHub</a></li>

</ul>
</details>

**社区讨论**: 一些社区成员对 AI 辅助开发的安全审查流程表达了担忧，因为 Claude 被用于帮助识别缺失的向后移植。总体情绪似乎是谨慎乐观的——认为 AI 可以作为维护者的工具，但也呼吁对 AI 建议的更改进行仔细的人工审查。

**标签**: `#ffmpeg`, `#multimedia`, `#release`, `#ai-assisted-development`, `#open-source`

---