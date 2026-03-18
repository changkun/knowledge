# 知识：数学与学习理论

[![English](https://img.shields.io/badge/Language-English-111827)](../math-and-learning.md)

数学在这里是一种组织对象、压缩定义和解释学习问题的语言，也构成方法习惯的一部分。

在整套知识地图里，这一页处在基础层的最底部。后面在[系统与工程](systems-and-engineering.md)中的判断、[博士阶段](doctoral-training-and-research-formation.md)形成的研究问题和写作习惯，很多都能追溯到这里的公理化倾向和定义意识。

## 形成过程

后来工作中可见的数学气质，大致在 2009 到 2013 年间成形。2009 年关于瑕积分的写作已经显示出一种偏好：宁可自己推导边界行为，也不愿接受现成的公式套路。2011 年用拓扑方法证明素数无穷多，标志着跨领域结构性推理的转向。2012 年关注点移向基础问题：良序原理，以及证明加法交换律在线性空间公理体系中是独立的。到 2013 年，ZFC 公理已不再被当作背景假设，而是可以逐条检验其必要性的构造工具；同期的流形读书笔记从 Riemann 追溯到现代形式化。贯穿这段时期的核心问题始终是"为什么要这样定义"，而非"这个定理怎么用"——这个习惯延续到了此后所有数学和研究工作中。

## 核心知识

- 集合论与公理化：长期关注集合、关系、函数、序、良序、基础公理与对象构造方式，强调"对象为何存在""性质如何被实体化"。例如，ZFC 的文章逐条去掉公理、观察哪些东西会坍塌；线性空间的文章证明了加法交换律在其余公理下是多余的。两者体现同一个习惯：检验定义中的每一条是否真的必要。
- 证明结构与定义意识：不满足于会用定理，更关心为什么这样定义，哪些公理是必要的，哪些只是历史上的方便写法。
- 概率与统计学习理论：把学习问题理解为风险最小化与经验风险最小化之间的一致性问题，不会只把机器学习理解成调参。核心洞察在于，经典统计只保证逐点收敛，这对高维学习是不够的；Vapnik 的贡献是指出经验风险最小化的一致性要求函数族上的一致收敛——本质上是把大数定律提升到函数空间。后来的文章（2017—2018）进一步区分了规定性理论（提供能实际指导架构或训练选择的界）和仅仅描述性的理论（事后给现象贴标签，却不约束实践）。
- 泛函分析与泛化理论：关注泛函空间大数定律、一致收敛、VC/Rademacher/PAC-Bayes、压缩法、平坦极小值、噪声稳定性等主题。
- 计算机视觉中的数学建模：曾系统写过 Kalman 滤波、MeanShift、Fourier 变换、图像信号相关性、边界积分匹配等内容。
- 数学建模与可讲授化：不仅研究理论，也多次把概率、马尔可夫链、蒙特卡洛、排队论、隐马尔可夫模型、不动点等主题组织成教程、视频和建模问题。

## 典型思考方式与知识侧重点

- 关注点落在一个理论系统如何被搭起来，重心不在解题技巧本身。先解释"为什么这样定义"，再解释"这个定义能做什么"。
- 对纯经验主义保持警惕，反复追问收敛条件、有效复杂度、稳定性、可压缩性和边界。
- 不只接受"这在工程上能用"，还会追问它为什么在某些条件下成立，或者为什么根本不该被过度解释。
- 倾向把机器学习问题重新翻译成数学问题，例如函数空间、一致收敛、复杂度度量和误差传播。
- 对深度学习的关注更偏理论解释，尤其是泛化性、压缩、稳定秩、样本复杂度这些母题。
- 会继续把抽象理论压缩成可讲授、可模拟、可编程的对象，不满足于停留在纸面证明。
- 数学兴趣也延伸到集合论、流形、测度、Riemann 等更基础的问题。
- 未发布草稿里还能看到一条尚未完全展开的数学长线：不等式证明、Fermat 数、三维复数、单值函数论到流形思想、统计学习理论综述等。

## 参考文章与页面

- [changkun.de/blog/posts/2009-08-20-小谈瑕积分/](https://changkun.de/blog/posts/2009-08-20-小谈瑕积分/)
- [changkun.de/blog/posts/2011-01-28-素数无穷多的拓扑学证明/](https://changkun.de/blog/posts/2011-01-28-素数无穷多的拓扑学证明/)
- [changkun.de/blog/posts/2012-06-28-谈谈良序原理/](https://changkun.de/blog/posts/2012-06-28-谈谈良序原理/)
- [changkun.de/blog/posts/2012-12-16-为什么要有特征值和特征向量/](https://changkun.de/blog/posts/2012-12-16-为什么要有特征值和特征向量/)
- [changkun.de/blog/posts/2012-12-26-谈线性空间定义中加法交换律独立性/](https://changkun.de/blog/posts/2012-12-26-谈线性空间定义中加法交换律独立性/)
- [changkun.de/blog/posts/2013-01-31-ZFC-集合论中各公理的意义及作用/](https://changkun.de/blog/posts/2013-01-31-ZFC-集合论中各公理的意义及作用/)
- [changkun.de/blog/posts/2013-03-25-又读流形/](https://changkun.de/blog/posts/2013-03-25-又读流形/)
- [changkun.de/blog/math-modeling/](https://changkun.de/blog/math-modeling/)
- [changkun.de/blog/posts/2013-08-29-Kalman滤波器数学原理与应用/](https://changkun.de/blog/posts/2013-08-29-Kalman滤波器数学原理与应用/)
- [changkun.de/blog/posts/2013-09-04-均值漂移跟踪算法原理/](https://changkun.de/blog/posts/2013-09-04-均值漂移跟踪算法原理/)
- [changkun.de/blog/posts/2013-10-07-Fourier变换应用小记/](https://changkun.de/blog/posts/2013-10-07-Fourier变换应用小记/)
- [changkun.de/blog/posts/2013-09-21-基于图像信号分析的碎纸片的拼接复原/](https://changkun.de/blog/posts/2013-09-21-基于图像信号分析的碎纸片的拼接复原/)
- [changkun.de/blog/posts/2015-02-17-什么是泛函空间的大数定律？它是机器学习理论的里程碑吗？/](https://changkun.de/blog/posts/2015-02-17-什么是泛函空间的大数定律？它是机器学习理论的里程碑吗？/)
- [changkun.de/blog/posts/2017-12-17-深度学习的泛化理论简介/](https://changkun.de/blog/posts/2017-12-17-深度学习的泛化理论简介/)
- [changkun.de/blog/posts/2018-01-28-Generalization-in-Deep-Learning/](https://changkun.de/blog/posts/2018-01-28-Generalization-in-Deep-Learning/)
- [changkun.de/blog/specialization/](https://changkun.de/blog/specialization/) 中的 UMSLT 系列与建模、机器学习教程索引
- 2018《UMSLT01-04》
- [changkun.de/blog/posts/2018-03-26-压缩法与深度网络的泛化性/](https://changkun.de/blog/posts/2018-03-26-压缩法与深度网络的泛化性/)
- 未发布草稿《统计学习理论综述》《浅谈不等式证明二三事》《Hamilton 找不到「三维复数」的原因》

## 一句话总结

这里的数学气质，核心落在公理化、结构化、可证明性，以及把机器学习重新拉回理论基础的倾向，重心不在竞赛式技巧。
