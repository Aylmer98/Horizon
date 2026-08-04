---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 41 条内容中筛选出 14 条重要资讯。

---

1. [白宫逆转开源 AI 监管立场，硅谷分歧加深](#item-1) ⭐️ 8.5/10
2. [Mistral 发布 Shieldstral 3B 开放权重多模态审核模型](#item-2) ⭐️ 8.0/10
3. [用于生成多样化肤色的新算法与色彩空间](#item-3) ⭐️ 8.0/10
4. [Waymo 在达拉斯向公众开放无人驾驶网约车服务](#item-4) ⭐️ 8.0/10
5. [Troy Hunt：联邦快递混乱的邮件助长钓鱼攻击](#item-5) ⭐️ 8.0/10
6. [DeepSeek V4 Flash 在单块 AMD MI300X 上实现 150+ tokens/s](#item-6) ⭐️ 8.0/10
7. [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](#item-7) ⭐️ 8.0/10
8. [Xbox 宕机致光盘游戏无法游玩，数字所有权之争再起](#item-8) ⭐️ 8.0/10
9. [为 AI 自我改进而设计驾驭工程](#item-9) ⭐️ 8.0/10
10. [MiniMax-H3 全能模态模型发布 MLX 移植版，适配 Apple Silicon](#item-10) ⭐️ 8.0/10
11. [华为首席科学家警告英伟达芯片将触及物理极限](#item-11) ⭐️ 8.0/10
12. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资架构](#item-12) ⭐️ 8.0/10
13. [特朗普政府拟起草中国光模块进口禁令](#item-13) ⭐️ 8.0/10
14. [我国首部 L3/L4 自动驾驶强制性国标发布](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [白宫逆转开源 AI 监管立场，硅谷分歧加深](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 8.5/10

据报道，白宫放弃了限制中国开源 AI 模型的计划，转而聚焦提升美国 AI 竞争力。8 月 4 日，白宫邀请科技公司商议新框架，拟在模型发布前审查网络安全。 这一政策逆转可能重塑美中科技竞争和全球 AI 格局。AI 实验室与平台公司之间的深刻分歧，揭示了在开源 AI 是否构成国家安全威胁上的根本对立。 这一逆转源于硅谷的强烈反对，包括英伟达 CEO 黄仁勋为开源辩护，并组建了逾 230 家成员的安全联盟。导火索是中国 Kimi 模型的部分性能比肩 OpenAI 顶级模型。

telegram · zaihuapd · 8月4日 15:22

**背景**: 开源 AI 模型公开发布权重，任何人都可以使用和修改，这引发了关于其是否会助长滥用或加速创新的辩论。Kimi 是中国公司月之暗面的系列大语言模型，其最新 K3 模型据称拥有 2.8 万亿参数和 100 万 token 上下文窗口。白宫的内部辩论反映了国家安全与 AI 竞争力之间的更广泛张力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_%28chatbot%29">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/">Kimi API Platform</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#Open source`, `#Geopolitics`, `#Technology policy`, `#Artificial Intelligence`

---

<a id="item-2"></a>
## [Mistral 发布 Shieldstral 3B 开放权重多模态审核模型](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral 发布了 Shieldstral，一个 3B 规模的开权重多模态安全分类器，用于内容审核。该模型使用 LoRA 在语言模型参数上进行微调，并已在 Hugging Face 上提供。 Shieldstral 提供了一种经济高效且可本地部署的审核方案，这可能会让那些在内容审核责任上挣扎的平台受益。它相对于模型规模而言的强劲表现表明，更小、更专门化的模型可以与更大的系统竞争。 该模型将内容审核转化为一种策略自适应的“是/否”问答任务，据称在文本安全基准上可以匹敌甚至超越近七倍大的模型。它是开放权重的，这意味着最终参数被公开，但训练数据和代码可能不会完全发布。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**背景**: 开放权重模型被公开，使任何人都能在自己的基础设施上使用和自定义它们，但它们不同于完全开源的人工智能系统——后者还会公开训练数据和代码。多模态内容审核利用自动化系统分析文本、图像、音频和视频，以检测违反政策的内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral . | Mistral AI</a></li>
<li><a href="https://arxiv.org/html/2607.25857">Shieldstral</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_artificial_intelligence">Open-weight artificial intelligence</a></li>

</ul>
</details>

**社区讨论**: 评论者对这个模型的可定制性提出疑问，有人询问它能否在不重新训练的情况下应用任意规则集。还有人开玩笑建议将其改名为“Safestral”，并指出 Mistral 可能转向更小、更专门化的模型；一位开发者称其为内容审核的“现实且经济高效的解决方案”，另一位则询问它与 OpenAI 的 omni-moderation 相比如何。

**标签**: `#AI`, `#moderation`, `#open-source`, `#Mistral`, `#multimodal`

---

<a id="item-3"></a>
## [用于生成多样化肤色的新算法与色彩空间](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

一位开发者发布了一个交互式页面，介绍了一种自定义色彩空间和程序化生成算法，用于在数字艺术和游戏开发中选择多样化且可信的肤色。该项目包含取色器、多个 JavaScript 演示，以及关于底层方程和性质的详细说明。 这项工作解决了数字艺术和游戏开发工具中的一个实际缺口：在这些场景中，选择一组多样化但写实的肤色往往既繁琐又不直观。它还将算法思维引入到一个关乎代表性的领域，可能帮助创作者制作更具包容性的内容。 根据社区评论，该方法可能涉及类似 PCA 的降维，以及对 U-space 向量进行手动函数拟合。作者指出方法论可能不太严谨，并包含“未来工作”章节；部分评论者还观察到该模型在某些情况下会产生绿色、蓝色或紫色等异常颜色。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 肤色是物理与人类感知的复杂混合体，受光照和许多其他因素影响很大。颜色科学研究，如 Pantone SkinTone 和 Oklab 等感知均匀色彩空间，一直在尝试对这些变化建模；此外，无论什么种族，当饱和度调高到 100% 时，肤色往往会趋向橙色。

**社区讨论**: 评论者总体上热情很高，称赞了页面的呈现方式，并表示原本以为会看到基于 PCA 的降维，结果发现函数拟合的想法非常巧妙。多位评论者补充了有价值的背景，例如这种色彩分布在 Oklab 空间中与粉底色号分布呈现的月牙形相似、提到 Pantone SkinTone，以及高饱和度会让所有肤色看起来偏橙色的观察；还有一位评论者提到在某些样本中看到了绿色、蓝色和紫色。

**标签**: `#color science`, `#skin tones`, `#procedural generation`, `#digital art`, `#game development`

---

<a id="item-4"></a>
## [Waymo 在达拉斯向公众开放无人驾驶网约车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 已在德克萨斯州达拉斯向公众开放完全无人驾驶的网约车服务，达拉斯-沃斯堡地区是全美最大、最依赖汽车的大都会区之一。该服务现面向达拉斯-沃斯堡地区的所有乘客开放。 这标志着自动驾驶网约车服务大规模扩展至一个人口密度低、城区蔓延且公共交通有限的大都会区，考验自动驾驶汽车能否在密集市中心之外蓬勃发展。若取得成功，可能加速自动驾驶汽车的普及，并影响城市规划、住房和交通政策。 Waymo 的服务完全无人驾驶，Waymo Driver 系统从接载到目的地全程掌控，车内没有安全驾驶员。达拉斯-沃斯堡地区的此次推出是一次显著的考验，因为该地区以低密度城市蔓延和重度依赖汽车的文化著称，与 Waymo 早期运营区域不同。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 是 Alphabet 旗下的自动驾驶子公司，开发 Waymo Driver 系统，该系统被设计为 Level 4 级别的完全自动驾驶技术。该公司于 2018 年在凤凰城推出了全球首个自动驾驶网约车服务 Waymo One，此后扩展到美国其他城市。其服务全天候运营，已累计完成超过 2000 万次行程，乘客满意度达到 93%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride - Hail</a></li>
<li><a href="https://waymo.com/waymo-driver/">Self-Driving Car Technology for a Reliable Ride - Waymo Driver</a></li>

</ul>
</details>

**社区讨论**: 评论总体积极，有乘客表示 Waymo 车辆已变得司空见惯，且比人类司机引发的事故少得多，尽管偶尔会卡住。一位房地产开发商认为，无人驾驶汽车可以成为一种非常有效且被忽视的可负担住房政策；另一位评论者则提出关于交通罚单、保险和自动驾驶事故刑事责任等尚未解决的法律问题。

**标签**: `#Waymo`, `#autonomous vehicles`, `#transportation`, `#urban mobility`

---

<a id="item-5"></a>
## [Troy Hunt：联邦快递混乱的邮件助长钓鱼攻击](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

知名安全研究员 Troy Hunt 批评联邦快递的合法邮件做法，认为这些邮件看起来与钓鱼邮件极为相似，用户根本难以分辨。这削弱了人们识别诈骗邮件的能力。 由于钓鱼攻击仍然是最大的网络安全威胁之一，正规公司发送看似未通过认证的混乱邮件，会降低用户的警惕性，从而使钓鱼攻击更容易得手。 Hunt 指出，联邦快递的邮件常使用泛化的发件人名称、奇怪的链接和不一致的格式——这些正是钓鱼活动常用的特征。他认为，如果没有 DMARC 等强邮件认证机制，用户就没有可靠信号去区分真实邮件与伪造邮件。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**背景**: 钓鱼攻击通常利用伪装成联邦快递等可信品牌的欺诈邮件。SPF、DKIM 和 DMARC 等邮件认证协议可帮助收件方验证邮件是否确实来自声称的域名，但这些协议并非总是被强制执行，因此用户只能依靠外观来判断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://dmarc.org/overview/">Overview – dmarc.org</a></li>
<li><a href="https://abnormal.ai/glossary/email-spoofing">Email Spoofing: Types, Examples, and Prevention | Abnormal AI</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了类似经历，例如收到的合法联邦快递海关通知看上去像诈骗邮件，Google 存储空间警告使用了 c.gle 等不熟悉的域名。他们还指出，新顶级域名的泛滥以及国税局（IRS）等机构使用的文本转语音系统，让非技术用户更难以识别钓鱼邮件。

**标签**: `#security`, `#phishing`, `#email`, `#ux`, `#fedex`

---

<a id="item-6"></a>
## [DeepSeek V4 Flash 在单块 AMD MI300X 上实现 150+ tokens/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一个社区项目展示了 DeepSeek V4 Flash（284B 参数的混合专家模型）能在单块 AMD MI300X GPU 上高效运行，速度超过每秒 150 个 token。该方案将原本完整的 100 万 token 上下文窗口缩减为仍然实用的 25.6 万 token，以此换取性能。 在单块加速器上运行最先进的 MoE 模型，挑战了前沿推理必须依赖 NVIDIA 硬件或多块 GPU 的固有假设。这使得高端推理模型更容易获得，也凸显了拥有大容量 HBM 的 AMD MI300X 是本地 AI 推理的可行平台。 MI300X 是一种 OAM 模块，配备 192GB HBM；这一实用化的 256k 上下文配置之所以能装入显存，是因为 DeepSeek V4 Flash 的 256 个 MoE 专家原生采用 MXFP4 量化。该实现参考了早期在双路 MI300X 上运行该模型的成果，相关链接已在项目 readme 中列出。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**背景**: DeepSeek V4 Flash 是 DeepSeek 推出的面向效率优化的混合专家（MoE）模型，总参数量为 284B，但每个 token 仅激活 13B 参数，原生支持 100 万 token 的上下文窗口。MoE 模型对每个 token 只激活一部分参数，从而在大幅降低计算成本的同时保留庞大的总参数量。相比 NVIDIA H100，AMD MI300X 的理论算力为 1.32 倍、显存容量为 2.4 倍、峰值显存带宽为 1.58 倍，因此非常适合显存受限的大模型推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://moreh.io/technical-report/moreh-vllm-performance-evaluation-deepseek-v3-r1-671b-on-amd-instinct-mi300x-gpus-250829/">Moreh vLLM Performance Evaluation: DeepSeek V3/R1 671B on AMD ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体积极，但也指出了若干问题：MI300X 单块难以单独购买，通常需要约 25 万欧元的 8 卡整机；也有人指出基于 PCIe 的 MI350P（144GB）是更容易获得的替代方案。还有评论提到 DwarfStar 等已有工作能在更小显存中运行同一模型，作者未引用；多数人认为 256k 上下文窗口是务实取舍，因为模型在接近完整 100 万窗口时质量确实会下降。

**标签**: `#AI/ML`, `#GPU inference`, `#DeepSeek`, `#AMD MI300X`, `#Mixture of Experts`

---

<a id="item-7"></a>
## [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

Shai-Hulud 蠕虫的新一轮攻击正在积极入侵 npm 包，最先受到影响的是 Node.js 生态中广泛使用的 keyv 和 cacheable。该恶意软件会窃取开发者的凭证，将自己发布到所有可写的 npm 包，并在 GitHub 仓库中植入执行钩子。 仅 keyv 一个包就被超过 1700 个 npm 项目依赖，因此这次攻击对 JavaScript/Node.js 生态的波及面很广。这也是最近几个月内第三起针对 npm 的重大供应链攻击，凸显出开发者与企业共同面临的威胁模式正在加剧。 据 JFrog 安全研究团队称，这个蠕虫会窃取凭证，并通过把自己发布到所有可写的 npm 包来进行传播，同时还会在 GitHub 仓库中植入执行钩子。npm 官方页面显示 keyv 最新版 6.0.0 于一小时前发布，说明被入侵的版本非常新。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: npm 是 Node.js 的默认包管理器，安装依赖时会自动运行安装脚本，这使得 npm 生态成为供应链攻击的主要目标。Shai-Hulud 是一种能自我传播的蠕虫，此前已入侵过数百个 npm 包并窃取开发者凭证。SecurityWeek 指出，这是继 s1ngularity 攻击和 Josh Junon 被入侵之后，npm 面临的第三起重大供应链攻击；Josh Junon 维护的包每周下载量合计超过 25 亿次。上游包一旦被入侵，就会通过自动安装脚本，把恶意代码传播给所有依赖它的项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.jfrog.com/post/shai-hulud-is-back-august/">Major Shai Hulud campaign strikes npm again, affecting keyv and 400+ packages - JFrog Security Research</a></li>
<li><a href="https://www.securityweek.com/shai-hulud-supply-chain-attack-worm-used-to-steal-secrets-180-npm-packages-hit/">Shai - Hulud Supply Chain Attack : Worm Used to... - SecurityWeek</a></li>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体上是沮丧而谨慎的：多位评论者呼吁取消或严格限制 pre-install 和 post-install 钩子，因为它们是此类攻击的常见载体。还有人分享了实用的缓解方法，例如在 .npmrc 中设置 &\#x27;min-release-age=5&\#x27;，以及提供关于 npm 供应链攻击技术的最新文档链接。一些评论者对依赖系统的脆弱性以及清理连锁入侵的难度表示担忧。

**标签**: `#security`, `#npm`, `#supply-chain`, `#javascript`, `#devops`

---

<a id="item-8"></a>
## [Xbox 宕机致光盘游戏无法游玩，数字所有权之争再起](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

近期一次 Xbox 服务宕机导致用户无法游玩自己拥有的实体光盘游戏，因为主机无法与微软服务器完成所需的 DRM 验证。这一事件引发了 594 条社区评论，成为讨论 DRM 限制和数字游戏所有权侵蚀的焦点。 这一事件表明，即使是“实体”游戏购买也日益依赖在线许可证检查，一次服务器宕机就能让消费者失去对自己已购游戏的访问权。它影响到所有玩家，并强化了关于消费者权利、DRM 以及向许可证式所有权转变的行业辩论。 在 Xbox 上，光盘游戏的 DRM 通常会将许可验证链到光盘、主机、用户账户、微软服务器和“常用 Xbox”设置上，因此离线游玩依赖多个条件。微软一直在悄悄调整其 DRM，但该平台仍然是一个混合生态系统，更新、账户系统和服务可用性依然影响着所有权。

hackernews · surprisetalk · 8月4日 12:01 · [社区讨论](https://news.ycombinator.com/item?id=49167448)

**背景**: DRM（数字版权管理）是限制数字内容使用方式的技术，游戏主机用它来验证玩家是否真正拥有某款游戏。当你购买数字游戏时，通常买到的只是按特定条款访问该游戏的许可证，而不是软件本身，发行商可以几乎不发出警告就撤销或更改访问权限。这推动了例如“Stop Killing Games”请愿等活动，以及大众对娱乐行业数字购买长期可靠性的广泛担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.windowscentral.com/xbox-drm-explained">Xbox DRM explained: Setting a home console, console sharing, licenses, and more | Windows Central</a></li>
<li><a href="https://dataconomy.com/2025/08/28/digital-ownership-in-gaming-what-you-actually-own/">Digital Ownership In Gaming: What You Actually ‘own’ - Dataconomy</a></li>
<li><a href="https://www.strandmagazine.co.uk/single-post/do-we-own-the-games-we-play-a-look-into-what-digital-game-ownership-means">Do We Own the Games We Play? A Look into What Digital Game Ownership Means</a></li>

</ul>
</details>

**社区讨论**: 评论者对真正所有权的丧失表达了强烈不满：一位用户指出，像 GameCube 这样较老的主机可以离线游玩“直到我离世”，另一位则认为真正的问题在于所有权，而不是实体与数字之争，并列举了转售和把游戏传给子女等权利。还有人指出，第七代主机在本地托管联机、匹配服务器至今可用，反而处理得更好。总体情绪是，现代 DRM 让即使是光盘游戏也变得更脆弱，离不开在线基础设施。

**标签**: `#gaming`, `#DRM`, `#digital ownership`, `#Xbox`, `#outage`

---

<a id="item-9"></a>
## [为 AI 自我改进而设计驾驭工程](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

在 2026 年 7 月的一篇博客文章中，Lilian Weng 探讨了如何通过工程化的驾驭（harness）——即工具、技能和评估——使 AI 系统能够改进自身性能。这篇文章引发了社区的高度关注，获得了 291 个点赞和 64 条评论，讨论实施策略。 这标志着 AI 改进的重点从模型权重转向了周围的驾驭层，有望实现更高效的自我改进。这对构建智能体系统的工程团队至关重要，因为工具、上下文和评估设计正成为影响性能的关键手段。 文章涵盖了适应度函数、工具优化和驾驭评估策略。社区评论分享了一些实用技巧，例如读取生产环境轨迹、让智能体编写自己的工具（将上下文从 15 次调用的 2 万 token 压缩到单次调用的 800token），以及使用评估/验证集来防止奖励黑客行为。

hackernews · tosh · 8月4日 06:17 · [社区讨论](https://news.ycombinator.com/item?id=49164896)

**背景**: 驾驭工程指的是设计 AI 模型外部的基础设施——包括工具、上下文、指令和评估——来控制和优化其行为，而不是修改模型的权重。OpenAI、Anthropic 和 Martin Fowler 等近期工作也探索了类似理念，强调信息组织和高效工具编写对智能体性能至关重要。这一概念还与递归自我改进相关联，即系统改进自身代码或工具的愿景，这自 AI 研究诞生之初便是核心目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/harness-engineering/">Harness engineering: leveraging Codex in an agent-first world | OpenAI</a></li>
<li><a href="https://www.anthropic.com/engineering/writing-tools-for-agents">Writing effective tools for AI agents—using AI agents \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区态度总体积极且务实。bisonbear 强调需要可靠的适应度函数来优化大型代码库的智能体驾驭；zby 认为面向提示词和代码的训练范式可能比权重训练更具样本效率；scosman 分享了利用自动研究优化驾驭的成功经验，要求读取生产轨迹并允许智能体编写自己的工具；storus 则好奇何时驾驭层能生成自己的 RLHF/DPO 训练集并进行 LoRA 微调。还有一条轻松评论调侃了追求“Torment Nexus”的持续探寻。

**标签**: `#AI agents`, `#harness engineering`, `#self-improvement`, `#tool optimization`, `#evaluation`

---

<a id="item-10"></a>
## [MiniMax-H3 全能模态模型发布 MLX 移植版，适配 Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax 发布了 MiniMax-H3，一个支持文本、图像、音频和视频的全能模态生成系统。一个新的 Python 包将该模型移植到 MLX，Simon Willison 已在 M5 Max MacBook Pro 上成功运行并生成了视频片段。 这使开发者和研究者能够在 Apple Silicon 上本地运行最先进的多模态视频生成，减少对云端 GPU 服务的依赖。这也凸显了 MLX 模型移植生态的快速增长，让先进 AI 模型更加易用。 该模型可生成最长 15 秒、最高 2K 分辨率并带有原生音频的视频片段。该实验需要约 115 GB 的模型文件，在 M5 Max 上生成单个视频耗时近 45 分钟；在未使用提示词指南的情况下，音频输出质量较差。

rss · Simon Willison · 8月4日 19:10

**背景**: MLX 是 Apple 专为 Apple silicon 设计的开源机器学习数组框架，针对统一内存架构优化，并提供类似 NumPy 的 API。全能模态模型是指在单一统一架构中处理多种数据模态（文本、图像、音频和视频）的 AI 系统。MiniMax-H3 是 MiniMax 发布的一款通用全能模态生成模型，提供开放权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://fal.ai/minimax-h3">MiniMax H3 - Open-Weights General-Purpose Multimodal Video Model | fal</a></li>

</ul>
</details>

**标签**: `#MLX`, `#MiniMax-H3`, `#multimodal AI`, `#video generation`, `#Apple Silicon`

---

<a id="item-11"></a>
## [华为首席科学家警告英伟达芯片将触及物理极限](https://www.bloomberg.com/news/articles/2026-08-04/huawei-s-top-scientist-warns-of-chip-limit-nvidia-will-soon-face) ⭐️ 8.0/10

华为首席半导体科学家廖恒在 7 月底一次罕见的四小时公开采访中警告，英伟达通过不断增加计算芯片和高带宽内存来扩展规模的做法终将触及物理极限，并提出华为的 LogicFolding（逻辑折叠）框架作为替代路径。首款采用 LogicFolding 技术的手机芯片将于今年晚些时候亮相。 这位华为顶尖科学家的警告意味着，长期以来由摩尔定律驱动的传统芯片缩放正逼近终点，而华为正将 LogicFolding 框架和“韬定律”（Tau Scaling Law）打造为绕开制裁的替代路线。在中美半导体产业分化为两个独立生态系统的背景下，这一技术路线可能重塑 AI 芯片和先进制程的竞争格局。 LogicFolding 架构将逻辑电路物理折叠并堆叠为双层结构，以缩短信号传输距离、降低电阻电容负载，从而在不使用 EUV 光刻机的情况下实现等效 1.4nm 级性能，并宣称晶体管密度提升 55%。廖恒还指出，中美半导体产业正分化为两个独立生态系统，各方必须建立完整的制造与供应能力才能生存。

telegram · zaihuapd · 8月4日 08:04

**背景**: 摩尔定律是半导体行业长期遵循的经验法则，指芯片上的晶体管密度大约每两年翻一番，从而推动性能持续提升。随着传统制程微缩越来越困难，英伟达等公司转而依靠更大的芯片尺寸和高带宽内存来维持性能增长。由于美国制裁使华为无法获得先进 EUV 光刻机，华为于 2026 年在国际电路与系统会议（ISCAS）上正式发布“韬定律”和 LogicFolding 架构，希望在不依赖 EUV 的情况下继续提升芯片性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/huawei-claims-sanctions-busting-breakthrough-with-1-4nm-class-chips-by-2031-claims-55-percent-higher-transistor-density-firm-claims-new-logicfolding-chip-architecture-can-bypass-euv-restrictions-introduces-tau-scaling-law-to-replace-moores-law">Huawei claims sanctions-busting breakthrough with 1.4nm-class chips by 2031, claims 55% higher transistor density — firm claims new LogicFolding chip architecture can bypass EUV restrictions, introduces &#x27;Tau Scaling Law&#x27; to replace Moore&#x27;s Law | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.huaweicentral.com/huawei-logicfolding-architecture-everything-you-need-to-know/">Huawei LogicFolding Architecture: Everything you need to know - Huawei Central</a></li>
<li><a href="https://timesofindia.indiatimes.com/technology/tech-news/explained-what-is-huaweis-logicfolding-tau-scaling-law-and-how-it-plans-to-build-1-4nm-chips-without-asml/articleshow/131314122.cms">Explained: What is Huawei&#x27;s LogicFolding, Tau Scaling Law, and how it plans to build 1.4nm chips without ASML - The Times of India</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#AI chips`, `#Huawei`, `#Nvidia`, `#physical limits`

---

<a id="item-12"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

谷歌已悄然搭建史上最大规模的基础设施融资架构之一，支持向 Anthropic 交付超过 1500 亿美元的 AI 芯片，相关合同总额约 2000 亿美元。今年 6 月，特殊目的载体 Compute SPV 完成首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力、100 万颗 TPU。 这是有史以来为 AI 基础设施搭建的最大融资机制，使 Anthropic 在无信用评级的情况下仍能获得巨大算力。该架构将风险分散到芯片制造商、资产管理公司和银行之间，可能为 AI 公司为数据中心和芯片融资开创先例。 谷歌为数据中心提供担保，博通购买并协助融资芯片，阿波罗与黑石购买硬件后回租给 Anthropic。该模式借鉴了波音和 GE 推销飞机和发动机时采用的厂商融资玩法，使各方都不必把数百亿美元的 AI 硬件压在自己资产负债表上。

telegram · zaihuapd · 8月4日 10:52

**背景**: 特殊目的载体（SPV）是为特定项目或融资而成立的破产隔离子公司，用于隔离财务风险。谷歌的张量处理单元（TPU）是专为加速机器学习任务而设计的定制 ASIC。厂商融资是波音、GE 等制造商协助客户为昂贵设备安排融资的做法，本次与阿波罗、黑石的租赁结构正是借鉴了这一模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://corporatefinanceinstitute.com/resources/management/special-purpose-vehicle-spv/">Special Purpose Vehicle ( SPV ) - Guide, Examples, What You Need...</a></li>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>
<li><a href="https://jonathan-hui.medium.com/ai-chips-tpu-3fa0b2451a2d">AI Chips: Google TPU . Google ’s chip designers argue that the | Medium</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#finance`, `#hardware`

---

<a id="item-13"></a>
## [特朗普政府拟起草中国光模块进口禁令](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 8.0/10

据四位知情人士透露，特朗普政府正在起草一项禁令，拟禁止进口用于数据中心的新型中国光模块。FCC 正在推进该措施，官员希望今年内发布并生效，以保护支撑 AI 热潮的关键基础设施。 若禁令实施，将冲击全球 AI 数据中心供应链，并重创全球光模块龙头中际旭创（市场份额约 27%）。此举也将使美中在关键基础设施领域的技术“脱钩”进一步升级。 该禁令仍可能被修改或搁置；中国驻美使馆表示，将对损害中国利益的行为采取一切必要措施。此前 FCC 已陆续对中国无人机、路由器、机器人和逆变器实施类似进口限制。

telegram · zaihuapd · 8月4日 11:29

**背景**: 光模块又称光收发器，是一种可热插拔的器件，用于在数据中心和电信网络中将电信号转换为光信号，实现高带宽数据传输。它们是支撑 AI 工作负载的关键基础设施组件，因此成为以安全为由的贸易限制的目标。中国是该类组件的主要生产国，其中中际旭创（Zhongji Innolight）为全球龙头。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Optical_module">Optical module</a></li>
<li><a href="https://www.linkedin.com/pulse/data-center-optical-module-real-world-5-uses-youll-actually-apnxc">Data Center Optical Module in the Real World: 5 Uses You&#x27;ll Actually...</a></li>

</ul>
</details>

**标签**: `#trade policy`, `#AI infrastructure`, `#optical modules`, `#China`, `#data centers`

---

<a id="item-14"></a>
## [我国首部 L3/L4 自动驾驶强制性国标发布](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

2026 年 7 月 30 日，工业和信息化部发布我国首部针对 L3 级和 L4 级自动驾驶系统的强制性国家标准 GB 44721—2026。该标准将于 2027 年 7 月 1 日起实施，将 2024 年的推荐性国标升级为强制性要求。 这一里程碑式的监管举措将中国 L3/L4 自动驾驶安全要求从推荐性转为强制性，为车企和科技公司设置了明确的合规期限。它将对全球最大汽车市场中高级别自动驾驶汽车的开发、测试与部署产生深远影响。 该标准适用于搭载 L3、L4 级系统的 M 类（载客）和 N 类（载货）车辆，但不适用于自动泊车系统。标准从企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、多维度检验检测四个维度构建安全要求体系，并要求 L3 级系统具备驾驶人接管能力监测功能。

telegram · zaihuapd · 8月4日 13:06

**背景**: SAE 国际标准将 L3 定义为“有条件自动化”，此时驾驶员必须在系统请求时随时接管；L4 为“高度自动化”，系统可在特定条件下完成全部驾驶操作，无需人工干预。中国强制性国家标准以 GB 编号开头，必须执行；推荐性国标以 GB/T 开头，自愿采用。本次发布把 2024 年的推荐性国标升级为强制性标准。M 类和 N 类车辆是联合国车辆分类体系中载客和载货车辆的定义，中国型式认证也采用这一分类。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.21jingji.com/article/20260804/herald/2ce85d00b1498fe646e9b8d576be5564.html">《智能网联汽车 自 动 驾 驶 系 统 安 全 要 求 》强制性国家标准正式发布 - 21...</a></li>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://www.shangyici.com/vehicle_778784">数乘 车 辆 _机动 车 的准乘人数_商易赐汽 车</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#regulation`, `#China`, `#standards`, `#automotive`

---