# Knowledge: Doctoral Training and Research Formation

[![中文](https://img.shields.io/badge/Language-%E4%B8%AD%E6%96%87-0A66C2)](zh/doctoral-training-and-research-formation.md)

This page tracks how formal research capability was organized: from early interaction prototypes, to behavior understanding and prediction, to doctoral human-in-the-loop work, together with several recurring case domains.

Within the overall map, this is the point where the foundation layer first flows into a formal research trajectory. Compared with the pages on [mathematics](math-and-learning.md), [systems](systems-and-engineering.md), and [languages](languages-platforms-and-products.md), this page is more concerned with what kinds of questions, methods, and case structures formal research training produced. What core problem space these lines ultimately converge on is handled by [Human Systems, AI, and Social Structures](human-systems.md); how research training is reorganized into courses and supervision is handled by [Teaching and Course Design](teaching-and-course-design.md).

## A Clear Line of Formation

- The 2016 bachelor's thesis, *Designing Alternative Contact-free Control Modalities for Smart Watches*, already works on input channels, interaction modalities, and human-machine questions on wearable devices.
- The 2019 master's thesis, *Understanding and Predicting Web Browsing Behavior*, pushes the line toward behavior understanding, prediction, and user-state modeling.
- From 2018 onward, work at LMU as a research assistant and lecturer lets research, teaching, industry collaboration, and course organization develop in parallel.
- The LMU doctoral defense was completed on 2023-04-03. The dissertation, *The Intelligence in the Loop: Empirical Explorations and Reflections*, was later released publicly in a 2024 version. By this point, the research line had clearly shifted toward **intelligence in the loop / human in the loop** rather than a single technical direction.

Seen together, the three theses form a clear progression: interaction modality -> behavior modeling -> human-in-the-loop judgment, optimization, and system failure.

- Research continues actively post-PhD. A 2026 paper on trust calibration in AI systems and a submitted paper on opinion measurement interfaces show that the intelligence-in-the-loop line remains active, now extending into trust, preference elicitation, and agentic oversight.

## Several Connected Research Clusters

### Behavior Understanding and User State

- The master's work on web browsing behavior studies how users switch among tabs, websites, and tasks. "Understanding the user" is already at the level of something that can be modeled, predicted, and incorporated into system design.
- What the work actually showed is that browsing behavior is not random switching but is structured by task context and intention — users form predictable tab and window trajectories that can be captured in models. This reframed "understanding the user" as a modeling problem rather than an interface problem, and set up the later transition toward system-level behavior analysis.
- This line later extends into prospective memory, context switching, and attention state, continuing to ask how digital systems interrupt, reorder, or weaken intention retention, task state, and cognitive load.

### Human-in-the-Loop Optimization and Machine Rationality

- The central doctoral line studies how humans enter optimization loops, how interfaces shape judgment, and how systems expose or hide loop failure.
- *The Impact of Expertise in the Loop for Exploring Machine Rationality*, *The Human in the Infinite Loop*, and work on opinion measurement interfaces form a clear line in which humans act as judges, interpreters, constraint sources, and failure points.
- This also explains the later move toward preference, trade-offs, explanation, and responsibility chains.

### Physiological Signals, Adaptive Systems, and Immersive Interaction

- Another major line studies adaptive VR/AR systems through signals such as EEG, EDA, ECG, and eye tracking.
- Related work covers visual-complexity adaptation, internal/external attention balance, mixed-reality visual search, input performance, motion training, and VR exergaming.
- These topics look scattered on the surface, but they all ask the same question: if user state is dynamic, embodied, and only partly articulable, how should a system sense, model, and adapt to it?

### Crowd + Machine Learning and Social Systems

- The relationship between groups and systems appears early. There is early work on malicious-player detection in a GWAP disaster-monitoring system, followed by intelligent-interface work on oil-spill detection that combines crowds with machine learning.
- The GWAP work showed that gamified disaster monitoring is vulnerable to malicious players who exploit scoring rules, requiring detection mechanisms that go beyond simple input filtering. The oil-spill work showed that crowd input can be combined with machine learning to achieve detection quality that neither crowds nor models reach alone — establishing a pattern where human and machine contributions are complementary rather than redundant.
- This shows that the research line has always had a social dimension. Humans enter the system not only as individual users, but also as groups, label sources, noise sources, cheaters, collaborators, or parts of collective judgment.

## Methodological Temperament

- **Empirical research and system building together**: the work includes experiments, interfaces, signal collection, and user studies, but also cares about whether algorithms, data pipelines, and prototypes actually run.
- **From interaction to loop**: the question does not stop at whether an interface is usable. It continues to how interaction changes judgment, how judgment enters optimization, and how optimization shapes humans in return.
- **Cross-layer evidence awareness**: behavioral data, physiological signals, experimental manipulation, failure cases, explanation interfaces, and running systems are often placed in the same chain of evidence.
- **Case domains in service of method**: the value of different application domains is that they make these questions observable, controllable, and testable.

## The Real Place of Graphics, Geometry, and 3D Systems

- Graphics, geometry processing, and 3D systems remain important for a long time, but more as dense case domains than as the sole definition of research identity.
- Their weight comes partly from large teaching investment and partly from the way they naturally connect mathematical structure, interaction interfaces, algorithmic implementation, and engineering collaboration.
- Collaboration with WAY digital solutions on a mesh-processing backend also shows that this line was not confined to the classroom and did reach formal production systems.
- Across theses, core papers, and recent directions, the most stable parent theme remains intelligence in the loop / human in the loop.

## Go Systems as a Research Case Domain

- The systems-engineering expertise described on the [systems page](systems-and-engineering.md) did not remain at the level of blog notes. Six investigations into Go concurrency, channel semantics, pointer management, benchmarking methodology, and the options pattern were written up as formal research papers through golang.design, and a co-authored Go programmer interview handbook was published by China Machine Press (2022).
- Like graphics and geometry, Go serves as a high-density case domain where mathematical structure (CSP theory, scheduling), system implementation (runtime, compiler), and engineering judgment converge.
- Its weight in the research formation comes from the same reason as graphics: it connects foundational theory to implementation detail in a way that makes research questions observable.
- The difference is that Go mechanism work also feeds back into the open-source and community output lines, giving it a dual role that graphics does not have to the same degree.

## References

- [changkun.de/research/](https://changkun.de/research/)
- [The Intelligence in the Loop: Empirical Explorations and Reflections](https://changkun.de/thesis/phd.pdf)
- [Understanding and Predicting Web Browsing Behavior](https://changkun.de/thesis/master.pdf)
- [The Impact of Expertise in the Loop for Exploring Machine Rationality](https://changkun.de/paper/expertise.pdf)
- [The Human in the Infinite Loop](https://changkun.de/paper/infloop.pdf)
- [golang.design/research](https://golang.design/research/)
- [Trust Calibration in AI Systems](https://changkun.de/paper/ou2026trustcalib.pdf)
- [Short-Form Video and Prospective Memory](https://changkun.de/paper/tiktok.pdf)

## One-Sentence Summary

This page keeps the way formal research training organized interaction, behavior, optimization, adaptive systems, and case domains into an evolving research line, rather than reducing the story to a list of papers.
