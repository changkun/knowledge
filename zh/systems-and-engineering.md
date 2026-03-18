# 知识：系统与工程

[![English](https://img.shields.io/badge/Language-English-111827)](../systems-and-engineering.md)

这里关注的重点是"底层机制 + 可运行系统"，不追逐框架更新。

如果说[数学页](math-and-learning.md)回答的是"对象和理论怎样被搭起来"，这一页处理的就是这些结构怎样落地成可运行、可部署、可长期维护的系统。在基础层中，它处于数学与[编程语言、平台与产品感](languages-platforms-and-products.md)之间，后者补充的是语言设计和产品边界。

## 核心能力

- 语言基础：C/C++ 是早期打底语言，Go 是近年的主力工程语言；Python、JavaScript、Lua 等更多作为问题驱动的工具。
- 操作系统与运行时：写过 Linux 内核实验、Go 运行时与调度器、`sync.Pool`、`unsafe`、内存管理与系统调用相关内容。
- 性能分析：对基准测试偏差、`StopTimer/StartTimer` 的额外成本、缺页与预取、`MADV_DONTNEED`/`MADV_FREE`、RSS/PSS/USS 等问题非常敏感。这些研究反复揭示的是：测量工具本身从来不是透明的——`time.Now()` 本身就有约 16 ns 的开销，而 `StopTimer`/`StartTimer` 之间的计时器中断引入的系统性偏差足以让已发表的基准测试结果失效。同样的规律出现在参数传递问题上：常见的"大结构体用指针传"的建议在很多场景下是错的，因为内联和寻址模式效应往往让值参数更快——性能取决于编译器的优化路径，而不是表面的调用约定。内存指标同样隐藏着陷阱：Go 1.12 切换到 `MADV_FREE` 之后，RSS 不再反映真实内存消耗，除非你理解内核的惰性回收语义；而一次内存访问走的是缺页中断还是硬件预取，取决于访问模式而非分配量。每一个案例中，真正的性能模型都藏在大多数工程师当作事实的 API 下面一两层。
- 系统基础设施：长期维护个人站点，经历 WordPress、Hexo、GitHub Pages、CI/CD、Nginx、Docker、Traefik，再到纯 Go 技术栈。
- 工程运维：写过 Docker 教程、自动部署、零停机迁移、HTTPS、日志分析、数据库与服务搭建相关文章。
- 生产系统建设：后续工作又把这条线推进到更多正式系统类型，包括跨平台桌面应用、实时语音机器人、远程桌面代理、多云资源管理、收益优化、知识系统、LLM 网关、工作流编排、低代码平台与文档处理流水线。
- 微观机制札记：公开短笔记持续记录 `io/fs`、错误处理提案、异步抢占、GC pacer、内存模型、goroutine id、Apple Silicon、计时器优化等问题。这些笔记不是主题书签，每一篇都把一个问题从语言语义追踪到运行时实现、再到内核行为和硬件约束，直到形成判断为止。无论主题是调度器改动还是文件系统接口，方法始终相同：拒绝表面解释，沿着机制一路追到成本模型变得具体为止。其中若干研究——关于基准测试方法论、channel 抽象、指针分析和调度——还通过 [golang.design](https://golang.design/research/) 撰写为正式研究论文，跨越了从工程速记到发表方法论的边界。

## 生产系统轨迹

- 2016 年的实习经历已经包含跨平台桌面客户端、推荐系统和 ELK logging system，说明工程线一开始就已经进入完整的系统实现与产品交付。
- 2017-2019 年的创业与远程工作阶段，把系统能力推进到实时语音、远程桌面代理、多云服务抽象和类似 Kubernetes 的混合管理服务。
- 这些经历让平台、协议、部署和伸缩性直接落到支撑过 5k 到 30k 用户增长的服务系统上。
- 2022 年之后在企业里，这条线又升级为自动定价、收益优化、AI 安全与治理、统一 LLM 网关、公司级知识管理与工作流编排。
- 300x 的性能提升、10x 的业务规模支撑、约 2.5% 的利润率提升，说明这里的工程能力能够在真实业务结构中兑现为系统结果。

## 工程偏好

- 机制优先：不愿意把性能问题交给猜测，倾向自己做实验、读实现、看系统行为。实际操作中，这意味着把一个性能问题从 Go 编译器的内联决策追到运行时的内存归还策略，再追到内核的缺页处理路径，而不是停在 API 层面。
- 依赖克制：能自己实现就尽量不引入重依赖；必须依赖时，也更偏向结构简单、可控、可长期维护的方案。
- 简洁架构：偏爱少层级、少魔法、能解释清楚每一层职责的系统。
- Go 倾向：选择 Go 作为主力语言是基于可维护性、部署成本和系统一致性的判断，而非基于语言流行度。
- 生产意识：不仅关心代码能跑，还关心部署、监控、迁移、回滚、长期维护和数据安全。
- 压缩表达：愿意把一个局部机制问题写成很短的 note，只保留判断、约束和关键结论。

## 典型问题意识

- 一个指标到底测到了什么，是否被工具本身污染。
- 一段性能差异来自语言、运行时、内核还是硬件行为。
- 一个服务架构的复杂度是否真的必要，还是只是历史包袱。
- 一个技术栈是否能在新机器上稳定复现，还是已经被生态变化拖垮。

## 参考文章与页面

- [changkun.de/blog/posts/2013-03-31-my-string-copystr-v2/](https://changkun.de/blog/posts/2013-03-31-my-string-copystr-v2/)
- [changkun.de/blog/posts/2013-05-07-结构体排序引发的一连串问题/](https://changkun.de/blog/posts/2013-05-07-结构体排序引发的一连串问题/)
- [changkun.de/blog/specialization/](https://changkun.de/blog/specialization/) 中的 Linux、Docker、C++ 项目与系统教程索引
- 2015《Linux 内核分析》系列
- [changkun.de/blog/posts/2016-08-07-Docker-极速入门教程1-基本概念和操作/](https://changkun.de/blog/posts/2016-08-07-Docker-极速入门教程1-基本概念和操作/) / [changkun.de/blog/posts/2016-08-07-Docker-极速入门教程2-镜像与容器管理/](https://changkun.de/blog/posts/2016-08-07-Docker-极速入门教程2-镜像与容器管理/)
- [changkun.de/blog/posts/2016-08-21-Guacamole-与-VNC-的坑/](https://changkun.de/blog/posts/2016-08-21-Guacamole-与-VNC-的坑/)
- [changkun.de/blog/posts/2017-06-21-Hexo-GitHub-Travis-CI-VPS-自动部署/](https://changkun.de/blog/posts/2017-06-21-Hexo-GitHub-Travis-CI-VPS-自动部署/)
- 未发布草稿《Go Web in 1 Hour》
- [changkun.de/blog/posts/2018-03-21-Go-in-1-Hour/](https://changkun.de/blog/posts/2018-03-21-Go-in-1-Hour/)
- [changkun.de/blog/posts/2018-09-23-Go-runtime-programming/](https://changkun.de/blog/posts/2018-09-23-Go-runtime-programming/)
- [changkun.de/blog/posts/2018-09-26-sync-Pool-源码精读/](https://changkun.de/blog/posts/2018-09-26-sync-Pool-源码精读/)
- [changkun.de/blog/posts/2020-09-30-A-Source-of-Errors-in-Go-Benchmarking/](https://changkun.de/blog/posts/2020-09-30-A-Source-of-Errors-in-Go-Benchmarking/)
- [changkun.de/blog/posts/2020-12-24-all-in-go/](https://changkun.de/blog/posts/2020-12-24-all-in-go/)
- [changkun.de/blog/posts/2020-12-28-zero-downtime-migration/](https://changkun.de/blog/posts/2020-12-28-zero-downtime-migration/)
- 2020-2021 年的公开短笔记：`回顾异步抢占`、`全新的 GC 调步器`、`数据竞争和内存模型`
- [changkun.de/blog/posts/2021-01-18-page-fault-vs-prefetch/](https://changkun.de/blog/posts/2021-01-18-page-fault-vs-prefetch/)
- [changkun.de/blog/posts/2021-01-23-pss-uss-rss/](https://changkun.de/blog/posts/2021-01-23-pss-uss-rss/)

## 一句话总结

这里的工程能力，本质上是一种从源码、内核和运维现实里找答案的系统工程能力，已经超出应用层的拼装能力。
