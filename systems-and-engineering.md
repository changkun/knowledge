# 知识：系统与工程

工程关注的重点是“底层机制 + 可运行系统”，而不是框架追新。

如果说数学页回答的是“对象和理论怎样被搭起来”，这一页处理的就是这些结构怎样真正落地成可运行、可部署、可长期维护的系统。

## 核心能力

- 语言基础：C/C++ 是早期打底语言，Go 是近年的主力工程语言；Python、JavaScript、Lua 等更多作为问题驱动的工具。
- 操作系统与运行时：写过 Linux 内核实验、Go 运行时/调度器、`sync.Pool`、`unsafe`、内存管理与系统调用相关内容。
- 性能分析：对 benchmark 偏差、`StopTimer/StartTimer` 的额外成本、缺页与预取、`MADV_DONTNEED`/`MADV_FREE`、RSS/PSS/USS 非常敏感。
- 系统基础设施：长期维护个人站点，经历 WordPress、Hexo、GitHub Pages、CI/CD、Nginx、Docker、Traefik，再到纯 Go 技术栈。
- 工程运维：写过 Docker 教程、自动部署、零停机迁移、HTTPS、日志分析、数据库与服务搭建相关文章。
- 生产系统建设：后续工作又把这条线推进到更多正式系统类型，包括跨平台桌面应用、实时语音 bot、远程桌面代理、多云资源管理、收益优化、knowledge system、LLM gateway、workflow orchestration、低代码平台与文档处理流水线。
- 微观机制札记：公开短笔记持续记录 `io/fs`、错误处理提案、异步抢占、GC pacer、内存模型、goroutine id、Apple Silicon、计时器优化等问题。

## 生产系统轨迹

- 2016 的实习经历已经包含跨平台桌面客户端、推荐系统和 ELK logging system，这说明工程线一开始就不是纯算法练习。
- 2017-2019 的创业与远程工作阶段，把系统能力推进到实时语音、远程桌面代理、多云服务抽象和类似 Kubernetes 的混合管理服务。
- 这些经历让“平台、协议、部署、伸缩性”不只是文章中的知识点，而是实际支撑过 5k 到 30k 用户增长的服务系统。
- 2022 之后在企业里，这条线又升级为自动定价、收益优化、AI security/governance、centralized LLM gateway、company-wide knowledge management 与 workflow orchestration。
- 300x 的性能提升、10x 的业务规模支撑、约 2.5% 的利润率提升，说明这里的工程能力不是停留在技术偏好，而是能在真实业务结构中兑现为系统结果。

## 工程偏好

- 机制优先：不愿意把性能问题交给猜测，倾向自己做实验、读实现、看系统行为。
- 依赖克制：能自己实现就尽量不引入重依赖，必须依赖时也更偏向结构简单、可控、可长期维护的方案。
- 简洁架构：偏爱少层级、少魔法、能解释清楚每一层职责的系统。
- Go 倾向：喜欢 Go 的语言设计和工程落地方式，但不是宗教式推崇，而是基于可维护性、部署成本和系统一致性做选择。
- 生产意识：不仅关心代码能跑，还关心部署、监控、迁移、回滚、长期维护和数据安全。
- 压缩表达：愿意把一个局部机制问题写成很短的 note，只保留判断、约束和关键结论。

## 典型问题意识

- 一个指标到底测到了什么，是否被工具本身污染。
- 一段性能差异来自语言、运行时、内核还是硬件行为。
- 一个服务架构的复杂度是否真有必要，还是只是历史包袱。
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

这里的工程能力，本质上是一种“从源码、内核和运维现实里找答案”的系统工程能力，而不是停留在应用层的拼装能力。
