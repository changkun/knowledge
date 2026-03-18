# Knowledge: Human Systems, AI, and Social Structures

[![中文](https://img.shields.io/badge/Language-%E4%B8%AD%E6%96%87-0A66C2)](zh/human-systems.md)

The "human" on this page is treated as a system that gives feedback, plays strategic games, distorts, and also forms institutions and group structure. This is not an abstract humanistic gesture.

If the [doctoral-training page](doctoral-training-and-research-formation.md) explains how research training was formed, this page asks what core problem space those lines ultimately flowed into: how humans enter systems, and how systems reshape humans in return. Within the research layer, it connects forward to [teaching](teaching-and-course-design.md) and the output layer.

## From Interaction to Human-in-the-Loop Questions

- The central question is how humans enter system loops: as judges, feedback sources, constraint providers, and failure points.
- Understanding interaction here means matching user intent, input channels, system assumptions, cognitive load, and feedback structure, not just interface aesthetics.

## Behavior, Memory, and Attention

- In the behavior-understanding line, the long-term concern is how people switch windows, allocate attention, form browsing trajectories, and develop behavior patterns in real tasks, rather than static preference alone.
- This later extends into context switching and prospective memory, including the effect of short-video systems on intention retention, and keeps asking how digital systems interrupt, reorder, or weaken human task maintenance.
- Concretely, the TikTok study (CHI 2023) showed that context switching induced by short-form video significantly degrades prospective memory — providing empirical evidence for the claim that digital systems weaken human task maintenance.
- Attention also moves beyond the behavioral layer. Later EEG and eye-tracking work brings internal and external attention states directly into adaptive-system design.

## Human-in-the-Loop Optimization, Judgment, and Failure Modes

- The central doctoral research theme is **intelligence in the loop / human in the loop**.
- The human here is a judgment-bearing subject with expertise, bounded rationality, expression noise, and context dependence.
- *The Impact of Expertise in the Loop for Exploring Machine Rationality* studies how expertise changes optimization loops. *The Human in the Infinite Loop* further shows how human-machine loop failure is produced, hidden, and interpreted.
- Later work on opinion measurement interfaces pushes the question further: systems do not passively "read" opinions, but shape, amplify, or distort expression through interface structure.
- The durable focus lies in trade-offs, explanation, failure, responsibility, and judgment structure inside optimization loops, rather than in a single model.

## Adaptive VR/AR and Embodied Signals

- Another clear line brings physiological and perceptual state directly into the system loop.
- Related work covers adaptive VR/AR, visual-complexity adaptation, mixed-reality visual search, mixed-reality typing, motion training, and VR exergaming.
- EEG, EDA, ECG, fixation-related potentials, and eye tracking are used here to ask a deeper question: when user state is partly ineffable, continuously drifting, and embodied, what does it mean for a system to genuinely understand the human?
- This also explains the later interest in attention, engagement, arousal, and fatigue, which are more complex human signals than conventional click feedback.

## Human Computation and Group Systems

- There is sustained work on crowdsourcing, collective intelligence, human computation, prediction markets, credit-risk rating, social-behavior analysis, and participation incentives.
- The ten-part human-computation series works through this space systematically, starting from the distinction between crowdsourcing as task distribution to anonymous workers and collective intelligence as emergent accuracy under structural conditions. GWAPs are treated as intent-alignment games: they succeed not by instructing participants but by making useful computation a side effect of entertainment. Aggregation is not averaging; the series examines link-prediction and PageRank-style mechanisms that extract signal from heterogeneous, noisy contributions. A persistent theme is how standard data-science assumptions break down in participation systems: selection bias, observer effects, and power-law artifacts make naive analysis unreliable. Incentive design receives the sharpest attention — gamification often fails because players optimize for points rather than quality, cold-start problems starve new systems of signal, and reputation mechanisms invite gaming. The recurring structural lesson is that group intelligence is not a default outcome but an engineering target: most designs fail because they assume goodwill instead of building for adversarial or lazy participants.
- This line does not remain at the level of blog reflection; it also enters formal research, including malicious-player detection in a GWAP disaster-monitoring setting and intelligent interfaces that combine crowd input with machine learning for oil-spill detection.
- A repeated claim is that groups are not automatically smart. Collective intelligence requires diversity, independence, decentralization, and working aggregation mechanisms.
- There is continued attention to cold start, noise, power-law participation, long tails, cheating, reputation, gamification side effects, incentive compatibility, and ethics.
- Reflexivity and herd effects are treated as recurring sources of vicious cycles in markets, search, democracy, and wiki-like systems.

## View of AI

- Early thinking about AI already comes from computational complexity, the von Neumann architecture, and statistics, with a consistent reservation toward claims that intelligence has already been "solved."
- Later, the frame shifts toward stable structure, control planes, constraint systems, agency, and self-reference.
- The focus moves from "will the model become stronger?" to "what kind of system forms a stable self-model, outsources human metacognition, or shifts the position of the subject?"
- Once AI enters the real world, the decisive factors are often permissions, monitoring, evaluation, governance, and organizational structure, with the model as only one layer.

## Agentic AI and Responsibility Chains

- Recent public notes sharpen this cluster further: confirmation fatigue, approval scaling, plan-level approval, risk-proportional oversight, and sandbox-first review.
- The unpublished synthesis draft *HIAL: Human-in-the-Agent-Loop for Agentic Systems with Side Effects* shows that this has already been organized into a new research problem: how human oversight remains effective under scale, fatigue, and adversarial pressure when agents have real side effects.
- Trust calibration has recently become a concrete research output (2026), studying how the degree of trust humans place in AI systems can be measured and adjusted. This extends the intelligence-in-the-loop line into a question about how humans should calibrate reliance on agentic systems.
- Human-in-the-loop questions here also touch protocol gaps, responsibility allocation, audit reconstructability, and organizational governance.
- The core judgment about agent workflows is that scarce human value lies in calibration, intervention, veto, and explanation at high-leverage boundaries, not in step-by-step confirmation.
- The unpublished talk *Intelligence in the Agentic Loop* shows that this cluster is already being treated as a central design problem for AI-first software-engineering workflows. Enterprise AI platforms, workflow orchestration, knowledge management, and governance work further show that these judgments have entered real organizational systems.

## Preference, Ethics, and Self-Reference

- Recent notes push the human question toward preference and subjectivity: preference is treated as a heterogeneous object spanning computer science, behavioral economics, biology, ethics, and organizational decision-making, not as a single utility function.
- The synthesis draft *Preferential Bayesian Optimization: Frontiers and Cross-Disciplinary Reflections* systematizes this further, connecting preference optimization to constructed preference, dynamic preference, natural-language preference elicitation, and preference ecology.
- There is explicit interest in moral judgment, action, knowledge-belief paradoxes, self-referential structure, transparent minds, and identity construction.
- The self-reference question is sharpened into a structural claim: the question of AI capability can be reframed as a question about self-model formation. A system that maintains a recursive representation of itself — tracks its own state, corrects its own errors, includes its own actions in its world-model — is where "I" begins. This reframing moves the debate from philosophical deadlock around consciousness and qualia to a researchable complexity problem: how recursive self-representation is built, maintained, and bounded.
- LLMs are approached by asking whether they really form self-referential loops, whether they only simulate metacognition, and whether the human subject position is being reassigned.

## Society and Organization

- There is sustained interest in social choice, the Pareto frontier, and the mismatch between individual preference and collective decision-making.
- There has also been systematic thinking about firm theory, business models, and information-industry regularities, especially company boundaries, automation, market transparency, and organizational genes.
- Systems are often viewed by comparing technical, organizational, and social systems within the same complex-systems frame.
- More recently, questions such as whether responsibility chains are visible, whether control and accountability align, and why oversight decays into ritual have moved to the center.

## References

- [changkun.de/research/](https://changkun.de/research/)
- [The Impact of Expertise in the Loop for Exploring Machine Rationality](https://changkun.de/paper/expertise.pdf)
- [The Human in the Infinite Loop](https://changkun.de/paper/infloop.pdf)
- [Optimizing Visual Complexity for Physiologically-Adaptive VR Systems](https://changkun.de/paper/chiossi2024optimizing.pdf)
- [changkun.de/blog/posts/2014-02-18-Paper读后感：人机交互的进展及面临的挑战/](https://changkun.de/blog/posts/2014-02-18-Paper读后感：人机交互的进展及面临的挑战/)
- [changkun.de/blog/posts/2014-06-24-拙谈人工智能的未来/](https://changkun.de/blog/posts/2014-06-24-拙谈人工智能的未来/)
- The human-computation series starting from [changkun.de/blog/posts/2017-05-14-人肉计算-一-众包与群众智慧/](https://changkun.de/blog/posts/2017-05-14-人肉计算-一-众包与群众智慧/)
- [changkun.de/blog/posts/2017-06-06-瞎扯-对现代企业理论与当下IT企业的商业模式和信息产业链的规律性的思考/](https://changkun.de/blog/posts/2017-06-06-瞎扯-对现代企业理论与当下IT企业的商业模式和信息产业链的规律性的思考/)
- 2018 paper / note: `Issues of Human-Bot Interaction`
- [changkun.de/blog/posts/2022-12-30-2022-reading/](https://changkun.de/blog/posts/2022-12-30-2022-reading/)
- 2026 public notes: `Confirmation Fatigue and Protocol Gaps in Agentic-AI Oversight`, `Trade-Offs and Responsibility-Chain Design in Human-Machine Loops`
- 2026 public notes: `Multidisciplinary Definitions and Driving Mechanisms of Preference`, `Self-Reference Paradoxes and Self-Reference in Living Programs`
- Unpublished talk: `Intelligence in the Agentic Loop: Designing an AI-First Software Engineering Workflow`
- [changkun.de/blog/posts/2026-03-10-self-reference-boundary/](https://changkun.de/blog/posts/2026-03-10-self-reference-boundary/)
- [Short-Form Video and Prospective Memory](https://changkun.de/paper/tiktok.pdf)
- [Trust Calibration in AI Systems](https://changkun.de/paper/ou2026trustcalib.pdf)

## One-Sentence Summary

The stable interest on this page is to treat humans, machines, organizations, and societies alike as constrained systems with feedback, incentives, responsibility chains, and subject boundaries.
