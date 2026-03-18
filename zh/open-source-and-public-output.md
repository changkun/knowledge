# 知识：开源、演讲与公共输出

[![English](https://img.shields.io/badge/Language-English-111827)](../open-source-and-public-output.md)

这里讨论的是面向他人的技术输出。

如果其他专题页更偏知识结构本身，这里关注的是这些结构如何被公开、传播并组织成可复用资产。

在输出层里，这一页处理的是课堂之外的公共化：仓库、社区、站点、演讲、翻译、模板和知识基础设施。它处在[教学与课程设计](teaching-and-course-design.md)和[写作、研究与文化世界](writing-and-culture.md)之间，前者处理知识如何在课程内部组织，后者处理公共表达背后的写作方法和文化取向。

## 输出形态

- 开源仓库
- 系列教程 / 书籍
- 论文与研究工件
- 演讲 slide 与公开分享
- 翻译项目
- 讲义 / 模板
- 播客与社区活动
- 个人站点与附属服务

## 组织性的公共角色

- 公开统计条目给出了更明确的规模信息：20.8k+ GitHub stars、14.9k+ commits、20+ 开源项目。
- 公开贡献排名也把这条线坐实为长期身份：德国最活跃开发者前 200。
- 在 Go 社区，同时承担 Go 官方组织成员、`x/mobile` 维护者等角色，并持续向运行时和标准库贡献。
- 在 Fyne 里的参与也延续到长期组织成员角色，持续关注图形驱动与性能。
- `golang.design`、TalkGo、翻译社区与教程项目共同说明，公共输出的单位已经扩展到组织、站点、社区和一组长期资产，不再局限于单篇文章。

## 早期形态：项目与教程

2018 年前后已经能看到一批成型的公开知识仓库，例如 `modern-cpp-tutorial`、机器学习教程仓库、`translation`、`computer-networks`、`lmu-thesis-latex`。公共输出在研究生阶段已经形成，2020 年之后只是继续扩展。其形式也覆盖书、课程、阅读清单、模板和翻译目录，不局限于一组代码仓库。

## 仓库本身就是知识产品

GitHub 上有一批仓库直接以知识组织为主体：

- `modern-cpp-tutorial` 是一本完整的书。
- `computer-networks` 是课程讲义。
- `translation` 是持续维护的笔译作品目录。
- 阅读清单与研究输入类仓库也把知识输入结构公开出来。
- `lmu-thesis-latex` 则把学术写作经验沉淀成可复用模板。

这说明公共输出的习惯是直接把知识做成可以被别人学习、复用、继续扩展的公共资产，形成了比项目介绍更完整的公共接口。

## Go 作为公共输出放大器

2019-2021 年是一个明显的放大期。

- 2019 年通过《Go 语言原本 / Go Under the Hood》进入更大的 Go 社区。
- 参与 Go 夜读、Go 社区活动、欧洲 Go Contributor Summit。
- 持续产出 Go 性能、运行时、基准测试、内存管理相关内容。
- 2020 年建立 `golang.design`，把分散资源重新组织成一个长期站点与项目集合。
- 除了代码和文档之外，golang.design 还产出了正式研究出版物：六篇关于 Go 并发、channel 设计、指针管理、基准测试、调度和 options 模式的论文以研究论文形式撰写，跨越了从工程文档到正式研究方法论的边界。

关键不在于"写了几篇 Go 文章"，而在于形成了一个完整的公共输出面：

- 文章
- 仓库
- 域名
- 工具
- 演讲
- 社区连接
- 播客

## 研究工件与知识可复现性

研究输出也没有停在论文标题。

- `dissertation`、`intelligence-in-the-loop`、`rankui`、`expertise-loop` 等仓库表明，公开输出还包括论文源码、数据集、分析脚本与复现实验。
- 这说明这里对“公开”的理解不仅包括结论，也尽量把通向结论的工件组织出来。
- 这种习惯与工程气质是一致的：更偏向可重建、可追踪、可复核的公共知识，材料通常比摘要更完整。

## 翻译与知识基础设施

翻译在这里也占据稳定位置，并非边角工作。

- 在 2017、2018、2019 的总结里，翻译工作被持续提到。
- 这条线也长期落实为正式公共角色，例如翻译 50+ 英文文章进入中文社区。
- “把外部知识迁移进中文世界”是稳定自我定位的一部分。
- 它与写作观高度一致：不仅吸收知识，还希望重组后公开给别人使用。

与翻译相邻的，还有一类更底层的知识基础设施：

- `ideas` 把灵感捕获、双语整理和发布流程做成了服务。
- `lmu-thesis-latex`、`SWUNThesis` 这类模板把“如何把知识写成正式文档”也做成了公共工具。
- 这说明对公共输出的理解不仅是内容生产，还包括内容生产工具链本身。

## 演讲与播客

演讲输出跨越十余年，其轨迹与语料库其他部分可见的知识发展路径一致。早期学术讲座涉及深度学习与泛化理论；在 TalkGo 和 GopherChina 的 Go 社区演讲处理 channel、CSP、并发 bug、计时器内部机制、基准测试与泛型；IUI 2023 和 MuC 2022 的正式研究会议报告将人在环工作带入 HCI 社区；企业工程演讲涵盖生产环境中的 PGO 优化和 AI-first 工作流设计；关于自由意志、决策困境和理性讨论的哲学类演讲则贯穿始终。这一轨迹并非随意扩展——它追踪着与整个语料库结构相同的路径：从技术基础到社区建设，再到正式研究，然后是企业应用。

- [changkun.de/talk/](https://changkun.de/talk/)

## 学术服务与社区认可

在 ACM CHI（2024、2025、2026）和 INTERACT（2025）担任 Associate Chair，表明本语料库其他部分所描述的研究身份在 HCI 社区具有认可度。在 CHI、INTERACT、ICMI、IMWUT 和 MobileHCI 的多年审稿工作代表了对研究质量管控的持续参与。2023 年获得 ACM SIGCHI 的 Gary Marsden Travel Award 进一步确认了这种认可。这里不是作为资历罗列，而是作为研究线具有外部认可的证据——这种认可来自多年的持续贡献，而非某一篇论文。

## 公共输出的共同特征

- **组织欲强**：喜欢把分散知识做成系列。
- **寿命意识强**：希望内容能跨越短期热度继续有价值。
- **不只写文章**：更偏向“知识产品化”。
- **基础设施意识强**：网站、域名、服务、重定向、部署本身也是输出的一部分。

## 参考文章与页面

- [changkun.de/blog/posts/2018-10-01-Go-source-code-study-is-now-open-source/](https://changkun.de/blog/posts/2018-10-01-Go-source-code-study-is-now-open-source/)
- [changkun.de/blog/posts/2018-12-27-2018-年终总结/](https://changkun.de/blog/posts/2018-12-27-2018-年终总结/)
- [changkun.de/blog/posts/2020-02-01-2019-年终总结/](https://changkun.de/blog/posts/2020-02-01-2019-年终总结/)
- [changkun.de/blog/posts/2021-01-03-2020-summary/](https://changkun.de/blog/posts/2021-01-03-2020-summary/)
- [changkun.de/blog/about/](https://changkun.de/blog/about/)
- [github.com/changkun/modern-cpp-tutorial](https://github.com/changkun/modern-cpp-tutorial)
- [github.com/changkun/translation](https://github.com/changkun/translation)
- [github.com/changkun/intelligence-in-the-loop](https://github.com/changkun/intelligence-in-the-loop)
- [github.com/changkun/lmu-thesis-latex](https://github.com/changkun/lmu-thesis-latex)
- [golang.design/research](https://golang.design/research/)
- [changkun.de/research/](https://changkun.de/research/)
- [changkun.de/talk/](https://changkun.de/talk/)

## 一句话总结

这里的开源与公共输出，持续把知识、经验、研究工件、模板、工具和社区关系组织成可传播的公共结构。
