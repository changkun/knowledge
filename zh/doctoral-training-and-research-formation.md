# 知识：博士阶段与研究形成

[![English](https://img.shields.io/badge/Language-English-111827)](../doctoral-training-and-research-formation.md)

这页处理正式研究能力如何被组织起来：从早期交互原型，到行为理解与预测，再到博士阶段的人在环研究，以及若干反复出现的案例域。

它在整张地图里的位置，是基础层第一次汇入正式研究脉络的地方。与[数学](math-and-learning.md)、[系统](systems-and-engineering.md)、[语言与平台](languages-platforms-and-products.md)相比，这一页更关心正式研究训练形成了什么问题意识、方法组合和案例结构。这些研究最终汇成什么核心问题，由[人机、AI 与社会系统](human-systems.md)展开；研究训练如何再被组织成课程与指导，由[教学与课程设计](teaching-and-course-design.md)展开。

## 一条清晰的形成线

- 2016 年的本科论文 *Designing Alternative Contact-free Control Modalities for Smart Watches*，已经在处理输入通道、交互模式与可穿戴设备上的人机问题。
- 2019 年的硕士论文 *Understanding and Predicting Web Browsing Behavior*，把兴趣推进到行为理解、预测与用户状态建模。
- 2018 年起在 LMU 作为研究助理与讲师工作，研究、教学、工业合作和课程组织在同一阶段并行展开。
- 2023-04-03 完成 LMU 博士答辩，博士论文 *The Intelligence in the Loop: Empirical Explorations and Reflections* 随后以 2024 年版本公开。到这一阶段，研究主线已经明确转向 **intelligence in the loop / human in the loop**，而不再是某个单一技术方向。

把这三篇学位论文连起来看，研究形成沿着一条清楚的线推进：交互方式 -> 行为建模 -> 人在环判断、优化与系统失效。

- 博士后研究仍在活跃推进。2026 年关于 AI 系统信任校准的论文以及一篇已提交的意见测量界面论文表明，intelligence-in-the-loop 这条线仍在持续，现在正延伸到信任、偏好获取和代理式监督。

## 几个彼此相连的研究簇

### 行为理解与用户状态

- 硕士阶段的网页浏览行为研究，处理的是用户如何在标签页、网站和任务之间切换。这里的"理解用户"已经进入可建模、可预测、可进入系统设计的层面。
- 这项工作实际发现的是，浏览行为并非随机切换，而是被任务上下文和意图所组织——用户会形成可预测的标签页与窗口轨迹，这些轨迹可以被模型捕获。这使得"理解用户"从一个界面问题变成了一个建模问题，并为后来转向系统层面的行为分析奠定了基础。
- 这条线后来又延伸到前瞻记忆、上下文切换、注意状态等问题，继续追问系统如何影响人的意图保持、任务状态和认知负担。

### 人在环优化与机器理性

- 博士阶段最核心的工作，在于研究人如何进入优化回路、接口如何塑造判断、系统如何暴露或掩盖回路失效。
- *The Impact of Expertise in the Loop for Exploring Machine Rationality*、*The Human in the Infinite Loop* 与意见测量界面的工作，连成了一条明确的线：人在其中承担判断者、解释者、约束源和失效环节等角色。
- 这也解释了为什么后期会自然推进到偏好、权衡、解释和责任链这些问题。

### 生理信号、自适应系统与沉浸式交互

- 另一条重要的研究线，是用 EEG、EDA、ECG、eye tracking 等信号研究 adaptive VR/AR 系统。
- 相关工作覆盖视觉复杂度自适应、内外注意平衡、混合现实视觉搜索、输入表现、动作训练、VR 运动游戏等。
- 这些课题表面上分散，实际上都在问同一件事：如果用户状态本身是动态的、具身的、部分不可言说的，系统应该如何感知、建模并适应这种变化。

### 众包与机器学习结合与社会性系统

- 群体与系统的关系很早就出现了。早期有 GWAP 灾害监测系统中的恶意玩家检测，之后又有漏油检测这类把众包与机器学习结合起来的智能界面工作。
- GWAP 的工作表明，游戏化灾害监测容易被利用评分规则的恶意玩家攻击，所需的检测机制超出了简单的输入过滤范畴。漏油检测的工作则表明，众包输入与机器学习结合后能达到两者单独都无法达到的检测质量——由此建立了一种人与机器互补而非冗余的协作模式。
- 这说明研究脉络里一直有一条社会性维度：人在其中既可能是单个用户，也可能作为群体、标注源、噪声源、作弊者、协作者或集体判断的一部分进入系统。

## 方法气质

- **经验研究与系统实现并重**：既做实验、界面、信号采集和用户研究，也关心算法、数据处理和系统原型是否真的可运行。
- **从 interaction 到 loop**：问题不会停在“界面好不好用”，而会继续追问交互如何改变判断、判断如何进入优化、优化又如何反过来塑造人。
- **跨层证据意识**：行为数据、生理信号、实验操控、失败案例、解释界面和运行系统经常被放到同一证据链里。
- **案例域服务于方法**：不同应用场景的价值，在于它们让这些问题可以被观察、操控和验证。

## 图形、几何与 3D 系统在这里的真实位置

- 图形、几何处理和 3D 系统确实长期重要，但更准确的角色是高密度案例域，本身不定义研究身份。
- 它之所以显得分量较重，首先因为相关教学投入很大；其次因为它天然连接数学结构、交互界面、算法实现和工程合作。
- 与 WAY digital solutions 的 mesh processing backend 合作，也说明这条线并非纯课堂产物，而确实落到过正式工程系统。
- 从学位论文、核心论文和近年的问题推进方向看，真正稳定的母题仍然是 intelligence in the loop / human in the loop。

## Go 系统作为研究案例域

- [系统页](systems-and-engineering.md)所描述的系统工程能力并未停留在博客笔记层面。六项关于 Go 并发、channel 语义、指针管理、基准测试方法论和 options 模式的研究通过 golang.design 撰写为正式研究论文；一本合著的 Go 程序员面试手册由机械工业出版社出版（2022）。
- 与图形和几何类似，Go 是一个高密度案例域，数学结构（CSP 理论、调度）、系统实现（运行时、编译器）和工程判断在其中汇合。
- 它在研究形成中的分量，与图形出于同一原因：它以一种使研究问题可观察的方式，把基础理论和实现细节连在一起。
- 不同之处在于，Go 的机制研究同时反馈到开源与社区输出线，赋予它一种图形所不具备的双重角色。

## 参考页面

- [changkun.de/research/](https://changkun.de/research/)
- [The Intelligence in the Loop: Empirical Explorations and Reflections](https://changkun.de/thesis/phd.pdf)
- [Understanding and Predicting Web Browsing Behavior](https://changkun.de/thesis/master.pdf)
- [The Impact of Expertise in the Loop for Exploring Machine Rationality](https://changkun.de/paper/expertise.pdf)
- [The Human in the Infinite Loop](https://changkun.de/paper/infloop.pdf)
- [golang.design/research](https://golang.design/research/)
- [AI 系统中的信任校准](https://changkun.de/paper/ou2026trustcalib.pdf)
- [短视频与前瞻记忆](https://changkun.de/paper/tiktok.pdf)

## 一句话总结

这一页保留的是正式研究训练如何把交互、行为、优化、自适应系统和案例域组织成一条持续演化的研究脉络，重点不在“做过哪些论文”。
