---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 31 items, 10 important content pieces were selected

---

1. [Moonshot AI Releases Kimi K3: First Open-Source 3T-Parameter Model](#item-1) ⭐️ 9.0/10
2. [Fastjson2 RCE Vulnerability Affects All Versions, No Patch Yet](#item-2) ⭐️ 9.0/10
3. [vLLM v0.26.0 Released with Inkling Models, DeepSeek-V4 Optimizations](#item-3) ⭐️ 8.0/10
4. [Anthropic Clarifies Open-Weights Model Position](#item-4) ⭐️ 8.0/10
5. [Forum Software Migrates from React to HTMX](#item-5) ⭐️ 8.0/10
6. [Rethinking Email Architecture with Borrowed Protocols](#item-6) ⭐️ 8.0/10
7. [Solo evaluation finds all 6 frontier LLMs lean left including Grok](#item-7) ⭐️ 8.0/10
8. [Huawei Reportedly Building DRAM Fab with 140K Wafers/Month](#item-8) ⭐️ 8.0/10
9. [Google reveals Gemini 4 as its most ambitious pre-training project, launch by end of 2026](#item-9) ⭐️ 8.0/10
10. [China starts mass producing domestic DUV lithography machines](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Moonshot AI Releases Kimi K3: First Open-Source 3T-Parameter Model](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

Moonshot AI has open-sourced Kimi K3 on Hugging Face, the world&\#x27;s first 2.8 trillion parameter \(3T-scale\) model with 104B active parameters, featuring the novel Kimi Delta Attention \(KDA\) and Attention Residuals \(AttnRes\) architectures built on the Stable LatentMoE framework. This release marks a significant milestone in open-source AI by providing a frontier-scale model that rivals proprietary systems like GPT-5.6 Sol and Claude Fable 5, potentially accelerating research and development in long-context, multimodal, and agentic applications. Kimi K3 uses a Mixture-of-Experts architecture with 896 total experts, activating 16 per token, and supports native text, image, and video understanding with a 1 million token context window. The model is released under the Kimi K3 License and supports MXFP4 quantization for efficient deployment.

telegram · zaihuapd · Jul 27, 15:15

**Background**: Large language models have grown rapidly, with total parameters now reaching trillions but with only a fraction active per inference due to mixture-of-experts \(MoE\) techniques. Stable LatentMoE is a new MoE framework that improves routing and load balancing using latent-space representations. Kimi Delta Attention is a linear attention mechanism designed for efficient long-context and multimodal processing, extending prior work like Gated DeltaNet with finer-grained gating.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://huggingface.co/blog/ResterChed/kimi-k3-model-overview-mxfp4-quantization-open-wei">Kimi K3 Model Overview: 2.8T Parameters, MXFP4 Quantization, and...</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**Discussion**: The discussion from Telegram appears to be a pre-announcement rather than a technical discussion; no substantive community reactions are available in the provided content.

**Tags**: `#AI`, `#Open Source Model`, `#Moonshot AI`, `#Large Language Model`, `#Mixture of Experts`

---

<a id="item-2"></a>
## [Fastjson2 RCE Vulnerability Affects All Versions, No Patch Yet](https://mp.weixin.qq.com/s/LJaul1jNjK9pXRAkoUiMEA) ⭐️ 9.0/10

On July 27, Chaitin Technology disclosed a remote code execution \(RCE\) vulnerability in Fastjson2, affecting version 2.0.62 and earlier \(i.e., all released versions\). The project maintainer has confirmed the issue but no official patch has been released. This is a critical zero-day vulnerability affecting every version of Fastjson2, a widely used Java JSON library. Attackers can bypass AutoType validation via malicious JSON data to execute arbitrary code, posing a severe risk to applications that use Fastjson2. The vulnerability allows bypassing AutoType validation. The PR \#7695 was closed without merging into the main branch, meaning there is no fix in any published version. As a temporary mitigation, users are advised to completely disable AutoType.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson2 is a high-performance JSON library for Java developed by Alibaba. The AutoType feature allows type information to be included in serialized JSON strings, which can be exploited to deserialize arbitrary objects. Previous versions of Fastjson \(1.x\) have also suffered from similar RCE vulnerabilities related to AutoType.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson2/blob/main/docs/autotype_en.md">fastjson 2 /docs/ autotype _en.md at main · alibaba/ fastjson 2 · GitHub</a></li>
<li><a href="https://alibaba.github.io/fastjson2/autotype_cn.html">FASTJSON 2 Autotype 机制介绍 | fastjson 2</a></li>
<li><a href="https://developer.aliyun.com/article/1749997">Fastjson 远 程 代 码 执 行 漏 洞 ，阿里云AI...</a></li>

</ul>
</details>

**Tags**: `#安全`, `#漏洞`, `#Fastjson2`, `#RCE`, `#Java`

---

<a id="item-3"></a>
## [vLLM v0.26.0 Released with Inkling Models, DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces the new Inkling model family with full support including Hopper FA4 relative attention, NVFP4 quantization, and MTP speculative decoding, along with significant performance improvements for DeepSeek-V4 across vendors and support for fp32 lm\_head via head\_dtype. This release strengthens vLLM&\#x27;s position as a leading LLM inference engine by adding cutting-edge features like NVFP4 quantization and MTP decoding, which can improve throughput and accuracy for production deployments. The DeepSeek-V4 optimizations demonstrate vLLM&\#x27;s ability to deliver major performance gains for popular models across hardware vendors. The release includes 411 commits from 212 contributors, featuring a specialized routing kernel for DeepSeek-V4 yielding a 2.94% E2E TPOT improvement, and fp32 lm\_head support extends to the LoRA path. Flexible attention backends can now be selected per KV-cache group, and the Rust frontend added multimodal video and audio support.

github · khluu · Jul 27, 01:06

**Background**: vLLM is an open-source high-throughput LLM inference engine. The Inkling model family is a new set of models leveraging advanced techniques like Hopper FA4 attention \(FlashAttention-4 for Hopper GPUs\) and NVFP4 quantization \(4-bit floating point weights\) to improve efficiency. MTP \(Multi-Token Prediction\) is a speculative decoding method that predicts multiple tokens per forward pass, reducing latency.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design ...</a></li>
<li><a href="https://www.spheron.network/blog/tensorrt-model-optimizer-modelopt-quantization-guide/">NVIDIA TensorRT Model Optimizer (ModelOpt): FP8, INT4, and FP4 Quantization Guide (2026) | Spheron Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#model optimization`, `#DeepSeek`, `#release`

---

<a id="item-4"></a>
## [Anthropic Clarifies Open-Weights Model Position](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic published a statement clarifying it does not advocate for banning open-weights models, but instead calls for mandatory safety testing for all capable models and cracking down on industrial-scale distillation. This statement from a leading AI company shapes the debate around open-weights regulation, signaling a middle ground that many critics argue could effectively restrict open models through costly testing requirements. Anthropic did not specify the testing criteria or who would administer them, and its call to crack down on distillation may disproportionately affect smaller developers who rely on distillation to create efficient models.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open weight models are AI models whose trained parameters \(weights\) are publicly available for download and use, enabling anyone to inspect, modify, and run them. Knowledge distillation is a technique where knowledge from a large model is transferred to a smaller one, often used to create efficient models. The debate centers on balancing openness with safety risks.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters overwhelmingly criticized Anthropic&\#x27;s stance as contradictory, arguing that mandatory safety testing and distillation crackdowns effectively constitute a ban. Some pointed to Anthropic&\#x27;s own settlement in a piracy lawsuit as hypocritical, while others raised concerns about government overreach in testing administration.

**Tags**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`

---

<a id="item-5"></a>
## [Forum Software Migrates from React to HTMX](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

The Misago forum software project announced they have removed React.js from their codebase and adopted HTMX for UI interactivity, replacing a complex JavaScript framework with hypermedia-driven HTML attributes. This migration highlights a growing trend in web development where developers opt for simpler, server-rendered approaches over heavy client-side frameworks, potentially reducing complexity and improving performance for content-heavy applications like forums. The project replaced React with HTMX, a library that uses HTML attributes to enable AJAX requests, CSS transitions, and WebSocket support without custom JavaScript. Community comments noted performance issues with large forms but praised HTMX&\#x27;s fit for forums.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: HTMX is an open-source front-end library that extends HTML with custom attributes, allowing developers to build dynamic interfaces using server-rendered HTML fragments. Unlike React&\#x27;s client-side rendering, HTMX leverages hypermedia principles, where the server returns HTML and the library swaps parts of the DOM. This approach can lead to simpler code and smaller bundles, though it may struggle with highly interactive UIs requiring complex state management.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**Discussion**: Community comments were mixed but generally supportive; some users praised HTMX for simplicity and fit for forums, while one reported performance issues with large forms. Alternatives like PyView were suggested, and others noted that mini React/Vue apps can be embedded when needed.

**Tags**: `#HTMX`, `#React`, `#Web Development`, `#Server-Side Rendering`

---

<a id="item-6"></a>
## [Rethinking Email Architecture with Borrowed Protocols](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 8.0/10

A blog post argues that modern email can be built from borrowed parts of modern protocols, such as JMAP over HTTP, rather than relying on legacy SMTP/IMAP. Email remains a critical communication tool, but its underlying architecture has been largely unchanged for decades, leading to persistent problems like spam and lack of modern features. Rethinking email with borrowed protocols could lead to more secure and efficient email systems, but faces immense network effect barriers. The article specifically suggests borrowing from JMAP, which replaces IMAP/CardDAV/CalDAV with JSON APIs over HTTP, and other modern transport and authentication protocols. However, any new email protocol must maintain backward compatibility with SMTP to enable migration.

hackernews · andros · Jul 27, 08:27 · [Discussion](https://news.ycombinator.com/item?id=49066639)

**Background**: Email was built on SMTP for transfer and IMAP/POP3 for access, designed decades ago when security and spam were not primary concerns. Network effects make it extremely difficult to replace email because virtually everyone has an email address and any new protocol requires widespread adoption to be useful. JMAP \(JSON Meta Application Protocol\) is an open standard that aims to modernize email access by using HTTP and JSON.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Meta_Application_Protocol">JSON Meta Application Protocol - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Network_effect">Network effect - Wikipedia</a></li>
<li><a href="https://jmap.io/">JSON Meta Application Protocol Specification (JMAP)</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism, noting that many spam solutions have failed historically and that network effects make replacement nearly impossible. Some advocate for incremental fixes like economic friction for sending emails, while others argue the current stack is not as broken as claimed, citing the lack of successful reinvention.

**Tags**: `#email`, `#protocols`, `#network-effects`, `#architecture`, `#spam`

---

<a id="item-7"></a>
## [Solo evaluation finds all 6 frontier LLMs lean left including Grok](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

A solo evaluation tested six frontier LLMs—GPT-5.4, Claude Sonnet 4.6, Claude Opus 4.7, Gemini Pro, Gemini Flash, and Grok 4.3—across 8 bias benchmarks with about 20,600 examples, finding that all models exhibit left-leaning political bias, including Grok despite its self-reported right-leaning stance. This evaluation highlights persistent political bias across major LLMs, challenging claims of neutrality and raising concerns for fairness in AI deployment, especially for applications that must appear impartial. Notably, Grok self-reports as right-leaning but behaves left-leaning when classifying content or answering policy questions; refusal rates on race-related questions varied: GPT-5.4 refused 20.3% of the time, Claude Opus 4.7 13.8%, Grok 9.5%, and others around 5%.

reddit · r/MachineLearning · /u/marggggggggg · Jul 27, 22:37

**Background**: Bias benchmarks like WinoBias \(gender bias in coreference\), BBQ \(social bias in QA\), and SeeGULL \(stereotype dataset\) are standard tools for measuring fairness in language models. This study used eight such datasets covering political, gender, and racial bias to assess model behavior. The evaluation was a solo, non-peer-reviewed project with single prompt templates and no multi-run averaging, so results should be interpreted with caution.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2110.08193">BBQ : A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>
<li><a href="https://uclanlp.github.io/corefBias/overview">WinoBias dataset</a></li>

</ul>
</details>

**Tags**: `#LLM bias`, `#fairness evaluation`, `#political bias`, `#frontier models`, `#AI ethics`

---

<a id="item-8"></a>
## [Huawei Reportedly Building DRAM Fab with 140K Wafers/Month](https://www.xda-developers.com/huawei-is-building-its-own-dram-fab-and-it-could-reshape-ram-prices-for-everyone/) ⭐️ 8.0/10

Huawei is reportedly partnering with Shenzhen-based DRAM startup SwaySure to build a 12-inch DRAM fab in China with a planned monthly capacity of around 140,000 wafers. Huawei has denied the claims, but analysts believe the move aims to secure memory supply for its Ascend AI chips. If realized, this capacity could significantly impact global DRAM supply chains and potentially lower prices, especially amid geopolitical tensions affecting chip imports. It underscores Huawei&\#x27;s push for self-reliance in AI chip components. The fab would be a 12-inch wafer facility, and SwaySure is a state-backed company established in 2022, with former TSMC and Elpida executives. However, building and ramping production will take years, so near-term impact on consumer DRAM prices is unlikely.

telegram · zaihuapd · Jul 27, 03:17

**Background**: DRAM \(Dynamic Random Access Memory\) is a type of semiconductor memory used in computers, servers, and AI chips. Huawei&\#x27;s Ascend AI chips rely on high-bandwidth memory, which is currently sourced from external suppliers like ChangXin Memory Technologies \(CXMT\). The US-China tech conflict has restricted Huawei&\#x27;s access to advanced chips and equipment, prompting the company to seek domestic alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.swaysure.com/">SwaySure - 深圳市昇维旭技术有限公司官网</a></li>
<li><a href="https://baike.baidu.com/item/%E6%B7%B1%E5%9C%B3%E5%B8%82%E6%98%87%E7%BB%B4%E6%97%AD%E6%8A%80%E6%9C%AF%E6%9C%89%E9%99%90%E5%85%AC%E5%8F%B8/61554951">深圳市昇维旭技术有限公司_百度百科</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/533101886">揭秘50亿国产DRAM企业：挖来前台积电厂长+前尔必达社长！</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#DRAM`, `#Huawei`, `#AI chips`, `#supply chain`

---

<a id="item-9"></a>
## [Google reveals Gemini 4 as its most ambitious pre-training project, launch by end of 2026](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

Google CEO Sundar Pichai announced during the Alphabet Q2 2026 earnings call that Gemini 4 has entered pre-training, calling it the company&\#x27;s most ambitious pre-training project to date. The model is expected to launch by the end of 2026, likely in November or December. This signals Google&\#x27;s commitment to staying at the frontier of AI, as larger foundation models are crucial for advancing toward artificial general intelligence \(AGI\). The release of Gemini 4 could significantly impact the competitive landscape among leading AI labs and drive further innovation in large language models. Pichai emphasized that Google will prioritize compute allocation for frontier AGI research and development to ensure Gemini 4 remains cutting-edge at launch. Additionally, the Gemini 3.x Flash series will continue with near-monthly iteration cycles, focusing on improvements in coding capabilities.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Pre-training is the initial phase where large language models learn language patterns from massive text corpora using self-supervised learning, forming the foundation for later fine-tuning on specific tasks. Artificial General Intelligence \(AGI\) refers to a hypothetical AI system that can understand, learn, and apply knowledge across a wide range of tasks at a level comparable to or surpassing human abilities. Larger models trained on more data generally exhibit better performance, which drives companies like Google to invest in ever-larger pre-training runs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>
<li><a href="https://nlp.cs.princeton.edu/cos484-sp24/lectures/lec16.pdf">L16: Pre-training and large language models (LLMs)</a></li>

</ul>
</details>

**Tags**: `#Google`, `#Gemini 4`, `#AI`, `#large language model`, `#pre-training`

---

<a id="item-10"></a>
## [China starts mass producing domestic DUV lithography machines](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 8.0/10

China has begun mass-producing domestic immersion deep ultraviolet \(DUV\) lithography machines, planning to produce about 5 units in 2025 and 20 units by 2027 for use by major Chinese chipmakers like SMIC and Hua Hong. This milestone in semiconductor self-sufficiency could gradually erode ASML&\#x27;s market share in China, especially if Western export controls tighten. However, the technology still lags behind ASML in performance and reliability. The domestic DUV machines mainly use Chinese-made components, but some critical parts still come from Japan, and domestic supply chain delays have already affected progress this year. Customers may need months to test precision and compatibility before mass production use.

telegram · zaihuapd · Jul 27, 14:10

**Background**: DUV lithography uses deep ultraviolet light \(248nm or 193nm wavelength\) to pattern semiconductor wafers, with immersion lithography using a liquid layer between the lens and wafer to improve resolution. ASML dominates the market, and China has been striving to develop its own lithography equipment to reduce dependence on foreign technology amid US-led export restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DUV_lithography">DUV lithography</a></li>
<li><a href="https://en.wikipedia.org/wiki/Immersion_lithography">Immersion lithography</a></li>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products - ASML</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#lithography`, `#China`, `#ASML`, `#chip manufacturing`

---