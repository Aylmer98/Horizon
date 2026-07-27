---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 31 条内容中筛选出 10 条重要资讯。

---

1. [月之暗面发布 Kimi K3：全球首个开源 2.8 万亿参数模型](#item-1) ⭐️ 9.0/10
2. [Fastjson2 曝远程代码执行漏洞，所有版本受影响，尚无补丁](#item-2) ⭐️ 9.0/10
3. [vLLM v0.26.0 发布，引入 Inkling 模型系列与 DeepSeek-V4 优化](#item-3) ⭐️ 8.0/10
4. [Anthropic 澄清开放权重模型立场](#item-4) ⭐️ 8.0/10
5. [论坛软件从 React 迁移到 HTMX](#item-5) ⭐️ 8.0/10
6. [用借用的协议重构电子邮件架构](#item-6) ⭐️ 8.0/10
7. [独立评估发现 6 个前沿 LLM 均左倾，包括 Grok](#item-7) ⭐️ 8.0/10
8. [华为被指筹建月产 14 万片晶圆的 DRAM 工厂](#item-8) ⭐️ 8.0/10
9. [谷歌透露 Gemini 4 为迄今最雄心预训练，预计年底发布](#item-9) ⭐️ 8.0/10
10. [中国开始量产国产 DUV 光刻机](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [月之暗面发布 Kimi K3：全球首个开源 2.8 万亿参数模型](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

月之暗面（Moonshot AI）在 Hugging Face 上开源了 Kimi K3 模型，这是全球首个 2.8 万亿参数（3T 级别）的开源模型，激活参数 104B，采用基于 Stable LatentMoE 框架的全新 Kimi Delta Attention（KDA）和 Attention Residuals（AttnRes）架构。 此次发布标志着开源 AI 的一个重要里程碑，提供了一个与 GPT-5.6 Sol 和 Claude Fable 5 等专有系统竞争的前沿模型，可能加速长上下文、多模态和智能体应用的研究与开发。 Kimi K3 采用混合专家架构，共 896 个专家，每 token 激活 16 个，原生支持文本、图像和视频理解，上下文窗口达 100 万 token。模型按 Kimi K3 License 发布，并支持 MXFP4 量化以实现高效部署。

telegram · zaihuapd · 7月27日 15:15

**背景**: 大型语言模型发展迅速，总参数已达万亿级别，但由于混合专家（MoE）技术，每次推理仅激活其中一小部分。Stable LatentMoE 是一种新的 MoE 框架，利用潜在空间表示改进了路由和负载均衡。Kimi Delta Attention 是一种线性注意力机制，旨在高效处理长上下文和多模态任务，通过更细粒度的门控机制扩展了之前的 Gated DeltaNet 等工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://huggingface.co/blog/ResterChed/kimi-k3-model-overview-mxfp4-quantization-open-wei">Kimi K3 Model Overview: 2.8T Parameters, MXFP4 Quantization, and...</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**社区讨论**: Telegram 上的讨论似乎是预告而非技术讨论；所提供的材料中没有实质性的社区反应。

**标签**: `#AI`, `#Open Source Model`, `#Moonshot AI`, `#Large Language Model`, `#Mixture of Experts`

---

<a id="item-2"></a>
## [Fastjson2 曝远程代码执行漏洞，所有版本受影响，尚无补丁](https://mp.weixin.qq.com/s/LJaul1jNjK9pXRAkoUiMEA) ⭐️ 9.0/10

7 月 27 日，长亭科技披露了 Fastjson2 存在远程代码执行漏洞，影响 2.0.62 及之前所有版本。项目维护者已确认该安全问题，但尚未发布官方补丁。 这是一个影响 Fastjson2 所有版本的严重零日漏洞。Fastjson2 是广泛使用的 Java JSON 库。攻击者可以通过恶意 JSON 数据绕过 AutoType 类型校验并执行任意代码，对使用 Fastjson2 的应用构成严重威胁。 该漏洞允许绕过 AutoType 类型校验。PR \#7695 已关闭且未合入主分支，因此所有已发布版本均无正式补丁。作为临时缓解措施，建议用户彻底禁用 AutoType。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson2 是阿里巴巴开发的 Java 高性能 JSON 库。AutoType 特性允许在序列化的 JSON 字符串中包含类型信息，这可能被利用来反序列化任意对象。此前 Fastjson 1.x 版本也曾出现类似的与 AutoType 相关的远程代码执行漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson2/blob/main/docs/autotype_en.md">fastjson 2 /docs/ autotype _en.md at main · alibaba/ fastjson 2 · GitHub</a></li>
<li><a href="https://alibaba.github.io/fastjson2/autotype_cn.html">FASTJSON 2 Autotype 机制介绍 | fastjson 2</a></li>
<li><a href="https://developer.aliyun.com/article/1749997">Fastjson 远 程 代 码 执 行 漏 洞 ，阿里云AI...</a></li>

</ul>
</details>

**标签**: `#安全`, `#漏洞`, `#Fastjson2`, `#RCE`, `#Java`

---

<a id="item-3"></a>
## [vLLM v0.26.0 发布，引入 Inkling 模型系列与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 引入了全新的 Inkling 模型系列，完整支持包括 Hopper FA4 相对注意力、NVFP4 量化以及 MTP 推测解码，同时还针对 DeepSeek-V4 进行了多厂商的性能大幅提升，并支持通过 head\_dtype 使用 fp32 lm\_head。 此次发布增强了 vLLM 作为领先 LLM 推理引擎的地位，增加了 NVFP4 量化和 MTP 解码等前沿功能，可提升生产部署的吞吐量和准确性。对 DeepSeek-V4 的优化展示了 vLLM 能够跨硬件供应商为流行模型带来显著的性能提升。 该版本包含来自 212 位贡献者的 411 次提交，其中针对 DeepSeek-V4 的专用路由内核实现了 2.94% 的端到端 TPOT 改进，fp32 lm\_head 支持也扩展到了 LoRA 路径。现在可以按 KV-cache 组选择灵活的注意力后端，Rust 前端新增了多模态视频和音频支持。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎。Inkling 模型系列是一组新模型，利用 Hopper FA4 注意力（针对 Hopper GPU 的 FlashAttention-4）和 NVFP4 量化（4 位浮点权重）等先进技术来提高效率。MTP（多令牌预测）是一种推测解码方法，每次前向传播预测多个令牌，从而降低延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design ...</a></li>
<li><a href="https://www.spheron.network/blog/tensorrt-model-optimizer-modelopt-quantization-guide/">NVIDIA TensorRT Model Optimizer (ModelOpt): FP8, INT4, and FP4 Quantization Guide (2026) | Spheron Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#model optimization`, `#DeepSeek`, `#release`

---

<a id="item-4"></a>
## [Anthropic 澄清开放权重模型立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布声明，澄清其并不主张禁止开放权重模型（open-weights models），而是呼吁对所有足够强大的模型进行强制性安全测试，并打击工业规模的蒸馏（distillation）操作。 这一来自顶级 AI 公司的声明塑造了关于开放权重模型监管的辩论，表明了一种中间立场，但许多批评者认为，通过昂贵的测试要求可能实际上限制了开放模型。 Anthropic 没有明确测试标准或由谁执行，而且其打击蒸馏的呼吁可能对小开发者产生过大影响，因为他们依赖蒸馏来创建高效模型。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型（open-weights models）是指其训练参数（权重）公开可供下载和使用的 AI 模型，任何人都可以查看、修改和运行。知识蒸馏（knowledge distillation）是一种将大模型的知识迁移到小模型的技术，常用于创建高效模型。围绕开放权重模型的争论聚焦于在开放性与安全风险之间取得平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍批评 Anthropic 的立场自相矛盾，认为强制性安全测试和打击蒸馏实际上等同于禁止。有人指出 Anthropic 在盗版诉讼中的和解是虚伪的，而另一些人则担心测试管理中的政府过度干预。

**标签**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`

---

<a id="item-5"></a>
## [论坛软件从 React 迁移到 HTMX](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

Misago 论坛软件项目宣布，他们已从代码库中移除 React.js，并采用 HTMX 实现 UI 交互，用超媒体驱动的 HTML 属性取代了复杂的 JavaScript 框架。 这一迁移突显了 Web 开发中日益增长的趋势：开发人员选择更简单的服务器渲染方式而非笨重的客户端框架，从而可能降低复杂性并改善论坛这类内容密集型应用的性能。 该项目用 HTMX 取代了 React，HTMX 是一个使用 HTML 属性实现 AJAX 请求、CSS 过渡和 WebSocket 支持的库，无需自定义 JavaScript。社区评论指出大型表单存在性能问题，但称赞 HTMX 适合论坛场景。

hackernews · Ralfp · 7月27日 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: HTMX 是一个开源前端库，通过自定义属性扩展 HTML，使开发者能够使用服务器渲染的 HTML 片段构建动态界面。与 React 的客户端渲染不同，HTMX 利用超媒体原则，由服务器返回 HTML，库负责交换 DOM 部分。这种方法可以简化代码并减小包体积，但在需要复杂状态管理的高度交互式 UI 中可能表现不佳。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一但整体支持；一些用户称赞 HTMX 简单且适合论坛，而另有一人报告大型表单的性能问题。有评论推荐了 PyView 等替代方案，还有人指出需要时可以在模板中嵌入小型 React/Vue 应用。

**标签**: `#HTMX`, `#React`, `#Web Development`, `#Server-Side Rendering`

---

<a id="item-6"></a>
## [用借用的协议重构电子邮件架构](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

一篇博客文章提出，可以利用现代协议（如基于 HTTP 的 JMAP）的组件来构建现代电子邮件，而非依赖传统的 SMTP/IMAP 协议。 电子邮件仍是关键的通信工具，但其底层架构数十年来几乎未变，导致垃圾邮件等问题持续存在。用借用的协议重新思考电子邮件，可能带来更安全、高效的邮件系统，但面临巨大的网络效应障碍。 文章特别建议借用 JMAP（用 JSON API over HTTP 替代 IMAP/CardDAV/CalDAV）以及其他现代传输和认证协议。但任何新邮件协议必须保持与 SMTP 的向后兼容性以实现迁移。

hackernews · andros · 7月27日 08:27 · [社区讨论](https://news.ycombinator.com/item?id=49066639)

**背景**: 电子邮件基于 SMTP 进行传输，使用 IMAP/POP3 进行访问，这些协议设计于数十年前，当时安全性和垃圾邮件并非主要关注点。网络效应使得替换电子邮件极其困难，因为几乎每个人都有电子邮件地址，任何新协议都需要广泛采用才能发挥作用。JMAP（JSON 元应用协议）是一个开放标准，旨在通过使用 HTTP 和 JSON 来现代化电子邮件访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Network_effect">Network effect - Wikipedia</a></li>
<li><a href="https://jmap.io/">JSON Meta Application Protocol Specification (JMAP)</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了怀疑，指出许多垃圾邮件解决方案在历史上都失败了，网络效应使得替换几乎不可能。一些人主张渐进式修复，比如为发送邮件增加经济摩擦，而另一些人则认为当前的邮件栈并不像人们认为的那样糟糕，并引用了缺乏成功再造的案例。

**标签**: `#email`, `#protocols`, `#network-effects`, `#architecture`, `#spam`

---

<a id="item-7"></a>
## [独立评估发现 6 个前沿 LLM 均左倾，包括 Grok](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

一项独立评估测试了 6 个前沿 LLM——GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.7、Gemini Pro、Gemini Flash 和 Grok 4.3——在 8 个偏见基准上约 20,600 个样本，发现所有模型均表现出左倾政治偏见，包括自称为右倾的 Grok。 该评估突显了主要 LLM 中普遍存在的政治偏见，挑战了其中立性声称，并引发了对 AI 部署公平性的担忧，尤其是在需要保持公正的应用中。 值得注意的是，Grok 自称右倾但在内容分类或政策问答时表现左倾；种族相关问题的拒绝率差异显著：GPT-5.4 拒绝 20.3%，Claude Opus 4.7 为 13.8%，Grok 为 9.5%，其他模型约 5%。

reddit · r/MachineLearning · /u/marggggggggg · 7月27日 22:37

**背景**: 偏见基准如 WinoBias（指代消解中的性别偏见）、BBQ（问答中的社会偏见）和 SeeGULL（刻板印象数据集）是衡量语言模型公平性的标准工具。该研究使用了八个覆盖政治、性别和种族偏见的此类数据集来评估模型行为。该评估为个人、未经同行评审的项目，采用单一提示模板且未进行多次运行平均，因此结果应谨慎解读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2110.08193">BBQ : A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>
<li><a href="https://uclanlp.github.io/corefBias/overview">WinoBias dataset</a></li>

</ul>
</details>

**标签**: `#LLM bias`, `#fairness evaluation`, `#political bias`, `#frontier models`, `#AI ethics`

---

<a id="item-8"></a>
## [华为被指筹建月产 14 万片晶圆的 DRAM 工厂](https://www.xda-developers.com/huawei-is-building-its-own-dram-fab-and-it-could-reshape-ram-prices-for-everyone/) ⭐️ 8.0/10

据报道，华为正与深圳 DRAM 初创公司昇维旭合作，在中国建设一座 12 英寸 DRAM 晶圆厂，规划月产能约 14 万片晶圆。华为已否认相关说法，但分析人士认为此举旨在保障其昇腾 AI 芯片的内存供应。 若该项目实现，新增产能可能显著影响全球 DRAM 供应链并可能降低价格，尤其是在地缘政治紧张影响芯片进口的背景下。这凸显了华为在 AI 芯片组件方面推动自给自足的努力。 该工厂将是 12 英寸晶圆厂，昇维旭是一家 2022 年成立的国资背景公司，拥有前台积电和尔必达高管。但工厂建设和量产仍需数年时间，因此短期内不太可能影响消费级 DRAM 价格。

telegram · zaihuapd · 7月27日 03:17

**背景**: DRAM（动态随机存取存储器）是一种用于计算机、服务器和 AI 芯片的半导体存储器。华为的昇腾 AI 芯片依赖高带宽内存，目前从长鑫存储（CXMT）等外部供应商采购。中美科技冲突限制了华为获取先进芯片和设备，促使该公司寻求国内替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swaysure.com/">SwaySure - 深圳市昇维旭技术有限公司官网</a></li>
<li><a href="https://baike.baidu.com/item/%E6%B7%B1%E5%9C%B3%E5%B8%82%E6%98%87%E7%BB%B4%E6%97%AD%E6%8A%80%E6%9C%AF%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8/61554951">深圳市昇维旭技术有限公司_百度百科</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/533101886">揭秘50亿国产DRAM企业：挖来前台积电厂长+前尔必达社长！</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#DRAM`, `#Huawei`, `#AI chips`, `#supply chain`

---

<a id="item-9"></a>
## [谷歌透露 Gemini 4 为迄今最雄心预训练，预计年底发布](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

谷歌 CEO 桑达尔·皮查伊在 Alphabet 2026 年第二季度财报电话会议上透露，Gemini 4 已进入预训练阶段，称这是该公司迄今为止最具雄心的预训练项目。该模型预计于 2026 年底（11 月或 12 月）发布。 这表明谷歌致力于保持在 AI 前沿，因为更大的基础模型对于迈向通用人工智能（AGI）至关重要。Gemini 4 的发布可能显著改变领先 AI 实验室之间的竞争格局，并推动大型语言模型的进一步创新。 皮查伊强调，谷歌将优先将算力分配给前沿 AGI 研发，以确保 Gemini 4 在发布时仍处于行业前沿。此外，Gemini 3.x Flash 系列将保持几乎每月一次的迭代频率，重点提升智能编码等能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 预训练是大型语言模型通过自监督学习从海量文本语料中学习语言模式的初始阶段，为后续针对特定任务的微调奠定基础。通用人工智能（AGI）指一种假设的 AI 系统，能够在广泛任务中理解、学习并应用知识，其能力达到或超越人类水平。更大的模型在更多数据上训练通常表现更好，这促使谷歌等公司投资于规模越来越大的预训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>
<li><a href="https://nlp.cs.princeton.edu/cos484-sp24/lectures/lec16.pdf">L16: Pre-training and large language models (LLMs)</a></li>

</ul>
</details>

**标签**: `#Google`, `#Gemini 4`, `#AI`, `#large language model`, `#pre-training`

---

<a id="item-10"></a>
## [中国开始量产国产 DUV 光刻机](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 8.0/10

中国已开始大规模量产国产浸没式深紫外（DUV）光刻机，计划 2025 年生产约 5 台，2027 年约 20 台，交付中芯国际、华虹半导体等国内主要芯片制造商。 这一半导体自给自足的里程碑可能逐步侵蚀 ASML 在中国市场的份额，尤其是在西方出口管制收紧的情况下。不过，该技术在性能和可靠性上仍落后于 ASML。 国产 DUV 光刻机主要使用国产零部件，但部分关键部件仍来自日本，今年国内供应链延误已影响进度。客户可能需要数月时间测试精度与兼容性，方能投入量产产线。

telegram · zaihuapd · 7月27日 14:10

**背景**: DUV 光刻利用深紫外光（248nm 或 193nm 波长）在半导体晶圆上刻印图案，浸没式光刻通过在镜头与晶圆之间加入液体层来提高分辨率。ASML 主导该市场，中国一直努力自主研发光刻设备，以在美国主导的出口管制下减少对外国技术的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DUV_lithography">DUV lithography</a></li>
<li><a href="https://en.wikipedia.org/wiki/Immersion_lithography">Immersion lithography</a></li>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products - ASML</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#lithography`, `#China`, `#ASML`, `#chip manufacturing`

---