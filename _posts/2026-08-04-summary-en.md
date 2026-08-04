---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 41 items, 14 important content pieces were selected

---

1. [White House reverses on open-source AI curbs amid Silicon Valley split](#item-1) ⭐️ 8.5/10
2. [Mistral unveils Shieldstral 3B, open-weights multimodal safety classifier](#item-2) ⭐️ 8.0/10
3. [New algorithm and color space for generating diverse skin tones](#item-3) ⭐️ 8.0/10
4. [Waymo Opens Driverless Ride-Hailing to the Public in Dallas](#item-4) ⭐️ 8.0/10
5. [Troy Hunt: FedEx&\#x27;s Confusing Emails Fuel Phishing Problem](#item-5) ⭐️ 8.0/10
6. [DeepSeek V4 Flash Achieves 150+ Tokens/s on Single AMD MI300X](#item-6) ⭐️ 8.0/10
7. [Keyv npm Package Compromised in Active Shai-Hulud Supply Chain Attack](#item-7) ⭐️ 8.0/10
8. [Xbox Outage Blocks Disc Games, Reigniting Digital Ownership Debate](#item-8) ⭐️ 8.0/10
9. [Engineering AI Harnesses for Self-Improvement](#item-9) ⭐️ 8.0/10
10. [MiniMax-H3 omni-modal model gets MLX port for Apple Silicon](#item-10) ⭐️ 8.0/10
11. [Huawei Chief Scientist Warns Nvidia Chip Scaling Will Hit Physical Limits](#item-11) ⭐️ 8.0/10
12. [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](#item-12) ⭐️ 8.0/10
13. [Trump Administration Drafts Import Ban on Chinese Optical Modules](#item-13) ⭐️ 8.0/10
14. [China issues first mandatory national standard for L3/L4 autonomous driving](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [White House reverses on open-source AI curbs amid Silicon Valley split](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.5/10

The White House has reportedly abandoned plans to restrict Chinese open-source AI models and instead shifted focus to boosting U.S. AI competitiveness. On August 4, it invited tech companies to discuss a new framework that would require cybersecurity reviews before model release. This policy reversal could reshape U.S.-China tech competition and the global AI landscape. The deep rift between AI labs and platform companies reveals fundamental disagreements over whether open-source AI poses a national security threat. The reversal followed strong opposition from Silicon Valley, including Nvidia CEO Jensen Huang, who defended open source and formed a security alliance with over 230 members. The trigger was the performance of China&\#x27;s Kimi model, which reportedly rivals OpenAI&\#x27;s top models.

telegram · zaihuapd · Aug 4, 15:22

**Background**: Open-source AI models are publicly released with weights that anyone can use and modify, sparking debates over whether they enable misuse or accelerate innovation. Kimi is a series of large language models developed by Chinese company Moonshot AI; its latest K3 model reportedly has 2.8 trillion parameters and a 1M-token context window. The White House&\#x27;s internal debate reflects broader tensions between national security and AI competitiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_%28chatbot%29">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/">Kimi API Platform</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#Open source`, `#Geopolitics`, `#Technology policy`, `#Artificial Intelligence`

---

<a id="item-2"></a>
## [Mistral unveils Shieldstral 3B, open-weights multimodal safety classifier](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral unveiled Shieldstral, an open-weights 3B multimodal safety classifier for content moderation. The model is fine-tuned with LoRA on the language model parameters and is available on Hugging Face. Shieldstral offers a cost-effective, locally deployable moderation solution, which could benefit platforms struggling with content moderation responsibilities. Its strong performance relative to size suggests that smaller, task-specific models can compete with much larger systems. The model frames content moderation as a policy-adaptive yes/no question-answering task, and reportedly matches or outperforms models nearly seven times larger on text safety benchmarks. It is open-weights, which means the final parameters are shared, but training data and code may not be fully released.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**Background**: Open-weights models are shared so anyone can use and customize them on their own infrastructure, but they are distinct from fully open-source AI systems that also release training data and code. Multimodal content moderation automatically analyzes text, images, audio, and video to detect policy-violating material.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral . | Mistral AI</a></li>
<li><a href="https://arxiv.org/html/2607.25857">Shieldstral</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_artificial_intelligence">Open-weight artificial intelligence</a></li>

</ul>
</details>

**Discussion**: Commenters questioned customizability, with one asking whether the model can apply arbitrary rulesets without retraining. Others joked about the name \(&\#x27;Safestral&\#x27;\) and noted a possible strategic shift toward smaller, fine-tuned models, while a developer called it a &\#x27;realistic, cost effective solution&\#x27; for content moderation and another asked how it compares to OpenAI&\#x27;s omni-moderation.

**Tags**: `#AI`, `#moderation`, `#open-source`, `#Mistral`, `#multimodal`

---

<a id="item-3"></a>
## [New algorithm and color space for generating diverse skin tones](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

A developer published an interactive page introducing a custom color space and procedural generation algorithm for selecting diverse, plausible skin tones for digital art and game development. The project includes a color picker, multiple JavaScript demos, and detailed explanations of the underlying equations and properties. This work addresses a practical gap in digital art and game development tools, where choosing a diverse but realistic set of skin tones is often tedious and unintuitive. It also brings algorithmic thinking to an area with representation implications, potentially helping creators build more inclusive content. According to community comments, the method may involve dimensionality reduction similar to PCA, plus manual function fitting on U-space vectors. The author notes the methodology might be shaky and includes a Future Work section, and some commenters observed that the model can produce odd colors like green, blue, or purple in certain cases.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**Background**: Skin color is a complex mix of physics and human perception, strongly influenced by lighting and many other factors. Color science research, such as Pantone SkinTones and perceptually uniform spaces like Oklab, has tried to model these variations, and with high saturation, skin tones of any race tend toward orange.

**Discussion**: Commenters were generally enthusiastic, praising the presentation and the clever function-fitting idea after initially expecting a PCA-based reduction. Several added valuable context, such as the resemblance to a crescent shape seen in foundation shade distributions in Oklab, references to Pantone SkinTones, and the observation that high saturation makes all skin appear orange; one commenter also reported seeing green, blue, and purple colors in some samples.

**Tags**: `#color science`, `#skin tones`, `#procedural generation`, `#digital art`, `#game development`

---

<a id="item-4"></a>
## [Waymo Opens Driverless Ride-Hailing to the Public in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo has expanded its fully driverless ride-hailing service to the public in Dallas, Texas, one of the nation&\#x27;s largest and most car-centric metro areas. The service is now available to all riders in the Dallas-Fort Worth area. This marks a major expansion of autonomous ride-hailing into a low-density, sprawling metroplex with limited public transit, testing whether AVs can thrive outside dense urban cores. If successful, it could accelerate AV adoption and influence urban planning, housing, and transportation policy. Waymo&\#x27;s service is fully driverless, with the Waymo Driver system in control from pickup to destination and no safety driver onboard. The Dallas-Fort Worth launch is a notable stress test because the region is known for low-density sprawl and a car-heavy culture, unlike Waymo&\#x27;s earlier operating areas.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**Background**: Waymo is the autonomous-vehicle subsidiary of Alphabet, developing the Waymo Driver system, which is designed as Level 4 fully autonomous technology. The company launched the world&\#x27;s first autonomous ride-hailing service, Waymo One, in Phoenix in 2018, and has since expanded to other U.S. cities. Its service is available 24/7 and has completed more than 20 million rides with a reported 93% rider satisfaction rate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride - Hail</a></li>
<li><a href="https://waymo.com/waymo-driver/">Self-Driving Car Technology for a Reliable Ride - Waymo Driver</a></li>

</ul>
</details>

**Discussion**: Comments are largely positive, with riders noting Waymos feel normal and cause far fewer incidents than human drivers, though they occasionally get stuck. One real-estate developer argues driverless cars could serve as a highly effective, overlooked affordable-housing policy, while another commenter raises unresolved legal questions about traffic fines, insurance, and criminal liability in autonomous crashes.

**Tags**: `#Waymo`, `#autonomous vehicles`, `#transportation`, `#urban mobility`

---

<a id="item-5"></a>
## [Troy Hunt: FedEx&\#x27;s Confusing Emails Fuel Phishing Problem](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

Troy Hunt, a well-known security researcher, criticized FedEx&\#x27;s legitimate email practices, arguing they look so similar to phishing that users can&\#x27;t tell them apart. This erodes people&\#x27;s ability to identify scam messages. Because phishing remains a top cybersecurity threat, legitimate companies sending confusing, unauthenticated-style emails undermine user vigilance and make phishing attacks more effective. Hunt points out that FedEx emails often use generic sender names, odd links, and inconsistent formatting — the same cues used by phishing campaigns. He argues that without strong email authentication like DMARC, users have no reliable signal to distinguish real from fake.

hackernews · stymaar · Aug 4, 21:09 · [Discussion](https://news.ycombinator.com/item?id=49175192)

**Background**: Phishing attacks often rely on spoofed emails that impersonate trusted brands like FedEx. Email authentication protocols like SPF, DKIM, and DMARC help receivers verify that a message actually comes from the claimed domain, but they are not always enforced, leaving users to judge by appearance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://dmarc.org/overview/">Overview – dmarc.org</a></li>
<li><a href="https://abnormal.ai/glossary/email-spoofing">Email Spoofing: Types, Examples, and Prevention | Abnormal AI</a></li>

</ul>
</details>

**Discussion**: Commenters shared similar experiences, such as receiving legitimate FedEx customs notices that looked like scams and Google storage warnings using unfamiliar domains like c.gle. They also noted that the proliferation of new top-level domains and text-to-speech systems used by agencies like the IRS make phishing detection harder for non-technical users.

**Tags**: `#security`, `#phishing`, `#email`, `#ux`, `#fedex`

---

<a id="item-6"></a>
## [DeepSeek V4 Flash Achieves 150+ Tokens/s on Single AMD MI300X](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

A community project demonstrates DeepSeek V4 Flash, a 284B-parameter Mixture-of-Experts model, running efficiently on a single AMD MI300X GPU at over 150 tokens per second. This is achieved by trading the full 1M-token context window for a still-practical 256k tokens. Running a state-of-the-art MoE model on a single accelerator challenges the assumption that frontier inference requires NVIDIA hardware or multiple GPUs. It makes high-end reasoning models more accessible and highlights AMD&\#x27;s MI300X — with its large HBM capacity — as a viable platform for local AI inference. The MI300X is an OAM module with 192GB of HBM, and the practical 256k context configuration still fits in memory because DeepSeek V4 Flash&\#x27;s 256 MoE experts are natively MXFP4-quantized. The implementation builds on earlier work running the model on two MI300X GPUs, which is referenced in the project&\#x27;s readme.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**Background**: DeepSeek V4 Flash is an efficiency-optimized Mixture-of-Experts \(MoE\) model from DeepSeek with 284B total parameters but only 13B activated per token, supporting a 1M-token context window. MoE models activate only a subset of parameters for each token, which cuts compute cost dramatically while keeping a large total parameter count. The AMD MI300X provides 1.32x theoretical compute, 2.4x memory capacity, and 1.58x peak memory bandwidth versus NVIDIA&\#x27;s H100, making it attractive for memory-bound LLM inference.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://moreh.io/technical-report/moreh-vllm-performance-evaluation-deepseek-v3-r1-671b-on-amd-instinct-mi300x-gpus-250829/">Moreh vLLM Performance Evaluation: DeepSeek V3/R1 671B on AMD ...</a></li>

</ul>
</details>

**Discussion**: Discussion on Hacker News is broadly positive but highlights caveats: individual MI300X units are not readily purchasable outside an ~250K EUR 8-GPU box, and some point to the PCIe-based MI350P with 144GB as a more accessible alternative. Others note that prior work such as DwarfStar already ran the same model in less memory and wasn&\#x27;t cited, while the 256k context tradeoff is seen as practical since quality degrades toward the full 1M window.

**Tags**: `#AI/ML`, `#GPU inference`, `#DeepSeek`, `#AMD MI300X`, `#Mixture of Experts`

---

<a id="item-7"></a>
## [Keyv npm Package Compromised in Active Shai-Hulud Supply Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

A new wave of the Shai-Hulud worm is actively compromising npm packages, starting with keyv and cacheable, which are widely used in the Node.js ecosystem. The malware harvests developer credentials, publishes itself to writable npm packages, and plants execution hooks in GitHub repositories. Keyv alone is a dependency of over 1,700 npm projects, so this attack has a wide blast radius across the JavaScript/Node.js ecosystem. It is also the third major npm supply-chain attack in recent months, underscoring a growing threat pattern that affects developers and enterprises alike. According to JFrog Security Research, the worm harvests credentials and propagates by publishing itself to every writable npm package, and it plants execution hooks in GitHub repositories. The npm registry shows keyv&\#x27;s latest version 6.0.0 was published an hour ago, indicating the compromised release is very recent.

hackernews · cimi\_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**Background**: npm is the default package manager for Node.js, and packages are often installed automatically with their dependencies, which makes the ecosystem a prime target for supply-chain attacks. Shai-Hulud is a self-propagating worm that has previously compromised hundreds of npm packages, harvesting developer credentials. SecurityWeek notes it is the third major npm supply-chain attack, following the s1ngularity attack and the compromise of Josh Junon, a maintainer of packages with over 2.5 billion weekly downloads. A compromised upstream package can spread malware to any project that depends on it, often via install scripts that run automatically.

<details><summary>References</summary>
<ul>
<li><a href="https://research.jfrog.com/post/shai-hulud-is-back-august/">Major Shai Hulud campaign strikes npm again, affecting keyv and 400+ packages - JFrog Security Research</a></li>
<li><a href="https://www.securityweek.com/shai-hulud-supply-chain-attack-worm-used-to-steal-secrets-180-npm-packages-hit/">Shai - Hulud Supply Chain Attack : Worm Used to... - SecurityWeek</a></li>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely frustrated and cautious: several commenters call for killing or severely restricting pre-install and post-install hooks, which are a common vector for this kind of attack. Others share practical mitigation tips, such as setting &\#x27;min-release-age=5&\#x27; in .npmrc, and links to up-to-date documentation on npm supply-chain attack techniques. Some express worry about the fragility of the dependency system and the difficulty of cleaning up knock-on compromises.

**Tags**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#devops`

---

<a id="item-8"></a>
## [Xbox Outage Blocks Disc Games, Reigniting Digital Ownership Debate](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

A recent Xbox service outage left users unable to play games they owned on physical discs, because the console could not complete its required DRM verification with Microsoft&\#x27;s servers. The incident generated 594 community comments and became a flashpoint for debating DRM restrictions and the erosion of ownership in digital gaming. This episode shows that even &\#x27;physical&\#x27; game purchases are increasingly tied to online license checks, so a server outage can strip access to games consumers already paid for. It affects all gamers and reinforces ongoing industry debates about consumer rights, DRM, and the shift toward license-based ownership. On Xbox, DRM for disc games typically chains entitlement checks to the disc, the console, the user account, Microsoft&\#x27;s servers, and the &\#x27;Home Xbox&\#x27; setting, leaving offline play dependent on multiple conditions. Microsoft has quietly tweaked its DRM over time, but the platform remains a hybrid ecosystem where updates, account systems, and service availability still shape ownership.

hackernews · surprisetalk · Aug 4, 12:01 · [Discussion](https://news.ycombinator.com/item?id=49167448)

**Background**: DRM \(digital rights management\) is technology that restricts how digital content can be used, and game consoles use it to verify that a player actually owns a title. When you buy a game digitally, you are generally purchasing a license to access it under specific terms, not the software itself, and publishers can revoke or alter access with little warning. This has fueled initiatives such as the Stop Killing Games petition and broad concerns about the long-term viability of digital purchases across entertainment industries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.windowscentral.com/xbox-drm-explained">Xbox DRM explained: Setting a home console, console sharing, licenses, and more | Windows Central</a></li>
<li><a href="https://dataconomy.com/2025/08/28/digital-ownership-in-gaming-what-you-actually-own/">Digital Ownership In Gaming: What You Actually ‘own’ - Dataconomy</a></li>
<li><a href="https://www.strandmagazine.co.uk/single-post/do-we-own-the-games-we-play-a-look-into-what-digital-game-ownership-means">Do We Own the Games We Play? A Look into What Digital Game Ownership Means</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong frustration with the loss of true ownership: one user pointed out that older consoles like the GameCube allow offline play &\#x27;until I pass away,&\#x27; while another argued the real issue is ownership, not physical vs. digital, and listed rights such as reselling and passing games to children. Others noted that seventh-generation consoles handled this better by hosting multiplayer on consoles with still-working matchmaking servers. The overall mood is that modern DRM has made even disc-based games fragile and dependent on online infrastructure.

**Tags**: `#gaming`, `#DRM`, `#digital ownership`, `#Xbox`, `#outage`

---

<a id="item-9"></a>
## [Engineering AI Harnesses for Self-Improvement](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

In a July 2026 blog post, Lilian Weng explored how engineering the harness—tools, skills, and evaluation—enables AI systems to improve their own performance. The post generated substantial community engagement with 291 points and 64 comments debating implementation strategies. This shifts the focus of AI improvement from model weights to the surrounding harness, potentially enabling more sample-efficient self-improvement. It matters for engineering teams building agentic systems, where tooling, context, and evaluation design become critical levers for performance. The article covers fitness functions, tool optimization, and evaluation strategies for harnesses. Community comments highlight practical techniques such as reading production traces, enabling agents to write their own tools \(reducing context from 20k tokens across 15 calls to 800 tokens in one call\), and using eval/validation splits to prevent reward hacking.

hackernews · tosh · Aug 4, 06:17 · [Discussion](https://news.ycombinator.com/item?id=49164896)

**Background**: Harness engineering refers to designing the external scaffolding around an AI model—tools, context, instructions, and evaluation—to control and optimize its behavior, rather than modifying the model&\#x27;s weights. Recent work from OpenAI, Anthropic, and Martin Fowler has explored similar ideas, emphasizing that organizing information and writing effective tools are key to agent performance. The concept also connects to recursive self-improvement, where a system improves its own code or tools, a goal that has been central to AI research since its inception.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/harness-engineering/">Harness engineering: leveraging Codex in an agent-first world | OpenAI</a></li>
<li><a href="https://www.anthropic.com/engineering/writing-tools-for-agents">Writing effective tools for AI agents—using AI agents \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive and practical. bisonbear stressed the need for reliable fitness functions to optimize agent harnesses for large codebases; zby argued that training paradigms for prompts and code may be more sample-efficient than weight training; scosman shared success with auto-research on harnesses, requiring production traces and allowing agents to write their own tools; storus wondered when harnesses would generate their own RLHF/DPO training sets for LoRA fine-tuning. A lighter comment joked about the ongoing quest for the &\#x27;Torment Nexus&\#x27;.

**Tags**: `#AI agents`, `#harness engineering`, `#self-improvement`, `#tool optimization`, `#evaluation`

---

<a id="item-10"></a>
## [MiniMax-H3 omni-modal model gets MLX port for Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax released MiniMax-H3, an omni-modal generative system supporting text, images, audio, and video, two days before this report. A new Python package ports the model to MLX, and Simon Willison successfully ran it on an M5 Max MacBook Pro to generate a video clip. This enables developers and researchers to run state-of-the-art multimodal video generation locally on Apple Silicon, reducing dependence on cloud GPU services. It also highlights the rapidly growing ecosystem of MLX model ports that make advanced AI models more accessible. The model can generate up to 15-second video clips with native audio at up to 2K resolution. The experiment required about 115 GB of model files and took nearly 45 minutes to generate a single video on the M5 Max; audio output was poor without proper prompt guidance.

rss · Simon Willison · Aug 4, 19:10

**Background**: MLX is Apple&\#x27;s open-source array framework for machine learning on Apple silicon, optimized for the unified memory architecture and offering a NumPy-like API. Omni-modal models are AI systems that process multiple data modalities—text, images, audio, and video—within a single unified architecture. MiniMax-H3 is a general-purpose omni-modal generation model released by MiniMax and available with open weights.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://fal.ai/minimax-h3">MiniMax H3 - Open-Weights General-Purpose Multimodal Video Model | fal</a></li>

</ul>
</details>

**Tags**: `#MLX`, `#MiniMax-H3`, `#multimodal AI`, `#video generation`, `#Apple Silicon`

---

<a id="item-11"></a>
## [Huawei Chief Scientist Warns Nvidia Chip Scaling Will Hit Physical Limits](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 8.0/10

In a rare four-hour public interview in late July, Huawei chief semiconductor scientist Liao Heng warned that Nvidia&\#x27;s approach of scaling compute chips and high-bandwidth memory will eventually hit physical limits, and proposed Huawei&\#x27;s LogicFolding framework as an alternative path. The first phone chip using LogicFolding technology is expected to debut later this year. This warning from a top Huawei scientist signals that conventional chip scaling, long driven by Moore&\#x27;s Law, is nearing its end, and it positions Huawei&\#x27;s LogicFolding and Tau Scaling Law as a sanctions-resistant alternative. As the US-China semiconductor industry splits into separate ecosystems, this technology route could reshape competition in AI chips and advanced manufacturing. LogicFolding physically folds and stacks logic circuits into a dual-layer structure to shorten signal travel distance and reduce resistive and capacitive load, potentially achieving 1.4nm-class performance without EUV lithography and claiming a 55% higher transistor density. Liao Heng also noted that the US and Chinese semiconductor industries are diverging into two independent ecosystems, requiring complete manufacturing and supply capabilities for survival.

telegram · zaihuapd · Aug 4, 08:04

**Background**: Moore&\#x27;s Law, the observation that transistor density roughly doubles every couple of years, has been the engine of semiconductor progress for decades. As traditional scaling slows, chipmakers such as Nvidia have relied on larger dies and high-bandwidth memory to keep pushing performance. Huawei, cut off from advanced EUV lithography tools by US sanctions, unveiled the Tau Scaling Law and LogicFolding architecture at ISCAS 2026 as a way to continue improving chip performance without those tools.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/huawei-claims-sanctions-busting-breakthrough-with-1-4nm-class-chips-by-2031-claims-55-percent-higher-transistor-density-firm-claims-new-logicfolding-chip-architecture-can-bypass-euv-restrictions-introduces-tau-scaling-law-to-replace-moores-law">Huawei claims sanctions-busting breakthrough with 1.4nm-class chips by 2031, claims 55% higher transistor density — firm claims new LogicFolding chip architecture can bypass EUV restrictions, introduces &#x27;Tau Scaling Law&#x27; to replace Moore&#x27;s Law | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.huaweicentral.com/huawei-logicfolding-architecture-everything-you-need-to-know/">Huawei LogicFolding Architecture: Everything you need to know - Huawei Central</a></li>
<li><a href="https://timesofindia.indiatimes.com/technology/tech-news/explained-what-is-huaweis-logicfolding-tau-scaling-law-and-how-it-plans-to-build-1-4nm-chips-without-asml/articleshow/131314122.cms">Explained: What is Huawei&#x27;s LogicFolding, Tau Scaling Law, and how it plans to build 1.4nm chips without ASML - The Times of India</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#AI chips`, `#Huawei`, `#Nvidia`, `#physical limits`

---

<a id="item-12"></a>
## [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

Google has quietly assembled one of the largest infrastructure financing structures in history to deliver over $150 billion in AI chips to Anthropic, with total contracts worth about $200 billion. The special purpose vehicle Compute SPV completed its first transactions in June, acquiring about $35 billion in hardware, roughly 1 gigawatt of compute and 1 million TPUs. This is the largest financing mechanism ever created for AI infrastructure, letting Anthropic access massive computing power despite having no credit rating. The structure spreads risk across chipmakers, asset managers, and banks, and could set a new template for how AI companies fund data centers and chips. Google guarantees the data centers, Broadcom buys and helps finance the chips, while Apollo and Blackstone purchase the hardware and lease it back to Anthropic. The model borrows from manufacturer financing used by Boeing and GE to sell planes and engines, keeping tens of billions of dollars in AI hardware off any single company&\#x27;s balance sheet.

telegram · zaihuapd · Aug 4, 10:52

**Background**: A special purpose vehicle \(SPV\) is a bankruptcy-remote subsidiary created for a specific project or financing, isolating financial risk. Google&\#x27;s Tensor Processing Units \(TPUs\) are custom ASICs designed specifically to accelerate machine learning workloads. Manufacturer financing is a practice where producers like Boeing or GE help customers arrange funding for expensive equipment, which is what inspired the leasing structure with Apollo and Blackstone.

<details><summary>References</summary>
<ul>
<li><a href="https://corporatefinanceinstitute.com/resources/management/special-purpose-vehicle-spv/">Special Purpose Vehicle ( SPV ) - Guide, Examples, What You Need...</a></li>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>
<li><a href="https://jonathan-hui.medium.com/ai-chips-tpu-3fa0b2451a2d">AI Chips: Google TPU . Google ’s chip designers argue that the | Medium</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#finance`, `#hardware`

---

<a id="item-13"></a>
## [Trump Administration Drafts Import Ban on Chinese Optical Modules](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

The Trump administration is drafting a ban on imports of new Chinese optical modules used in data centers, according to four sources. The FCC is advancing the measure, with officials hoping to issue and enforce it this year to protect AI infrastructure. A ban would disrupt the global AI data center supply chain and hit Innolight, the world&\#x27;s largest optical module maker with a 27% market share. It would also escalate US-China tech decoupling in a critical infrastructure sector. The ban may still be revised or shelved, and the Chinese embassy in Washington said it will take all necessary measures to protect Chinese interests. The FCC has previously imposed similar import restrictions on Chinese drones, routers, robots, and inverters.

telegram · zaihuapd · Aug 4, 11:29

**Background**: Optical modules, also called optical transceivers, are hot-pluggable devices that convert electrical signals to optical signals for high-bandwidth data transmission in data centers and telecom networks. They are a key component in the infrastructure powering AI workloads, making them a target of security-focused trade restrictions. China is a major producer of these components, with Innolight \(Zhongji Innolight\) being the global leader.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Optical_module">Optical module</a></li>
<li><a href="https://www.linkedin.com/pulse/data-center-optical-module-real-world-5-uses-youll-actually-apnxc">Data Center Optical Module in the Real World: 5 Uses You&#x27;ll Actually...</a></li>

</ul>
</details>

**Tags**: `#trade policy`, `#AI infrastructure`, `#optical modules`, `#China`, `#data centers`

---

<a id="item-14"></a>
## [China issues first mandatory national standard for L3/L4 autonomous driving](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

On July 30, 2026, China&\#x27;s Ministry of Industry and Information Technology issued GB 44721—2026, the country&\#x27;s first mandatory national standard for L3 and L4 autonomous driving systems. The standard takes effect on July 1, 2027, upgrading the previous 2024 recommended standard to a compulsory requirement. This marks a major regulatory milestone, shifting China&\#x27;s L3/L4 autonomous driving safety rules from voluntary to legally binding, giving automakers and technology companies a clear compliance deadline. It will shape the development, testing, and deployment of highly automated vehicles in the world&\#x27;s largest auto market. The standard applies to M-class \(passenger\) and N-class \(cargo\) vehicles equipped with L3/L4 systems, but explicitly excludes automated parking systems. It covers four dimensions — full-lifecycle safety assurance, dynamic driving capability, human-machine interaction and user notification, and multi-dimensional inspection and testing — and requires L3 systems to include driver-takeover-capability monitoring.

telegram · zaihuapd · Aug 4, 13:06

**Background**: SAE International&\#x27;s levels define L3 as &quot;conditional automation,&quot; where the driver must be ready to take over when the system requests, and L4 as &quot;high automation,&quot; where the system can handle all driving in specific conditions without human intervention. In China, national standards carry the GB code and are mandatory, while recommended standards use GB/T and are voluntary; this move converts the 2024 recommended standard into a compulsory one. M-class and N-class are United Nations vehicle-category definitions for passenger and cargo vehicles used in China&\#x27;s type-approval system.

<details><summary>References</summary>
<ul>
<li><a href="https://m.21jingji.com/article/20260804/herald/2ce85d00b1498fe646e9b8d576be5564.html">《智能网联汽车 自 动 驾 驶 系 统 安 全 要 求 》强制性国家标准正式发布 - 21...</a></li>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://www.shangyici.com/vehicle_778784">数乘 车 辆 _机动 车 的准乘人数_商易赐汽 车</a></li>

</ul>
</details>

**Tags**: `#autonomous-driving`, `#regulation`, `#China`, `#standards`, `#automotive`

---