---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 25 条内容中筛选出 8 条重要资讯。

---

1. [SGLang v0.5.16 发布：DSpark 与 Inkling 975B 支持](#item-1) ⭐️ 9.0/10
2. [vLLM v0.26.0：支持 Inkling 模型家族，DeepSeek-V4 性能提升，灵活注意力后端](#item-2) ⭐️ 8.0/10
3. [Android 可能限制设备上的 ADB 访问](#item-3) ⭐️ 8.0/10
4. [开源权重 AI 的 Kubernetes 时刻](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 显示对提示注入的强抵抗力](#item-5) ⭐️ 8.0/10
6. [AMD 软件生产挑战阻碍 CUDA 护城河突破](#item-6) ⭐️ 8.0/10
7. [市场监管总局对携程开出 51.79 亿元反垄断罚单](#item-7) ⭐️ 8.0/10
8. [苹果游说特朗普采用中国存储芯片，美光阻挠](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.16 发布：DSpark 与 Inkling 975B 支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 引入了 DSpark，一种置信度驱动的推测解码算法，实现了高吞吐量，并增加了对 Inkling 975B 参数多模态 MoE 模型的支持。 此版本通过 DSpark 的自适应验证显著提升了推理吞吐量，并支持服务庞大的 975B 参数 Inkling 模型，推动了高效 LLM 服务的边界。 DSpark 以半自回归方式分块草稿，并根据置信度调整验证窗口大小，在 DeepSeek-V4-Pro 上达到 383.7 tok/s。Inkling 是一个 975B 总参数/41B 激活的多模态 MoE，支持文本、图像、音频，上下文达 1M。此版本还移除了实验性的 QServe 和 FBGEMM FP8 量化路径。

github · Qiaolin-Yu · 7月25日 00:13

**背景**: 推测解码通过使用草稿模型生成令牌，然后由目标模型验证，从而加速 LLM 推理。DSpark 的创新在于根据草稿模型的置信度调整验证长度，提高效率。混合专家（MoE）模型每个令牌只激活部分参数，从而在可控计算下实现大总参数量。Inkling 总参数 975B、激活 41B，是一个重要的开源权重例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-07-06-dspark-sglang">DSpark in SGLang: Speculative Decoding with Confidence-Driven ...</a></li>
<li><a href="https://ai-trove.com/en/inkling">Inkling — 975 B open multimodal MoE | text, image, audio</a></li>
<li><a href="https://arxiv.org/abs/2607.05147">[2607.05147] DSpark: Confidence-Scheduled Speculative ...</a></li>

</ul>
</details>

**标签**: `#SGLang`, `#speculative decoding`, `#LLM inference`, `#DSpark`, `#Inkling`

---

<a id="item-2"></a>
## [vLLM v0.26.0：支持 Inkling 模型家族，DeepSeek-V4 性能提升，灵活注意力后端](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 引入了对全新 Inkling 模型家族的完整支持栈，跨供应商对 DeepSeek-V4 进行了显著的性能提升，通过 head\_dtype 支持 fp32 lm\_head，以及可按 KV-cache 组选择的灵活注意力后端。 此次发布为 DeepSeek-V4 等先进模型的推理带来了重大优化，并扩展了对 Inkling 等新架构的支持，使开发者更容易部署高性能 LLM。灵活的注意力后端和 KV 卸载增强提高了生产环境的效率和可扩展性。 Inkling 家族包括基础建模、分段 CUDA 图支持、Hopper FA4 相对注意力、MTP=1 推测解码、LoRA 和 ModelOpt NVFP4 量化。DeepSeek-V4 优化包括专用路由内核（端到端 TPOT 提升 2.94%）、fused\_topk\_bias（内核加速 1.5–2 倍）以及 ROCm 上的两阶段压缩器。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，支持多种模型和硬件加速器。此次发布包含来自 212 位贡献者的 411 次提交，是一个重要的更新，新增了模型家族并提升了性能。关键概念包括用于高效注意力计算的 FlashAttention、用于加速生成的推测解码，以及 NVFP4 等量化技术以减少内存占用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learnaivisually.com/ai-explained/vllm-v0-20-fa4-packing">vLLM v0.20 — FlashAttention 4 packing — What does it mean?</a></li>
<li><a href="https://docs.vllm.ai/projects/vllm-omni/en/latest/user_guide/quantization/modelopt/">ModelOpt - vLLM-Omni</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open-source`, `#performance optimization`, `#DeepSeek-V4`

---

<a id="item-3"></a>
## [Android 可能限制设备上的 ADB 访问](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

根据一篇高分报道，Android 正在考虑限制设备上的 ADB（Android 调试桥）访问，这将限制直接从设备本身进行调试和控制的能力。这一变化在开发者社区引发了激烈讨论。 这一限制可能严重影响依赖 ADB 进行调试、应用测试和自动化任务的 Android 开发者和高级用户。它代表了安全改进与开发者自由之间的权衡，可能会使某些工作流程变得更加繁琐。 拟议的更改针对的是设备上的 ADB（Wi-Fi 或本地主机），而非 USB ADB，并且需要同时启用开发者选项和远程 ADB 才能被利用。部分社区成员建议采用限制特定 IP 范围等替代方案，而不是完全阻止。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: Android 调试桥（ADB）是一个命令行工具，允许开发者与 Android 设备进行通信，用于调试、文件传输和运行 shell 命令。它可以通过 USB 或 TCP/IP 使用，设备上的 ADB 允许无需电脑即可进行无线调试。谷歌一直在逐步加强 Android 的安全性，此举被视为这一趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示出不同的反应：一些人认为攻击途径不切实际，因为它需要启用多个设置；而另一些人则认为这是进一步限制用户控制的步骤。一位通过 VPN 使用远程 ADB 的开发者对在公共 Wi-Fi 上暴露 ADB 表示担忧，但希望获得细粒度控制而不是全面禁止。

**标签**: `#Android`, `#ADB`, `#Developer Tools`, `#Security`, `#Google`

---

<a id="item-4"></a>
## [开源权重 AI 的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

一篇文章指出，开放权重 AI 模型正成为行业标准，其发展轨迹类似于 Kubernetes 在云基础设施中的崛起，这对模型治理和推理定价具有深远影响。 这种转变可能使 AI 访问民主化，减少供应商锁定，并通过提供基准来稳定推理定价，类似于 Kubernetes 实现的多云可移植性。然而，这也带来了治理挑战，例如按产地禁止模型的可行性。 该类比强调，一旦开放平台成为创新中心，任何单一供应商都无法匹敌联合创新速度。社区评论指出，代币经济学（每代币定价）一直不透明且摇摆不定，而开放权重模型为推理成本提供了合理的基准。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开放权重模型是一种其训练参数（权重）公开发布的人工智能模型，允许任何人下载并运行它。推理成本是在生产环境中运行模型所需的持续计算费用。Kubernetes 是一个开源容器编排系统，它已成为云基础设施的事实标准，实现了跨供应商的可移植性和创新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.cloudzero.com/blog/inference-cost/">Your Guide To Inference Cost (And Make It A Margin Advantage)</a></li>

</ul>
</details>

**社区讨论**: 评论者争论按产地禁止中国模型的可行性，认为权重只是数字，无法分配国家标签。其他人称赞文章关于开放平台的核心论断，讨论代币经济学的不透明性，并呼吁像 Kubernetes 的协作开发模式那样，开发训练数据公开的真正开放模型。

**标签**: `#open-weight`, `#AI`, `#Kubernetes`, `#model governance`, `#inference pricing`

---

<a id="item-5"></a>
## [Claude Opus 5 显示对提示注入的强抵抗力](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny 报告称，根据系统卡中记录的 prompt injection 评估和红队测试，Anthropic 的 Claude Opus 5 是目前最不易受提示注入影响的模型。 这表明在针对提示注入的 LLM 安全性方面取得了重大进展，提示注入一直是困扰 AI 系统的关键漏洞。更强的抵抗力增强了在真实世界应用中部署 LLM 的信任和安全性。 该说法得到了 Claude Opus 5 系统卡（第 73 页）中的评估和红队测试结果的支持。Anthropic 还指出，Opus 5 在发现漏洞方面有所改进，但故意避免在利用漏洞方面进行训练。

rss · Simon Willison · 7月25日 00:42

**背景**: 提示注入是一种安全漏洞，恶意输入会覆盖模型的预期指令，导致意外行为。对于像 Claude 这样的 LLM 来说，这是一个重大挑战，尤其是当模型获得网页浏览等能力时。红队测试是一种对抗性测试过程，用于在部署前发现此类漏洞。系统卡记录了 AI 模型的安全评估和负责任的部署决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection - OWASP Foundation</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-6"></a>
## [AMD 软件生产挑战阻碍 CUDA 护城河突破](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

AMD 发布了搭载 MI455X GPU 的 Helios AI 机架，并推出了自主内核生成技术 GEAK 以提升软件质量，但面临严重的生产爬坡困难和内部集群不稳定问题，财务工程甚至提供了高达 105%的折扣。 这之所以重要，是因为 AMD 能否与 NVIDIA 主导的 CUDA 生态系统竞争，取决于能否克服这些软件质量和生产挑战；成功将为 AI 工作负载提供可行替代方案，减少对 NVIDIA 硬件的依赖。 AMD 的 GEAK（生成高效 AI 内核）是一个利用多智能体系统和自进化知识库自动优化 GPU 内核的自主框架，但 MI455X 的 Infinity Fabric 带宽（896 GB/s）远低于 NVIDIA 的 NVLink 6（3.6 TB/s），且内部开发集群据称不稳定。

rss · Semianalysis · 7月25日 00:33

**背景**: NVIDIA 的 CUDA 平台一直是 GPU 计算领域领先的软件生态系统，提供全面的库和工具，使开发者锁定在 NVIDIA 硬件上。AMD 的开源替代方案 ROCm 在软件成熟度和开发者支持方面历史上一直落后。自主内核生成旨在自动化优化，减少手动工作，以在 AMD GPU 上达到 CUDA 级别的性能。Helios MI455X 是 AMD 最新的高端 AI 加速器，但其生产爬坡过程充满挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/AMD-AGI/GEAK">GitHub - AMD-AGI/GEAK: Generating Efficient AI-Centric ...</a></li>
<li><a href="https://rocm.blogs.amd.com/artificial-intelligence/kernel-optimization-agent/README.html">GEAK V3: Agent-Driven, Repository-Level GPU Kernel ...</a></li>
<li><a href="https://introl.com/blog/amd-helios-mi455x-nvidia-competition-ces-2026">AMD Helios Challenges NVIDIA: The MI 455 X and the... | Introl Blog</a></li>

</ul>
</details>

**标签**: `#AMD`, `#CUDA`, `#GPU`, `#AI hardware`, `#software ecosystem`

---

<a id="item-7"></a>
## [市场监管总局对携程开出 51.79 亿元反垄断罚单](https://www.xinhuanet.com/fortune/20260725/693124245aa44d2bbc7520b7a0c244ea/c.html) ⭐️ 8.0/10

国家市场监督管理总局对携程集团有限公司处以罚没款合计 51.79 亿元，其中没收违法所得 16.58 亿元，罚款 35.21 亿元，因其滥用市场支配地位实施垄断行为。 这是中国对科技公司开出的最大反垄断罚单之一，标志着对平台垄断行为的监管进一步收紧，为在线旅游市场的公平竞争树立了先例。 监管部门还责令携程立即停止违法行为，全额退还强制扣除酒店经营者的订单储备金 1.22 亿元，并要求其全面整改、公开整改措施。

telegram · zaihuapd · 7月25日 02:24

**背景**: 滥用市场支配地位是指具有市场支配地位的经营者利用其市场优势地位，实施排除、限制竞争的违法经营活动，违反《中华人民共和国反垄断法》。国家市场监督管理总局发布了《禁止滥用市场支配地位行为规定》以执行相关条款。携程作为中国最大的在线旅游平台，在酒店预订和旅行服务市场占据显著份额。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.samr.gov.cn/zw/zfxxgk/fdzdgknr/xwxcs/art/2023/art_78e487fb7b464e79880fdc8216c08c4c.html">《禁止滥用市场支配地位行为规定》解读</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#regulation`, `#Ctrip`, `#China`, `#tech industry`

---

<a id="item-8"></a>
## [苹果游说特朗普采用中国存储芯片，美光阻挠](https://www.wsj.com/tech/trump-apple-micron-china-chips-784bbd3d) ⭐️ 8.0/10

苹果 CEO 库克等高管近期向特朗普政府游说，希望在美国以外市场销售的产品中使用中国长鑫存储和长江存储的存储芯片，但美光科技正在积极阻挠。 这一游说凸显了全球科技供应链中降低成本与国家安全之间的紧张关系，若获批准可能重塑存储芯片市场，影响美国和中国芯片制造商。 苹果瞄准中国 DRAM 制造商长鑫存储和 NAND 闪存制造商长江存储，旨在降低非美国市场产品的成本。特朗普政府面临苹果及其主要供应商美光的双重压力，美光反对使用中国芯片。

telegram · zaihuapd · 7月25日 04:02

**背景**: 存储芯片是电子设备的关键组件，DRAM 用于临时数据存储，NAND 闪存用于长期存储。中国公司长鑫存储和长江存储已成为这些市场的主要参与者，挑战美光和三星等现有厂商。美国对向中国出口先进芯片实施了管制，但苹果的提议仅涉及在海外产品中使用中国芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/%E9%95%BF%E9%91%AB%E5%AD%98%E5%82%A8">长鑫存储 - 维基百科，自由的百科全书</a></li>
<li><a href="http://m.tetegu.com/gainiangu/changjiangchunchu/">长 江 存 储 概念股- 长 江 存 储 概念股龙头 - 特特股</a></li>

</ul>
</details>

**标签**: `#苹果`, `#美光`, `#存储芯片`, `#中美科技竞争`, `#供应链`

---