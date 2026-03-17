# 知识：开源、演讲与公共输出

这里讨论的是“面向他人的技术输出”。

如果其他专题页更偏知识结构本身，这里关注的是这些结构如何被公开、传播并组织成可复用资产。

如果教学页主要处理课堂和培养关系，这一页处理的则是另一种公共化：仓库、社区、站点、演讲、翻译、模板和知识基础设施。

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

- 公开统计条目给出了更硬的规模信息：20.8k+ GitHub stars、14.9k+ commits、20+ 开源项目。
- 公开贡献排名把这条线进一步坐实为长期身份，而不只是爱好者活动: top-200 active developer in Germany。
- 在 Go 社区并不是外围参与，而是 official Go organization member、`x/mobile` maintainer，并持续向 runtime 和 standard library 贡献。
- 在 fyne 里也不是一次性 PR，而是 organization member，长期关注 graphics driver 与 performance。
- `golang.design`、TalkGo、翻译社区与教程项目共同说明，公共输出的单位不是单篇文章，而是组织、站点、社区和一组长期资产。

## 早期形态：项目与教程

2018 年前后已经能看到相当完整的一批公开知识仓库：

- `modern-cpp-tutorial`
- `ws-18-19-deep-learning-tutorial`
- `ss18-machine-learning-tutorial`
- `translation`
- `applied-ml`
- `theoretical-ml`
- `computer-networks`
- `lmu-thesis-latex`

这说明公共输出并不是 2020 年之后才出现，而是在研究生阶段已经形成；而且形式也不只是一组代码仓库，而是书、课程、阅读清单、模板和翻译目录。

## 仓库本身就是知识产品

GitHub 上有一批仓库并不是“代码项目顺手带 README”，而是直接以知识组织为主体：

- `modern-cpp-tutorial` 是完整的书，而不是某个库的文档。
- `computer-networks` 是 lecture notes。
- `translation` 是持续维护的笔译作品目录。
- `applied-ml` 与 `theoretical-ml` 是阅读清单与研究输入结构。
- `lmu-thesis-latex` 则把学术写作经验沉淀成可复用模板。

这很重要，因为它说明公共输出的习惯不是“做完项目再写一篇介绍”，而是习惯直接把知识做成可以被别人学习、复用、继续扩展的公共资产。

## Go 作为公共输出放大器

2019-2021 是最强烈的放大期。

- 2019 年通过《Go 语言原本 / Go Under the Hood》进入更大的 Go 社区。
- 参与 Go 夜读、Go 社区活动、欧洲 Go Contributor Summit。
- 持续产出 Go 性能、运行时、benchmark、内存管理相关内容。
- 2020 年建立 `golang.design`，把分散资源重新组织成一个长期站点与项目集合。

关键不在于“写了几篇 Go 文章”，而在于形成了一个完整的公共输出面：

- 文章
- 仓库
- 域名
- 工具
- 演讲
- 社区连接
- 播客

## 研究工件与知识可复现性

研究输出也并不只停在论文标题。

- `dissertation`、`intelligence-in-the-loop`、`rankui`、`expertise-loop` 等仓库表明，公开输出还包括 thesis source、dataset、analysis script 与复现实验。
- 这说明这里对“公开”二字的理解，不只是把结论放出来，而是尽量把通向结论的工件也组织出来。
- 这种习惯与工程气质是一致的：更偏向可重建、可追踪、可复核的公共知识，而不是只给摘要。

## 翻译与知识基础设施

翻译并不是边角料。

- 在 2017、2018、2019 的总结里，翻译工作被持续提到。
- 这条线也长期落实为正式公共角色，例如翻译 50+ 英文文章进入中文社区。
- 这说明“把外部知识迁移进中文世界”是稳定自我定位的一部分。
- 它与写作观高度一致：不仅吸收知识，还希望重组后公开给别人使用。

与翻译相邻的，还有一类更底层的知识基础设施：

- `ideas` 把灵感捕获、双语整理和发布流程做成了服务。
- `lmu-thesis-latex`、`SWUNThesis` 这类模板把“如何把知识写成正式文档”也做成了公共工具。
- 这说明对公共输出的理解不仅是内容生产，还包括内容生产工具链本身。

## 演讲与播客

从 2019、2020 总结看，公开演讲和播客开始成为新的输出渠道。

- Go Nights 分享
- `gobench` 等主题演讲
- `talkgo.fm`
- 与社区核心人物的交流和录制

这意味着输出形式从文章扩展到了声音和现场表达。

## 公共输出的共同特征

- **组织欲很强**：喜欢把分散知识做成系列。
- **寿命意识很强**：希望内容能跨越短期热度继续有价值。
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

## 一句话总结

这里的开源与公共输出，不只是“把代码放上 GitHub”，而是持续把知识、经验、研究工件、模板、工具和社区关系组织成可传播的公共结构。
