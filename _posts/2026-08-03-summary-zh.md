---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 34 条内容中筛选出 13 条重要资讯。

---

1. [OpenAI 展示数学与理论计算机科学十项进展](#item-1) ⭐️ 9.0/10
2. [Qwen 发布 3.8-Max：2.4 万亿参数，首次开源 Max 级模型](#item-2) ⭐️ 9.0/10
3. [LLM 更青睐领域专长，拉大 AI 技能差距](#item-3) ⭐️ 8.0/10
4. [MiniMax H3 登陆 ComfyUI：开放权重、2K 视频与立体声音频](#item-4) ⭐️ 8.0/10
5. [数据库先驱 Andy Pavlo 加入 ClickHouse，成立 ClickHouse Labs](#item-5) ⭐️ 8.0/10
6. [Rust 项目目标：引入 \!Move 与 \!Forge 以取代 Pin](#item-6) ⭐️ 8.0/10
7. [SQLite CVE：真实漏洞还是 LLM 生成的垃圾内容？](#item-7) ⭐️ 8.0/10
8. [LLM 让开源的可检查性承诺更加切实可行](#item-8) ⭐️ 8.0/10
9. [Kimi K3 架构解析：压缩记忆、跨深度注意力与潜在路由](#item-9) ⭐️ 8.0/10
10. [审稿人呼吁：对缺少可复现代码的机器学习论文进行桌面拒稿](#item-10) ⭐️ 8.0/10
11. [美国 DNA 检测设备漏洞危及 30 年犯罪证据](#item-11) ⭐️ 8.0/10
12. [英伟达 CMP 170HX 矿卡被破解：解锁 80GB 显存、算力飙至 94 TFLOPS](#item-12) ⭐️ 8.0/10
13. [苹果就英国 iCloud 后门命令提起法律挑战](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 展示数学与理论计算机科学十项进展](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI 发布了一篇文章，展示了最近在数学和理论计算机科学领域的十项进展，体现了 AI 在数学推理和证明发现方面不断增强的能力。其中重点进展据称包括高维球堆积和多色 Ramsey 数方面的研究。 这标志着 AI 正成为数学研究的重要工具，可能加速发现过程并重塑证明的发现方式。它可能对数学家、计算机科学家以及更广泛的科学界产生深远影响。 根据社区评论，十项进展中有两项涉及高维球堆积和多色 Ramsey 数，这两者都是组合学和几何学中的经典难题。该文章可能强调了大型语言模型如何既能生成潜在解决方案，又能独立验证其有效性，这是自动定理证明领域的一大步。

hackernews · milkshakes · 8月3日 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49157930)

**背景**: 数学和理论计算机科学传统上依赖人类的直觉和细致的手动证明构建。近期大型语言模型的进展使 AI 能够探索猜想、生成候选证明，甚至验证结果，使得自动化变得越来越可行。球堆积问题研究的是如何在高维空间中排列相同球体以最大化密度，而 Ramsey 数则关注保证出现某种单色团所需的最小图规模。这些问题以难度著称，是检验 AI 数学推理能力的绝佳基准。

**社区讨论**: 评论者对 AI 在数学领域的指数级进展表示兴奋，有人认为任何可计算的问题最终都会被计算机解决，但也指出并非所有数学都会被自动攻克。还有人强调，当前模型无法凭直觉提出猜想，但可以通过蛮力快速否定一些猜想，并引用了道格拉斯·亚当斯（Douglas Adams）的典故。也有一些轻松的玩笑，比如 AI 能做高等数学却不会洗碗，同时有人分享了针对具体问题的可视化解释链接。

**标签**: `#AI`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#research`

---

<a id="item-2"></a>
## [Qwen 发布 3.8-Max：2.4 万亿参数，首次开源 Max 级模型](https://qwen.ai/blog?id=qwen3.8) ⭐️ 9.0/10

阿里巴巴通义千问团队发布了 Qwen 3.8-Max，总参数量达 2.4 万亿、活跃参数 95B，并宣布下周开源模型权重。这是 Qwen 首次开放 Max 级别模型的权重，该模型现已通过 QwenCloud 提供 API 服务。 开源 2.4 万亿参数的 Max 级模型是开放权重 AI 的重要里程碑，开发者有望以接近前沿的能力运行模型，同时无需支付按 token 计费的 API 费用。这也巩固了 Qwen 作为领先开源模型家族的地位，并加剧了与闭源前沿实验室的竞争。 Qwen 3.8-Max 基于 Qwen 3.5 架构，是迄今最强的 Qwen 模型，在编码、工作、研究和长周期任务上均有提升。在编码测试中，模型可自主运行超过 10 天完成项目构建与自我进化，并在 24 小时内的 WWW2025 多模态对话意图识别竞赛中击败了 526 支队伍中的 458 支。

telegram · zaihuapd · 8月3日 02:31

**背景**: Qwen 是阿里巴巴的开源权重大型语言模型系列，最初于 2023 年以“通义千问”之名推出，如今已成为全球下载量最大的开源模型家族之一。Qwen 3.8-Max 采用混合专家（MoE）架构，每个 token 只激活部分“专家”子模型，从而在保持推理算力可控的前提下实现巨大的总参数量。这正是该模型总参数达 2.4 万亿、而活跃参数仅为 95B 的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>
<li><a href="https://0xbenzo.dev/blog/understanding-model-parameters/">Understanding Model Parameters: Total Parameters vs Active ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Qwen`, `#Open Source`, `#Model Release`

---

<a id="item-3"></a>
## [LLM 更青睐领域专长，拉大 AI 技能差距](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 8.0/10

Sean Gedecke 的文章指出，大型语言模型（LLM）会不成比例地回报具有领域专长的用户，因为专家撰写的提示词隐式地包含了上下文和约束条件，从而产生更好的输出，并在 AI 辅助工作中造成日益扩大的技能差距。 这一观点很重要，因为它表明 LLM 会放大而非拉平现有的知识不平等，意味着经验丰富的专业人士从 AI 工具中获得的收益可能超过新手。这也将提示工程重新定义为一种由知识驱动的技能，而非纯粹的技术技能。 该论断基于一个观察：提示词不只是指令，还承载了隐含的任务上下文，这与提示工程和上下文学习（in-context learning）的概念一致。该文章在 Hacker News 上的讨论（206 分、83 条评论）反映出社区的高度关注和争论。

hackernews · MaxMussio · 8月3日 21:13 · [社区讨论](https://news.ycombinator.com/item?id=49161518)

**背景**: 提示工程（prompt engineering）是构建自然语言输入以从生成式 AI 模型获得预期输出的实践，包括少样本提示、思维链和角色分配等技术。上下文学习（in-context learning）是指大型语言模型在推理时通过提示中提供的示例或指令来适应新任务的能力。文章的核心观点将这两个概念联系起来：具有深厚领域知识的用户自然会写出更丰富的提示词，其中包含更有用的上下文，模型可利用这些内容给出更好的答案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_engineering">Prompt engineering</a></li>
<li><a href="https://arxiv.org/abs/2301.00234">[2301.00234] A Survey on In-context Learning</a></li>

</ul>
</details>

**社区讨论**: 评论者的观点不一。有些人同意明确表明专长会改变输出质量，并引用个人例子，如说明自己的圣经学背景或数十年 C 语言编程经验。一位持怀疑态度的评论者反驳说，即使是简单的‘认真思考’提示对 Anthropic 的数学家也有效；还有人将 LLM 比作‘放大镜’，能奖励那些将其视为自身思维延伸的用户。

**标签**: `#LLMs`, `#Prompting`, `#Expertise`, `#AI`, `#Software Engineering`

---

<a id="item-4"></a>
## [MiniMax H3 登陆 ComfyUI：开放权重、2K 视频与立体声音频](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI 宣布对 MiniMax H3 提供 Day-0 支持，这是一款开放权重的全模态模型，可生成最长 15 秒、带原生立体声音频的 2K 视频。本次发布还引入了一种剪枝技术，将模型内存占用降低 66%，使其能够在消费级 GPU 上本地运行。 这一进展将尖端的多模态视频生成能力带到个人创作者的本地硬件上，不再依赖纯云 API。开放权重与 ComfyUI 的集成有望加速社区在 AI 生成视频与音频工作流方面的创新。 该剪枝方法将约占模型总参数 40% 的调制权重替换为功能上等价的查找表。这使得总内存占用从全精度的 123.6 GB 降至 42.5 GB，再结合动态 VRAM 卸载，2K 视频模型可在 RTX 3060 上本地运行。

hackernews · vblanco · 8月3日 13:34 · [社区讨论](https://news.ycombinator.com/item?id=49155629)

**背景**: ComfyUI 是一个开源的节点式界面与推理引擎，用于生成式 AI，用户可以在本地构建自定义工作流。MiniMax H3 是中国公司 MiniMax 推出的开放权重通用全模态生成模型，能够联合理解文本、图像、视频和音频。神经网络剪枝是一种常见的模型压缩技术，通过移除冗余参数来减少内存占用并加速推理，通常质量损失很小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between ...</a></li>
<li><a href="https://docs.comfy.org/">ComfyUI Official Documentation - ComfyUI</a></li>
<li><a href="https://blog.paperspace.com/neural-network-pruning-explained/">Accelerating Inference: Neural Network Pruning Explained</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对生成质量印象深刻，一位用户报告称在 RTX 4070 Ti Super 上生成 10 秒 480p 视频需要 10 分钟，但结果“惊艳”。也有人质疑这种新剪枝技术的普适性，还有人认为生成的美学风格“乏味且雷同”。

**标签**: `#AI video generation`, `#ComfyUI`, `#MiniMax`, `#model compression`, `#open weights`

---

<a id="item-5"></a>
## [数据库先驱 Andy Pavlo 加入 ClickHouse，成立 ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

Andy Pavlo 已加入 ClickHouse，并创立 ClickHouse Labs，旨在将学术界数据库研究与产业界开发连接起来。 这对 ClickHouse 来说意义重大，因为它引入了一位数据库领域知名的学术界人物，有望加强其研究驱动的 OLAP 创新能力。这也体现了数据系统领域产学研合作的更广泛趋势。 公告本身并未披露 ClickHouse Labs 的具体技术细节或路线图。ClickHouse 是一个列式 SQL 数据库管理系统，用于联机分析处理，既有开源版本，也有云服务。

hackernews · nikolay\_sivko · 8月3日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49156011)

**背景**: ClickHouse 是一个开源的列式数据库管理系统，专为联机分析处理（OLAP）而设计，用户可以通过 SQL 查询实时生成分析报告。OLAP 是一种用于从不同角度分析业务数据的软件技术，通常对按列而非按行组织的大规模数据集进行查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ClickHouse">ClickHouse - Wikipedia</a></li>
<li><a href="https://clickhouse.com/docs/intro">What is ClickHouse? - ClickHouse Documentation</a></li>
<li><a href="https://aws.amazon.com/what-is/olap/">What is OLAP ? - Online Analytical Processing Explained - AWS</a></li>

</ul>
</details>

**社区讨论**: 社区讨论整体情绪积极：评论者祝贺 Andy Pavlo，并称赞 ClickHouse 吸引人才的能力，同时也希望他能推动 ClickHouse 资助学术界数据库研究。还有人好奇这次合作将如何影响未来的 OLAP 产品、数据摄入和索引。

**标签**: `#ClickHouse`, `#databases`, `#OLAP`, `#research`, `#industry-academia`

---

<a id="item-6"></a>
## [Rust 项目目标：引入 \!Move 与 \!Forge 以取代 Pin](https://github.com/rust-lang/rust-project-goals/blob/main/src/2026/move-trait.md) ⭐️ 8.0/10

Rust 的 2026 项目目标提出了两项新语言特性：不可移动类型（\!Move）与保证析构（\!Forge）。该提案认为这两者有望最终取代现有的 Pin 机制，将“不可移动”变为类型自身的属性。 这些特性有望解决 Rust 在处理自引用和异步类型时的长期缺陷，简化 unsafe 代码，并为安全的 scoped spawn 铺路。如果被采纳，将显著提升 Rust 的易用性和正确性保证，影响大量库与应用。 该提案目前只是项目目标，尚未成为正式语言变更，设计仍可能调整甚至被放弃。草案还顺带提到 \!Destruct / 线性类型等相邻可能性，并将能力建模为正向 trait：只有实现了 Move 的类型才能被移动。

hackernews · paavohtl · 8月3日 06:42 · [社区讨论](https://news.ycombinator.com/item?id=49152023)

**背景**: Rust 的 Pin 类型最初是为了支持自引用异步 future 等不可移动值而引入的，但因其将约束放在指针/位置而非类型上，常被视为一种“hack”。新提案反其道而行：类型系统直接标记某些类型为 \!Move，并用 \!Forge 保证析构函数即使经过 mem::forget 也会执行。这一目标是 Rust 2026 项目路线图的一部分，社区中还出现了 withoutboats 提出的 “pinned places” 替代方案，引发讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/rust-lang/rust-project-goals/blob/main/src/2026/move-trait.md">rust-project-goals/src/2026/move-trait.md at main · rust-lang/rust-project-goals</a></li>
<li><a href="https://lobste.rs/s/sp2wji/rust_project_goals_immobile_types">Rust Project Goals: Immobile types and guaranteed destructors | Lobsters</a></li>
<li><a href="https://cornfordandcross.com/art/technical-analysis-skills/rust-project-goals-immobile-types-and-guaranteed-destructors/">Rust Project Goals: Immobile Types And Guaranteed Destructors - Cornford and Cross</a></li>

</ul>
</details>

**社区讨论**: 评论者大多表示欢迎，认为不可移动类型自约 2016 年以来就是 Rust 缺失的重要拼图，Pin 只是权宜之计。也有人询问这是否意味着维护者会选择该设计而非 pinned places 替代方案；还有人补充了线性类型（\!Destruct）等相邻想法。整体态度积极但保持谨慎，因为目前只是项目目标而非正式变更。

**标签**: `#Rust`, `#language design`, `#memory safety`, `#Pin`, `#type system`

---

<a id="item-7"></a>
## [SQLite CVE：真实漏洞还是 LLM 生成的垃圾内容？](https://research.jfrog.com/post/sqlite-critical-cves-or-llm-slops/) ⭐️ 8.0/10

JFrog 的安全研究人员正在审查最近上报的 SQLite CVE 报告，以判断它们是真实漏洞还是由 LLM 生成的低质量“垃圾内容”。该分析凸显了 AI 生成的漏洞报告所带来的可信度与安全风险。 如果 LLM 生成的垃圾内容淹没漏洞数据库，信噪比将下降，使得甄别真实 CVE 变得更加困难。这凸显了在安全关键工作流中 AI 可靠性的更广泛担忧。 这项调查聚焦于最近的 SQLite CVE 条目是否由 LLM 生成，而非通过正当的安全研究发现的。它强调了未经核实的 AI 生成内容进入关键安全数据库的危险。

hackernews · ymir\_e · 8月3日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49154332)

**背景**: CVE（通用漏洞与披露）是一个公开的字典，用于识别和编目已知的网络安全漏洞，每个漏洞都有唯一编号；美国 NVD 会进一步丰富这些条目。“LLM slop”（LLM 垃圾内容）指的是大型语言模型生成的大量低质量文本，往往看似合理但实际上不准确。当这类内容被当作 CVE 报告提交时，可能污染安全数据库并引发误报。随着 LLM 输出在网络上传播，“slop”一词逐渐流行开来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/National_Vulnerability_Database">National Vulnerability Database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为 LLM 生成的 CVE 报告是一个日益严重的问题，他们指出信噪比降低使真正漏洞更难被发现。一些人强调恶意行为者可能利用大量虚假报告淹没系统，还有人指出必须修补所有 CVE 的机构将承担额外负担。也有人提到 LLM 确实能发现真实漏洞，使问题变得更加复杂。

**标签**: `#security`, `#LLM`, `#SQLite`, `#CVE`, `#AI reliability`

---

<a id="item-8"></a>
## [LLM 让开源的可检查性承诺更加切实可行](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 8.0/10

西蒙·威利森认为，LLM 降低了阅读、编译和修改陌生开源代码的摩擦，使开源在可检查和可修改方面的原始梦想更容易实现。他描述了自己如何利用 Claude 和 Codex 等工具以极小成本克隆并构建项目。 这可能促使开发者真正去阅读和修改源码，增强开源理念的实际意义。它也展示了一种有前景的 AI 辅助编程工作流，未来可能成为主流。 威利森提到，他经常让 Claude「从 GitHub 克隆 x/y，并告诉我 Z 是如何工作的」，并把让软件编译通过当作交给 Codex 或 Claude Code 的零成本挑战。他承认自己尚未养成修改软件的习惯，但已看到一条一年前不存在的路径。

rss · Simon Willison · 8月3日 15:30

**背景**: 开源软件赋予用户检查和修改代码的自由，但在实践中，阅读和编译陌生代码库往往需要大量时间投入。Claude 和 Codex 等 LLM 能够处理仓库克隆、构建和代码解释，消除了这一关键障碍。这让开源最初的理想对普通开发者而言更加具有实际可行性。

**标签**: `#open source`, `#LLMs`, `#developer tools`, `#software engineering`

---

<a id="item-9"></a>
## [Kimi K3 架构解析：压缩记忆、跨深度注意力与潜在路由](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

SemiAnalysis 发布了对 Kimi K3 架构的深度技术分析。Kimi K3 是一个拥有 2.8T 参数、支持 100 万 token 上下文窗口的模型；该分析探讨了其关键创新：基于 Gated DeltaNet 的压缩记忆、跨深度注意力以及潜在专家路由，并评估了它们对推理性能的影响。 该分析提供了对前沿大模型内部设计的罕见的独立解读，帮助研究人员和从业者理解 Kimi K3 如何实现强大性能与高效推理。随着模型架构成为竞争焦点，这些技术可能影响下一代大规模 AI 系统的设计方向。 Kimi K3 基于 Kimi Delta Attention 和 Attention Residuals 构建，并具备原生视觉能力。其压缩记忆采用 Gated DeltaNet，这是一种类 RNN 的方法，只计算预测纠正而不重写整个记忆，但硬件高效实现仍是一个未解决的挑战；潜在专家路由将 token 投影到更低维度，以降低路由和专家权重的字节开销。

rss · Semianalysis · 8月3日 19:42

**背景**: 像 Kimi K3 这样的大语言模型通常依赖混合专家（MoE）架构，在保持每 token 计算量大致固定的同时扩展参数量，但在全隐藏维度上进行专家路由代价高昂。标准的注意力机制随着上下文长度增长也会变得内存开销巨大，因此业界开始研究压缩记忆和跨层注意力机制。Gated DeltaNet 属于线性注意力/类 RNN 记忆的一类方法，通过高效更新状态来降低开销。SemiAnalysis 的这篇分析将 Kimi K3 的技术选择置于这些研究背景中进行解读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://portfolio.hagzag.com/blog/2026-07-25-kimi-k3-architecture-inference-economics/">Kimi K 3 : When Model Architecture Becomes a Platform... | Portfolio</a></li>
<li><a href="https://www.emergentmind.com/papers/2603.15619">Mixture-of- Depths Attention in LLMs</a></li>

</ul>
</details>

**标签**: `#Kimi K3`, `#LLM architecture`, `#inference`, `#latent expert routing`, `#compressed memory`

---

<a id="item-10"></a>
## [审稿人呼吁：对缺少可复现代码的机器学习论文进行桌面拒稿](https://www.reddit.com/r/MachineLearning/comments/1vei12v/its_time_to_desk_reject_papers_that_dont_include/) ⭐️ 8.0/10

一位审稿人报告称，今年在主要会议上评审的 12 篇机器学习论文中，只有 1 篇提供了完整的可复现代码，而在提供任何代码的 5 篇论文中，有 3 篇因包含错误而导致结果失效。作者建议，会议应对未提供能复现结果代码的论文进行桌面拒稿。 这凸显了机器学习研究中的可复现性问题，即论文常常缺少代码或包含隐藏错误。如果采用这种政策，对无代码论文进行桌面拒稿可能迫使作者分享可运行代码，但在激励机制未改进的情况下也可能增加审稿负担。 该审稿人今年为包括 NeurIPS 在内的 3 个主要会议审稿，发现 12 篇论文中只有 1 篇提供了从输入数据到输出 AUROC 的完整训练流程代码。他认为当前激励机制对代码公开不利，因为审稿人可能发现错误，而隐藏代码几乎没有成本。

reddit · r/MachineLearning · /u/Flaky-Ambition5900 · 8月3日 16:17

**背景**: NeurIPS 是机器学习和神经信息处理领域的顶级年度会议，被接收的论文常影响整个领域的发展方向。桌面拒稿是指编辑在同行评审之前就拒绝稿件，通常用于明显不符合要求或存在质量问题的稿件。AUROC 是二分类任务中常用的性能指标，衡量受试者工作特征曲线下的面积。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Neural_Information_Processing_Systems">Conference on Neural Information Processing Systems</a></li>
<li><a href="https://peerreviewai.org/guides/desk-rejection-prevention">How to Avoid Desk Rejection | PeerReviewAI</a></li>
<li><a href="https://glassboxmedicine.com/2019/02/23/measuring-performance-auc-auroc/">Measuring Performance: AUC ( AUROC ) – Glass Box Medicine</a></li>

</ul>
</details>

**标签**: `#reproducibility`, `#machine learning`, `#peer review`, `#research practices`, `#NeurIPS`

---

<a id="item-11"></a>
## [美国 DNA 检测设备漏洞危及 30 年犯罪证据](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

研究人员发现，美国多数犯罪实验室使用的 Thermo Fisher Scientific DNA 分析设备存在安全漏洞，攻击者可篡改自 1995 年以来的 DNA 证据文件而不被发现。厂商已于上周五发布高危安全公告，并推出带数字签名的软件更新。 由于 DNA 证据是刑事定罪的重要依据，这一漏洞可让约 30 年的案件卷宗中的 DNA 数据被无声篡改，可能影响在审及已结案件的司法公信力。同时，它也暴露出法医实验室缺乏统一网络安全监管的问题。 测试中，研究人员借助 Anthropic 的 Claude AI 生成漏洞利用代码，约 45 分钟即可篡改 DNA 扫描文件，且不会触发常用分析软件的警报。Thermo Fisher 表示尚未发现有漏洞被实际利用，并正与美国网络安全和基础设施安全局（CISA）合作。

telegram · zaihuapd · 8月3日 05:15

**背景**: 美国多数犯罪实验室使用毛细管电泳（CE）仪器来分离和识别 DNA 片段，而法医 DNA 分型通常依赖短串联重复序列（STR）分析。这些仪器输出的是电泳图谱（electropherogram），即通过荧光强度与 DNA 片段大小的关系图来呈现 DNA 图谱，用于身份鉴定。该漏洞影响这些仪器生成的原始数据文件，一旦访问控制被绕过，这些文件可被无声篡改。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/STR_analysis">STR analysis - Wikipedia</a></li>
<li><a href="https://nij.ojp.gov/topics/articles/what-str-analysis">What Is STR Analysis? | National Institute of Justice</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electropherogram">Electropherogram</a></li>

</ul>
</details>

**标签**: `#security`, `#forensics`, `#DNA analysis`, `#vulnerability`, `#cybercrime`

---

<a id="item-12"></a>
## [英伟达 CMP 170HX 矿卡被破解：解锁 80GB 显存、算力飙至 94 TFLOPS](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

亚利桑那州立大学研究人员公开了一种通过 Falcon 安全协处理器栈溢出漏洞破解英伟达 CMP 170HX 矿卡的方法。该漏洞利用绕过了 OTP 熔丝锁定，将显存扩展至最高 80GB，FP32 算力从 0.39 TFLOPS 飙升至 94 TFLOPS。 此次破解让廉价的矿卡变身强大的 AI 计算设备，以远低于同级数据中心 GPU 的成本实现大模型推理和图像生成的普及。同时，它也暴露了英伟达 Falcon 子系统的硬件安全漏洞，对 GPU 供应链和二手市场产生深远影响。 CMP 170HX 采用与 A100 相同的 GA100 核心，但通过一次性可编程\(OTP\)熔丝限制算力、显存和 PCIe。研究人员利用 Falcon 安全处理器中无界 DMA 溢出漏洞劫持权限并修改寄存器；社区测试表明，解锁卡可在 Windows 和 Linux 下运行 AI 工作负载，但长期稳定性及不同批次的解锁上限仍不确定。

telegram · zaihuapd · 8月3日 11:29

**背景**: 英伟达 CMP 170HX 于 2021 年推出，是一款专为以太坊挖矿设计的显卡，基于 GA100 GPU 但大幅限制了算力、显存和 I/O，以防止其用于数据中心。OTP 熔丝是物理的一次性可编程元件，用于永久设定硬件限制；绕过它们通常需要侵入性硬件修改或固件漏洞利用。Falcon 是内置于英伟达 GPU 中的定制微控制器系列，负责安全和管理任务，因此成为此类攻击的主要目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://knightli.com/en/2026/07/22/cmp-170hx-80gb-memory-unlock-ai-gpu-buying-risk/">Is the CMP 170HX 80GB Memory Unlock Reliable? AI Mining GPU Buying Risks and Checklist</a></li>
<li><a href="https://download.nvidia.com/open-gpu-doc/Falcon-Security/1/Falcon-Security.html">NVIDIA Falcon Security</a></li>
<li><a href="https://electronics.alibaba.com/question/nvidia-cmp-170hx-mining-gpu-explained">What Is the NVIDIA CMP 170HX? Mining-Only GPU Guide</a></li>

</ul>
</details>

**社区讨论**: 国内超频与 AI 社区已跟进验证，称解锁卡可在 Windows 和 Linux 下运行 AI 图像生成及大语言模型推理。但讨论中也提醒长期稳定性和不同批次解锁上限的差异；二手市场报价已从 300–500 元涨至 3000–4000 元，海外卖家甚至叫价约 1500 美元。

**标签**: `#GPU`, `#hardware-security`, `#exploit`, `#AI-inference`, `#NVIDIA`

---

<a id="item-13"></a>
## [苹果就英国 iCloud 后门命令提起法律挑战](https://www.ft.com/content/2cc9c96a-0e5b-4c33-a95a-3d11072a145c?syn-25a6b1a6=1) ⭐️ 8.0/10

苹果已向英国调查权力法庭提起法律挑战，针对一项要求开放加密 iCloud 云备份后门的技术能力通知（TCN）。这延续了苹果与英国政府之间持续的加密争端。 此案可能为政府强制要求加密后门树立关键先例，影响数百万用户的隐私与安全。它凸显了科技公司加密实践与国家安全需求之间日益紧张的矛盾，并对全球科技法律和数字权利具有潜在影响。 在英国政府发出仅针对英国用户的新 TCN 后，苹果于 2025 年 2 月在英国下架了 iCloud 高级数据保护功能，此前覆盖英美用户的初始要求已被撤回。隐私组织 Privacy International 和 Liberty 也提起了申诉，案件管理听证会定于下月举行。

telegram · zaihuapd · 8月3日 15:40

**背景**: 技术能力通知（TCN）是依据英国 2016 年《调查权力法案》第 253 条发出的，要求电信或技术运营商保持协助拦截令及其他合法访问的能力。iCloud 高级数据保护是苹果可选的最强端到端加密功能，可保护包括备份在内的大部分 iCloud 数据，使苹果和第三方无法访问；若不开启，苹果持有加密密钥，理论上可访问数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.legislation.gov.uk/ukpga/2016/25/section/253">Investigatory Powers Act 2016 - Legislation.gov.uk</a></li>
<li><a href="https://en.wikipedia.org/wiki/ICloud">iCloud - Wikipedia</a></li>
<li><a href="https://support.apple.com/en-us/108756">How to turn on Advanced Data Protection for iCloud - Apple Support</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Privacy`, `#Encryption`, `#UK Law`, `#Security`

---