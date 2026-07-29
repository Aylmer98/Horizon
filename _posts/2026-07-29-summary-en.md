---
layout: default
title: "Horizon Summary: 2026-07-29 (EN)"
date: 2026-07-29
lang: en
---

> From 43 items, 10 important content pieces were selected

---

1. [Open-source engine runs Gemma 4 26B in 2GB RAM on Mac](#item-1) ⭐️ 9.0/10
2. [AI worms self-propagate through Microsoft Copilot for Word](#item-2) ⭐️ 9.0/10
3. [Moonshot AI raises $3.5B at $35B valuation, driven by Kimi K3](#item-3) ⭐️ 9.0/10
4. [Mitchell Hashimoto Launches Superlogical for Terminal Apps on libghostty](#item-4) ⭐️ 8.0/10
5. [Kimi Launches K3-256k: Cheaper Model with 256k Context](#item-5) ⭐️ 8.0/10
6. [LLMs Fail to Reliably Follow Long Policy Documents, Study Finds](#item-6) ⭐️ 8.0/10
7. [Matthew Green on Post-Quantum Crypto Shift and AI Cryptanalysis](#item-7) ⭐️ 8.0/10
8. [Vendor-agnostic ML inference on edge with Vulkan and ncnn](#item-8) ⭐️ 8.0/10
9. [Claude shared chats, artifacts indexed by Google; Anthropic says by design](#item-9) ⭐️ 8.0/10
10. [Hugging Face Widely Used to Generate Deepfake Nudes, Report Finds](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Open-source engine runs Gemma 4 26B in 2GB RAM on Mac](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

An open-source inference engine called TurboFieldfare, written in Swift and Metal, allows running the 4-bit quantized Gemma 4 26B-A4B-IT model on any M-series Mac using only about 2 GB of RAM by streaming routed experts from SSD. This breakthrough enables running 14 GB models on memory-constrained devices like 8 GB Macs, significantly expanding the reach of on-device AI. It demonstrates a practical approach to large model inference without expensive hardware upgrades. TurboFieldfare uses a small expert cache and bounded parallel pread to overlap SSD reads with GPU computation, achieving 5–6 tok/s on an 8 GB M2 MacBook Air and 31–35 tok/s on an M5 MacBook Pro. It also includes an experimental OpenAI-compatible local server with streaming and tool call support.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Large language models like Gemma 4 use a Mixture-of-Experts \(MoE\) architecture, where only a subset of expert networks is activated per token, allowing efficient computation. 4-bit quantization reduces model weights from 32-bit to 4-bit, shrinking size with minimal quality loss. The KV cache stores key-value vectors from previous tokens, enabling faster generation but consuming significant memory. By keeping shared layers and KV cache in RAM and streaming experts from SSD on demand, TurboFieldfare dramatically lowers memory requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/mixture-of-experts/">What Is Mixture of Experts (MoE) and How It Works? - NVIDIA</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project&\#x27;s novelty, with some noting it&\#x27;s the second time seeing such an approach on HN. Technical discussions included comparisons to plain mmap in llama.cpp, with the author clarifying that TurboFieldfare explicitly synchronizes SSD reads with inference. A user on macOS 15 shared a workaround to compile the project, highlighting the prefill speedup benefit. Overall sentiment was positive, with users expressing interest in broader platform support.

**Tags**: `#llm`, `#inference`, `#Mac`, `#on-device AI`, `#open-source`

---

<a id="item-2"></a>
## [AI worms self-propagate through Microsoft Copilot for Word](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 9.0/10

Researchers have demonstrated a new class of adversarial attack where prompt injections in documents cause AI agents like Microsoft Copilot to propagate worms, automatically spreading malicious instructions to new documents via email or sharing. This reveals a fundamental security vulnerability in LLM-integrated applications where instructions and data are conflated, potentially allowing self-replicating malware that exploits the trust users place in AI assistants. The attack, discovered by Håkon Måløy, uses indirect prompt injection hidden in document text, such as white-on-white text, to hijack Copilot&\#x27;s behavior. At the time of publication, no robust mitigation is available.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection attacks exploit the fact that large language models \(LLMs\) cannot distinguish between user instructions and data within a prompt. In this case, Copilot for Word reads documents and may treat embedded instructions as commands. This is similar to SQL injection but for AI agents, and it undermines the security of LLM-based applications that process untrusted content.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.15759v1">Securing AI Agents Against Prompt Injection Attacks:</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection - OWASP Foundation</a></li>

</ul>
</details>

**Discussion**: Commenters express alarm, noting that as users grant more access to agents, such attacks will worsen. Some point out that white text tricks still work, and the fundamental issue of mixing instructions with data may be impossible to fix.

**Tags**: `#AI security`, `#adversarial attacks`, `#LLM`, `#Copilot`, `#worm`

---

<a id="item-3"></a>
## [Moonshot AI raises $3.5B at $35B valuation, driven by Kimi K3](https://www.bloomberg.com/news/articles/2026-07-29/china-s-moonshot-ai-passes-funding-goal-to-hit-35-billion-value) ⭐️ 9.0/10

Moonshot AI completed a $3.5 billion funding round, far exceeding its $1-2 billion target, reaching a $35 billion post-money valuation. The raise was propelled by its Kimi K3 model, which approaches frontier AI capabilities and triggered a &\#x27;DeepSeek moment&\#x27; in the industry. This massive funding round underscores the rapid maturation of Chinese AI startups and the growing global impact of open-weight frontier models. It signals intensifying competition with Western AI labs and could accelerate the commoditization of advanced AI capabilities. Moonshot AI has already initiated a new funding round at a $50 billion pre-money valuation and plans an IPO in Hong Kong as early as this year. The Kimi K3 model uses architectural innovations such as Kimi Delta Attention and Attention Residuals, and its weights were released open-source on July 27, 2026.

telegram · zaihuapd · Jul 29, 10:12

**Background**: Moonshot AI is a Chinese AI startup focused on developing large language models. The Kimi K3 is its flagship open-weight model, released in July 2026, which rivals frontier models from OpenAI and Anthropic. The &\#x27;DeepSeek moment&\#x27; refers to a watershed event where open-source AI models closed the performance gap with proprietary models, exemplified earlier by DeepSeek-R1.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://greylock.com/greymatter/the-deepseek-moment/">The DeepSeek Moment | Greylock</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#Moonshot AI`, `#China`, `#Kimi K3`

---

<a id="item-4"></a>
## [Mitchell Hashimoto Launches Superlogical for Terminal Apps on libghostty](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto has announced Superlogical, a new company that will build terminal applications on top of the open-source libghostty library, which was extracted from his earlier Ghostty terminal emulator. This move establishes a sustainable business model around an open-source terminal foundation, potentially driving broader innovation in terminal applications and fostering a community of developers leveraging the same core library. Superlogical will consume libghostty exactly as any other user, and the company commits to upstreaming shared improvements back to the project. Ghostty itself has been transferred to a non-profit organization to ensure its independence.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: libghostty is a cross-platform, zero-dependency library \(no libc\) for parsing terminal sequences and maintaining terminal state, extracted from the Ghostty terminal emulator. Ghostty is a fast, GPU-accelerated terminal emulator created by Mitchell Hashimoto, co-founder of HashiCorp. By providing a shared terminal core, libghostty aims to reduce duplication and enable a new ecosystem of terminal applications.

<details><summary>References</summary>
<ul>
<li><a href="https://bytes.dev/archives/427">Bytes #427 - Libghostty sneak peek</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty -org/ ghostty : Ghostty is a fast, feature-rich, and...</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**Discussion**: Commenter simonw praised the ownership transfer of Ghostty to a non-profit and the upstream commitment. Some commenters drew parallels to old component technologies like OLE/COM, while others criticized the title as clickbait. Overall, the sentiment was positive about the open-source foundation and business model.

**Tags**: `#terminal`, `#open-source`, `#mitchell-hashimoto`, `#ghostty`, `#superlogical`

---

<a id="item-5"></a>
## [Kimi Launches K3-256k: Cheaper Model with 256k Context](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Moonshot AI announced the Kimi K3-256k model, a cost-reduced variant of their K3-1M model that offers a 256k token context window at roughly half the price, while maintaining equivalent performance within that context limit. This move addresses a key pain point in the AI industry: balancing large context capabilities with cost. By offering a cheaper 256k option, Kimi makes long-context processing more accessible for users who don&\#x27;t need the full 1M context, potentially setting a trend for tiered pricing based on context size. According to the announcement, the K3-256k consumes about half the quota of the original K3-1M model when used within the 256k context window. Some community members suspect that infrastructure pressures may have led to degraded quality in recent Kimi models, though this has not been confirmed.

hackernews · monneyboi · Jul 29, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49101852)

**Background**: A context window in large language models determines how much text the model can process at once. Kimi is a series of AI models developed by Moonshot AI, a Chinese company, known for its long-context capabilities. The original K3 model featured a 1M token context window, which is among the longest available, but comes at a higher cost. The new K3-256k offers a reduced yet still substantial context window at a lower price point.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/context-window">What is a context window? - IBM</a></li>
<li><a href="https://medium.com/algomart/kimi-llm-models-why-moonshot-ais-long-context-models-are-getting-attention-12663e0a2351">Kimi LLM Models: Why Moonshot AI ’s Long-Context Models... | Medium</a></li>

</ul>
</details>

**Discussion**: Community sentiment is generally positive, with users appreciating the cost savings and finding the 256k context sufficient for most tasks. However, some users expressed concerns about recent model quality degradation, speculating that Kimi may have been using quantized models to reduce infrastructure load.

**Tags**: `#AI`, `#models`, `#context-window`, `#pricing`, `#infrastructure`

---

<a id="item-6"></a>
## [LLMs Fail to Reliably Follow Long Policy Documents, Study Finds](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new study \(arXiv: 2607.25398\) demonstrates that large language models \(LLMs\) fail to consistently follow long policy documents, even those with extended context windows up to 1 million tokens. This finding challenges the assumption that scaling context window size alone can ensure reliable agentic behavior, highlighting a critical obstacle to deploying LLMs as autonomous agents governed by complex policies. The research attributes failures to issues with KV cache quantization, poor sampling, and fundamental limitations in working memory and reasoning depth, noting that models often ignore earlier instructions after extended interaction.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: Long-context models claim support for millions of tokens, but studies show quality degrades beyond a few thousand tokens due to attention dilution and memory constraints. Agent governance aims to ensure AI agents follow corporate policies, but this research suggests current LLMs cannot reliably adhere to long rulebooks without additional mechanisms like runtime enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.17129v1?trk=article-ssr-frontend-pulse_little-text-block">Thus Spake Long - Context Large Language Model</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/ai-agents/governance-security-across-organization">Govern and secure AI agents AI agents across the organization - Cloud Adoption Framework | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree with the findings, citing personal experiences with Claude and GPT models ignoring long instructions. Some note that local inference could improve behavior, while others argue that humans also struggle with long policy documents, suggesting the benchmark may measure a hard problem.

**Tags**: `#LLMs`, `#long-context`, `#AI safety`, `#agent governance`

---

<a id="item-7"></a>
## [Matthew Green on Post-Quantum Crypto Shift and AI Cryptanalysis](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Matthew Green highlights the historic transition from traditional public-key algorithms \(RSA, ECC\) to post-quantum cryptography, and suggests this is an opportune moment for AI to advance cryptanalysis, potentially validating or undermining new cryptographic problems. This commentary connects two critical trends—post-quantum cryptography migration and AI progress—suggesting a synergistic opportunity. If AI can assist in cryptanalysis, it could either strengthen confidence in new schemes or reveal vulnerabilities, with major implications for cybersecurity. Green references HAWK as a post-quantum signature scheme under NIST standardization, and mentions Impagliazzo&\#x27;s &\#x27;Minicrypt&\#x27; world where only private-key cryptography is possible. He notes that unless AI undermines all hard problems, the timing for AI-driven cryptanalysis is perfect.

rss · Simon Willison · Jul 29, 18:18

**Background**: Post-quantum cryptography \(PQC\) develops systems secure against both classical and quantum computers. NIST is standardizing PQC algorithms to replace RSA and ECC, which quantum computers could break. Impagliazzo&\#x27;s Five Worlds include Minicrypt, where only one-way functions and symmetric cryptography exist, making public-key crypto impossible.

<details><summary>References</summary>
<ul>
<li><a href="https://hawk-sign.info/">Hawk</a></li>
<li><a href="https://www.csoonline.com/article/4202920/mythos-takes-its-first-shot-at-post-quantum-cryptography.html">Mythos takes its first shot at post-quantum cryptography</a></li>
<li><a href="https://www.nist.gov/pqc">Post-quantum cryptography | NIST</a></li>

</ul>
</details>

**Tags**: `#post-quantum cryptography`, `#AI`, `#cryptanalysis`, `#public-key algorithms`, `#Matthew Green`

---

<a id="item-8"></a>
## [Vendor-agnostic ML inference on edge with Vulkan and ncnn](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

A developer from PostSlate shares a practical approach using ncnn&\#x27;s Vulkan backend for on-device ML inference across diverse GPUs, achieving 10x speedup \(e.g., ArcFace from 30 ms to 3 ms\) compared to CPU-based ONNX. This solution solves a critical production challenge: running ML inference on any GPU without vendor-specific runtimes, enabling truly cross-platform edge AI applications. The approach uses ncnn framework with Vulkan GPU backend, converting ONNX models \(e.g., ArcFace 174 MB\) to ncnn format \(87 MB at fp16\), and leverages Vulkan drivers already present on all target devices.

reddit · r/MachineLearning · /u/ppchaos · Jul 29, 10:22

**Background**: ncnn is a high-performance neural network inference framework optimized for mobile and edge devices, developed by Tencent, supporting CPU and Vulkan GPU backends without third-party dependencies. Vulkan is a cross-platform GPU API that runs on NVIDIA, AMD, Intel, and Apple GPUs, making it ideal for vendor-agnostic inference. ONNX is an open format for ML models, but its CPU-only inference is often slower than GPU-accelerated alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Tencent/ncnn">GitHub - Tencent/ncnn: ncnn is a high-performance neural ...</a></li>
<li><a href="https://www.insightface.ai/research/scrfd">InsightFace SCRFD Paper Explained: Efficient Face Detection</a></li>
<li><a href="https://learnopencv.com/face-recognition-with-arcface/">Face Recognition with ArcFace Machine Learning Model ...</a></li>

</ul>
</details>

**Tags**: `#ML inference`, `#Vulkan`, `#edge computing`, `#cross-platform`, `#ncnn`

---

<a id="item-9"></a>
## [Claude shared chats, artifacts indexed by Google; Anthropic says by design](https://thenextweb.com/news/claude-shared-chats-artifacts-google-search-indexed) ⭐️ 8.0/10

Claude shared conversation and Artifacts links created by users have been indexed by Google search, exposing sensitive information such as medical records and company files. Anthropic confirmed no system breach and stated the indexing is by design because links are publicly shareable. This incident highlights significant privacy risks in AI tool design where shared links are assumed private but can be crawled by search engines. It affects all Claude users who shared links, potentially exposing confidential data to anyone on the internet. Anthropic blocked new indexing on Monday afternoon, but previously indexed links remain accessible. Users can revoke shared links in settings. Similar incidents occurred with Claude in September 2025, and with ChatGPT and Grok previously.

telegram · zaihuapd · Jul 29, 02:40

**Background**: Claude Artifacts is a feature that generates interactive code previews and applications, allowing users to share creations via public links. When a link is set to &\#x27;anyone with the link,&\#x27; it can be discovered by search engine crawlers if the page is publicly accessible. This is a common issue with shared links across platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/9487310-what-are-artifacts-and-how-do-i-use-them">What are artifacts and how do I use them? | Claude Help Center</a></li>
<li><a href="https://support.google.com/drive/thread/83160241/do-search-engines-index-the-files-which-are-shared-as-anyone-with-the-link?hl=en">Do search engines index the files which are shared as &quot;anyone with the link&quot; ? - Google Drive Community</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#AI safety`, `#Claude`, `#security`

---

<a id="item-10"></a>
## [Hugging Face Widely Used to Generate Deepfake Nudes, Report Finds](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

A report by European non-profit AI Forensics released on July 28 reveals that Hugging Face&\#x27;s top nine image-editing models include seven that can easily strip clothing from women with simple prompts, and a honeypot set up by the organization received over 1,000 requests in seven days, 73% of which were sexual and nearly 7% targeted children. This report highlights severe safety gaps in the Hugging Face platform, as it is widely used for non-consensual deepfake pornography with minimal protective measures, raising urgent ethical and regulatory concerns for the open-source AI community. The report states that Hugging Face has almost no platform-level safeguards against generating non-consensual intimate images, despite its policy prohibiting such content and child sexual abuse material; researchers did not need carefully crafted prompts to bypass filters.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a popular American company and open-source platform where machine learning models and datasets are shared. A honeypot is a cybersecurity mechanism that acts as a decoy to detect unauthorized activity. Deepfake technology uses AI to create realistic but fake images or videos, often used maliciously to generate non-consensual pornography.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Honeypot_%28computing%29">Honeypot (computing) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI伦理`, `#深度伪造`, `#Hugging Face`, `#内容安全`, `#开源模型`

---