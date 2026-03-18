# Knowledge: Systems and Engineering

[![中文](https://img.shields.io/badge/Language-%E4%B8%AD%E6%96%87-0A66C2)](zh/systems-and-engineering.md)

The focus here is "underlying mechanism + runnable system," rather than following framework churn.

If the [mathematics page](math-and-learning.md) answers how objects and theories are built, this page asks how those structures become runnable, deployable, and maintainable systems. Within the foundation layer, it sits between mathematics and [languages, platforms, and products](languages-platforms-and-products.md), which picks up where this page leaves off on language design and product boundaries.

## Core Capabilities

- Language foundation: C/C++ served as the early base, Go became the main engineering language later, while Python, JavaScript, Lua, and others were used more as problem-driven tools.
- Operating systems and runtime: sustained writing on Linux kernel experiments, the Go runtime and scheduler, `sync.Pool`, `unsafe`, memory management, and system-call-related topics.
- Performance analysis: high sensitivity to benchmark distortion, the extra cost of `StopTimer/StartTimer`, page faults versus prefetching, `MADV_DONTNEED` / `MADV_FREE`, and RSS/PSS/USS. The recurring lesson across these investigations is that measurement infrastructure is never transparent: `time.Now()` itself costs ~16 ns, and timer interruption between `StopTimer`/`StartTimer` introduces systematic bias large enough to invalidate published benchmarks. The same pattern appears in parameter-passing: the common advice to pass large structs by pointer turns out to be wrong in many cases, because inlining and addressing-mode effects make value parameters faster — performance depends on compiler optimization paths, not on surface-level calling conventions. Memory metrics carry the same trap: after Go 1.12 switched to `MADV_FREE`, RSS no longer reflects actual consumption without understanding the kernel's lazy-reclaim semantics, and whether an access triggers a page fault or a hardware prefetch depends on the memory-access pattern, not on the amount of memory allocated. In each case, the real performance model lives one or two layers below the API that most engineers treat as ground truth.
- System infrastructure: long-term maintenance of a personal site across WordPress, Hexo, GitHub Pages, CI/CD, Nginx, Docker, Traefik, and finally a pure Go stack.
- Engineering operations: Docker tutorials, automated deployment, zero-downtime migration, HTTPS, log analysis, databases, and service setup.
- Production system building: later work extends this line into cross-platform desktop applications, real-time voice bots, remote desktop proxies, multi-cloud resource management, revenue optimization, knowledge systems, LLM gateways, workflow orchestration, low-code platforms, and document-processing pipelines.
- Mechanism notes: public short notes keep tracking `io/fs`, error-handling proposals, asynchronous preemption, the GC pacer, memory models, goroutine identifiers, Apple Silicon, timer optimizations, and similar topics. These notes are not topic bookmarks; each one traces a question across the full stack — from language semantics through runtime implementation to kernel behavior and hardware constraints — before settling on a judgment. The method is the same whether the subject is a scheduler change or a filesystem interface: refuse the surface explanation, follow the mechanism until the cost model becomes concrete. Several of these investigations — on benchmarking methodology, channel abstractions, pointer analysis, and scheduling — were also written up as formal research papers through [golang.design](https://golang.design/research/), crossing the boundary from engineering shorthand into published methodology.

## Production-System Trajectory

- The 2016 internship already involved a cross-platform desktop client, a recommendation system, and an ELK logging system, showing that the engineering line entered full system implementation and product delivery early.
- The startup and remote-work phase from 2017 to 2019 pushed this line into real-time voice, remote desktop proxying, multi-cloud abstraction, and Kubernetes-like hybrid management services.
- These experiences turned platforms, protocols, deployment, and scalability into real service systems that supported growth from 5k to 30k users.
- After 2022, enterprise work expanded this into automated pricing, revenue optimization, AI security and governance, a centralized LLM gateway, company-wide knowledge management, and workflow orchestration.
- A 300x performance gain, support for a 10x business scale-up, and roughly 2.5% margin improvement show that the engineering work produces system-level outcomes in real business structures.

## Engineering Preferences

- Mechanism first: performance problems are not left to guesswork; the habit is to experiment, read implementations, and inspect system behavior directly. In practice this means tracing a performance question from the Go compiler's inlining decisions through the runtime's memory-return policy down to the kernel's page-fault handler, rather than stopping at the API level.
- Dependency restraint: prefer implementing directly when reasonable; when dependencies are necessary, prefer structurally simple, controllable, long-lived options.
- Simple architecture: favor systems with fewer layers, less magic, and clearly explainable responsibilities.
- Go preference: the choice of Go as the main language is a judgment call based on maintainability, deployment cost, and system coherence, not on language popularity.
- Production awareness: the concern is not only whether code runs, but also deployment, monitoring, migration, rollback, long-term maintenance, and data safety.
- Compressed expression: local mechanism questions are often written as short notes that keep only judgments, constraints, and key conclusions.

## Typical Questions

- What does a metric actually measure, and how much of it is polluted by the tool itself?
- Does a performance gap come from the language, the runtime, the kernel, or hardware behavior?
- Is the complexity of a service architecture genuinely necessary, or just historical baggage?
- Can a technology stack still be reproduced cleanly on new machines, or has ecosystem drift already broken it?

## References

- [changkun.de/blog/posts/2013-03-31-my-string-copystr-v2/](https://changkun.de/blog/posts/2013-03-31-my-string-copystr-v2/)
- [changkun.de/blog/posts/2013-05-07-结构体排序引发的一连串问题/](https://changkun.de/blog/posts/2013-05-07-结构体排序引发的一连串问题/)
- The Linux, Docker, C++, and systems-tutorial index in [changkun.de/blog/specialization/](https://changkun.de/blog/specialization/)
- 2015 series: `Linux Kernel Analysis`
- [changkun.de/blog/posts/2016-08-07-Docker-极速入门教程1-基本概念和操作/](https://changkun.de/blog/posts/2016-08-07-Docker-极速入门教程1-基本概念和操作/) / [changkun.de/blog/posts/2016-08-07-Docker-极速入门教程2-镜像与容器管理/](https://changkun.de/blog/posts/2016-08-07-Docker-极速入门教程2-镜像与容器管理/)
- [changkun.de/blog/posts/2016-08-21-Guacamole-与-VNC-的坑/](https://changkun.de/blog/posts/2016-08-21-Guacamole-与-VNC-的坑/)
- [changkun.de/blog/posts/2017-06-21-Hexo-GitHub-Travis-CI-VPS-自动部署/](https://changkun.de/blog/posts/2017-06-21-Hexo-GitHub-Travis-CI-VPS-自动部署/)
- Unpublished draft: `Go Web in 1 Hour`
- [changkun.de/blog/posts/2018-03-21-Go-in-1-Hour/](https://changkun.de/blog/posts/2018-03-21-Go-in-1-Hour/)
- [changkun.de/blog/posts/2018-09-23-Go-runtime-programming/](https://changkun.de/blog/posts/2018-09-23-Go-runtime-programming/)
- [changkun.de/blog/posts/2018-09-26-sync-Pool-源码精读/](https://changkun.de/blog/posts/2018-09-26-sync-Pool-源码精读/)
- [changkun.de/blog/posts/2020-09-30-A-Source-of-Errors-in-Go-Benchmarking/](https://changkun.de/blog/posts/2020-09-30-A-Source-of-Errors-in-Go-Benchmarking/)
- [changkun.de/blog/posts/2020-12-24-all-in-go/](https://changkun.de/blog/posts/2020-12-24-all-in-go/)
- [changkun.de/blog/posts/2020-12-28-zero-downtime-migration/](https://changkun.de/blog/posts/2020-12-28-zero-downtime-migration/)
- 2020-2021 public notes: `Revisiting Asynchronous Preemption`, `A New GC Pacer`, `Data Races and the Memory Model`
- [changkun.de/blog/posts/2021-01-18-page-fault-vs-prefetch/](https://changkun.de/blog/posts/2021-01-18-page-fault-vs-prefetch/)
- [changkun.de/blog/posts/2021-01-23-pss-uss-rss/](https://changkun.de/blog/posts/2021-01-23-pss-uss-rss/)

## One-Sentence Summary

The engineering strength here is a systems-engineering habit of finding answers in source code, kernels, and operational reality, well beyond application-level assembly.
