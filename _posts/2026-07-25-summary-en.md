---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 25 items, 8 important content pieces were selected

---

1. [SGLang v0.5.16: DSpark and Inkling 975B Support](#item-1) ⭐️ 9.0/10
2. [vLLM v0.26.0: Inkling model family, DeepSeek-V4 speed boost, flexible attention](#item-2) ⭐️ 8.0/10
3. [Android May Restrict On-Device ADB Access](#item-3) ⭐️ 8.0/10
4. [Open-Weight AI&\#x27;s Kubernetes Moment](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 Shows Strong Resistance to Prompt Injection](#item-5) ⭐️ 8.0/10
6. [AMD Faces Software and Production Hurdles to Break CUDA Moat](#item-6) ⭐️ 8.0/10
7. [China fines Ctrip $7.6 billion for antitrust abuse](#item-7) ⭐️ 8.0/10
8. [Apple Lobbies Trump to Use Chinese Memory Chips, Micron Objects](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.16: DSpark and Inkling 975B Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 introduces DSpark, a confidence-driven speculative decoding algorithm achieving high throughput, and adds support for the Inkling 975B-parameter multimodal MoE model. This release significantly boosts inference throughput with DSpark&\#x27;s adaptive verification, and enables serving of the massive 975B-parameter Inkling model, pushing the boundaries of efficient LLM serving. DSpark drafts semi-autoregressively in blocks and sizes verify windows based on confidence, reaching 383.7 tok/s on DeepSeek-V4-Pro. Inkling is a 975B total/41B active multimodal MoE with 1M context, supporting text, image, audio. The release also removes experimental QServe and FBGEMM FP8 quantization paths.

github · Qiaolin-Yu · Jul 25, 00:13

**Background**: Speculative decoding accelerates LLM inference by using a draft model to generate tokens that are then verified by the target model. DSpark innovates by adapting the verification length based on the draft model&\#x27;s confidence, improving efficiency. Mixture-of-Experts \(MoE\) models activate only a subset of parameters per token, enabling large total parameter counts with manageable compute. Inkling, with 975B total parameters and 41B active, is a notable open-weight example.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-07-06-dspark-sglang">DSpark in SGLang: Speculative Decoding with Confidence-Driven ...</a></li>
<li><a href="https://ai-trove.com/en/inkling">Inkling — 975 B open multimodal MoE | text, image, audio</a></li>
<li><a href="https://arxiv.org/abs/2607.05147">[2607.05147] DSpark: Confidence-Scheduled Speculative ...</a></li>

</ul>
</details>

**Tags**: `#SGLang`, `#speculative decoding`, `#LLM inference`, `#DSpark`, `#Inkling`

---

<a id="item-2"></a>
## [vLLM v0.26.0: Inkling model family, DeepSeek-V4 speed boost, flexible attention](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces support for the new Inkling model family with full stack capabilities, significant performance improvements for DeepSeek-V4 across vendors, fp32 lm\_head support via head\_dtype, and flexible attention backends that can be selected per KV-cache group. This release brings major optimizations for inference of state-of-the-art models like DeepSeek-V4 and expands support for new architectures such as Inkling, making it easier for developers to deploy high-performance LLMs. The flexible attention backends and KV offloading enhancements improve efficiency and scalability for production environments. The Inkling family includes base modeling, piecewise CUDA graph support, Hopper FA4 relative attention, MTP=1 speculative decoding, LoRA, and ModelOpt NVFP4 quantization. DeepSeek-V4 optimizations include a specialized routing kernel \(2.94% E2E TPOT improvement\), fused\_topk\_bias \(1.5–2x kernel speedup\), and two-stage compressor for ROCm.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source high-throughput LLM inference engine that supports a wide range of models and hardware accelerators. This release, with 411 commits from 212 contributors, is a substantial update that adds new model families and performance improvements. Key concepts include FlashAttention for efficient attention computation, speculative decoding for faster generation, and quantization techniques like NVFP4 to reduce memory footprint.

<details><summary>References</summary>
<ul>
<li><a href="https://learnaivisually.com/ai-explained/vllm-v0-20-fa4-packing">vLLM v0.20 — FlashAttention 4 packing — What does it mean?</a></li>
<li><a href="https://docs.vllm.ai/projects/vllm-omni/en/latest/user_guide/quantization/modelopt/">ModelOpt - vLLM-Omni</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#open-source`, `#performance optimization`, `#DeepSeek-V4`

---

<a id="item-3"></a>
## [Android May Restrict On-Device ADB Access](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

According to a high-scoring report, Android is considering restricting on-device ADB \(Android Debug Bridge\) access, which would limit the ability to debug and control devices directly from the device itself. This change has sparked significant debate in the developer community. This restriction could significantly impact Android developers and power users who rely on ADB for debugging, app testing, and automated tasks. It represents a trade-off between security improvements and developer freedom, potentially making certain workflows more cumbersome. The proposed change targets on-device ADB \(Wi-Fi or localhost\), not USB ADB, and requires both developer options and remote ADB to be enabled to be exploited. Some community members suggest alternatives like restricting to specific IP ranges rather than blocking entirely.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: Android Debug Bridge \(ADB\) is a command-line tool that allows developers to communicate with Android devices for debugging, file transfer, and running shell commands. It can be used over USB or TCP/IP, with on-device ADB enabling wireless debugging without a computer. Google has been gradually tightening security on Android, and this move is seen as part of that trend.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**Discussion**: The community comments reveal mixed reactions: some argue the attack vector is unrealistic because it requires multiple settings to be enabled, while others see it as a step toward further restricting user control. A developer using remote ADB via VPN expressed concern about exposing ADB on public Wi-Fi but hoped for granular controls rather than a blanket ban.

**Tags**: `#Android`, `#ADB`, `#Developer Tools`, `#Security`, `#Google`

---

<a id="item-4"></a>
## [Open-Weight AI&\#x27;s Kubernetes Moment](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

An article argues that open-weight AI models are becoming the industry standard, following the same trajectory as Kubernetes in cloud infrastructure, with implications for model governance and inference pricing. This shift could democratize AI access, reduce vendor lock-in, and stabilize inference pricing by providing a baseline, similarly to how Kubernetes enabled multi-cloud portability. However, it also raises governance challenges, such as the feasibility of banning models by origin. The analogy highlights that once an open platform becomes the center of gravity, no single vendor can match the combined innovation rate. Community comments note that tokenomics \(pricing per token\) has been opaque and seesaw-like, and that open-weight models provide a sanity baseline for inference costs.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: An open-weight model is an AI model whose trained parameters \(weights\) are publicly released, allowing anyone to download and run it. Inference cost is the ongoing compute expense of running a model in production. Kubernetes is an open-source container orchestration system that became the de facto standard for cloud infrastructure, enabling portability and innovation across vendors.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.cloudzero.com/blog/inference-cost/">Your Guide To Inference Cost (And Make It A Margin Advantage)</a></li>

</ul>
</details>

**Discussion**: Commenters debate the feasibility of banning Chinese models by origin, arguing weights are just numbers and cannot be assigned country tags. Others praise the article&\#x27;s core assertion about open platforms, discuss the opaque nature of tokenomics, and call for truly open models with public training data, akin to Kubernetes&\#x27; collaborative development model.

**Tags**: `#open-weight`, `#AI`, `#Kubernetes`, `#model governance`, `#inference pricing`

---

<a id="item-5"></a>
## [Claude Opus 5 Shows Strong Resistance to Prompt Injection](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny reported that Anthropic&\#x27;s Claude Opus 5 is the least prompt injectable model yet, based on prompt injection evaluations and red teaming documented in its system card. This marks significant progress in LLM security against prompt injection, a critical vulnerability that has plagued AI systems. Improved resistance enhances trust and safety in deploying LLMs for real-world applications. The claim is supported by evaluations and red teaming results buried in the Claude Opus 5 system card \(page 73\). Anthropic also noted that Opus 5 improved at finding vulnerabilities but deliberately avoided training on exploitation.

rss · Simon Willison · Jul 25, 00:42

**Background**: Prompt injection is a security vulnerability where malicious inputs override a model&\#x27;s intended instructions, causing unintended behavior. It has been a major challenge for LLMs like Claude, especially as models gain capabilities like web browsing. Red teaming is an adversarial testing process used to uncover such vulnerabilities before deployment. System cards document safety evaluations and responsible deployment decisions for AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection - OWASP Foundation</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-6"></a>
## [AMD Faces Software and Production Hurdles to Break CUDA Moat](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

AMD has unveiled its Helios AI rack with MI455X GPUs and introduced agentic kernel generation \(GEAK\) to improve software quality, but faces significant production ramp difficulties and instability in internal clusters, with financial engineering offering up to 105% discounts. This matters because AMD&\#x27;s ability to compete with NVIDIA&\#x27;s dominant CUDA ecosystem depends on overcoming these software quality and production challenges, which could provide a viable alternative for AI workloads and reduce reliance on NVIDIA hardware. AMD&\#x27;s GEAK \(Generating Efficient AI-Centric Kernels\) is an agentic framework for automatic GPU kernel optimization using multi-agent systems and a self-improving knowledge base, but the MI455X&\#x27;s Infinity Fabric bandwidth \(896 GB/s\) is significantly lower than NVIDIA&\#x27;s NVLink 6 \(3.6 TB/s\), and internal development clusters are reportedly unstable.

rss · Semianalysis · Jul 25, 00:33

**Background**: NVIDIA&\#x27;s CUDA platform has been the leading software ecosystem for GPU computing, providing comprehensive libraries and tools that lock developers into NVIDIA hardware. AMD&\#x27;s open-source alternative ROCm has historically lagged in software maturity and developer support. Agentic kernel generation aims to automate optimization and reduce manual effort to match CUDA performance on AMD GPUs. The Helios MI455X is AMD&\#x27;s latest high-end AI accelerator, but its production ramp has been challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/AMD-AGI/GEAK">GitHub - AMD-AGI/GEAK: Generating Efficient AI-Centric ...</a></li>
<li><a href="https://rocm.blogs.amd.com/artificial-intelligence/kernel-optimization-agent/README.html">GEAK V3: Agent-Driven, Repository-Level GPU Kernel ...</a></li>
<li><a href="https://introl.com/blog/amd-helios-mi455x-nvidia-competition-ces-2026">AMD Helios Challenges NVIDIA: The MI 455 X and the... | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#CUDA`, `#GPU`, `#AI hardware`, `#software ecosystem`

---

<a id="item-7"></a>
## [China fines Ctrip $7.6 billion for antitrust abuse](https://www.xinhuanet.com/fortune/20260725/693124245aa44d2bbc7520b7a0c244ea/c.html) ⭐️ 8.0/10

China&\#x27;s State Administration for Market Regulation fined Ctrip 51.79 billion yuan \($7.6 billion\) for abusing its dominant market position, including confiscating illegal gains of 1.658 billion yuan and imposing a fine of 3.521 billion yuan. This is one of the largest antitrust fines ever imposed on a Chinese tech company, signaling intensified regulatory scrutiny on platform monopolies and setting a precedent for fair competition in China&\#x27;s online travel market. The regulator also ordered Ctrip to cease its illegal practices and refund 122 million yuan in mandatory order reserves withheld from hotel operators, and required the company to implement comprehensive corrective measures.

telegram · zaihuapd · Jul 25, 02:24

**Background**: Abuse of market dominance refers to an operator with a dominant market position engaging in activities that exclude or restrict competition, violating China&\#x27;s Anti-Monopoly Law. The Anti-Monopoly Law prohibits such behavior, and the State Administration for Market Regulation has issued specific regulations to enforce these provisions. Ctrip, as the largest online travel platform in China, controls a significant share of the market for hotel booking and travel services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.samr.gov.cn/zw/zfxxgk/fdzdgknr/xwxcs/art/2023/art_78e487fb7b464e79880fdc8216c08c4c.html">《禁止滥用市场支配地位行为规定》解读</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#regulation`, `#Ctrip`, `#China`, `#tech industry`

---

<a id="item-8"></a>
## [Apple Lobbies Trump to Use Chinese Memory Chips, Micron Objects](https://www.wsj.com/tech/trump-apple-micron-china-chips-784bbd3d) ⭐️ 8.0/10

Apple CEO Tim Cook and other executives have recently lobbied the Trump administration to allow the use of memory chips from Chinese manufacturers CXMT and YMTC in products sold outside the U.S., but Micron Technology is actively opposing this move. This lobbying effort highlights the tension between cost reduction and national security in the global tech supply chain, and could reshape the memory chip market if approved, affecting both U.S. and Chinese chipmakers. Apple is targeting Chinese DRAM maker CXMT and NAND flash maker YMTC, aiming to reduce costs for non-U.S. market products. The Trump administration faces pressure from both Apple and its key supplier Micron, which opposes the use of Chinese chips.

telegram · zaihuapd · Jul 25, 04:02

**Background**: Memory chips are essential components in electronic devices, with DRAM used for temporary data storage and NAND flash for long-term storage. Chinese companies CXMT and YMTC have emerged as major players in these markets, challenging incumbents like Micron and Samsung. The U.S. has imposed export controls on advanced chips to China, but Apple&\#x27;s proposal involves using Chinese chips only in overseas products.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/%E9%95%BF%E9%91%AB%E5%AD%98%E5%82%A8">长鑫存储 - 维基百科，自由的百科全书</a></li>
<li><a href="http://m.tetegu.com/gainiangu/changjiangchunchu/">长 江 存 储 概念股- 长 江 存 储 概念股龙头 - 特特股</a></li>

</ul>
</details>

**Tags**: `#苹果`, `#美光`, `#存储芯片`, `#中美科技竞争`, `#供应链`

---