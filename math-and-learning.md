# Knowledge: Mathematics and Learning Theory

[![中文](https://img.shields.io/badge/Language-%E4%B8%AD%E6%96%87-0A66C2)](zh/math-and-learning.md)

Mathematics is treated here as a language for organizing objects, compressing definitions, and explaining learning problems. It also forms part of a durable method habit.

Within the overall map, this page sits at the lowest layer of the foundation. Many later judgments on [systems and engineering](systems-and-engineering.md), research questions formed during [doctoral training](doctoral-training-and-research-formation.md), and writing habits can be traced back to the axiomatic tendency and definition-sensitivity established here.

## Formation

The mathematical temperament visible in later work took shape between roughly 2009 and 2013. Early writing on improper integrals (2009) already shows a preference for working out boundary behavior rather than accepting a recipe. By 2011 a topological proof that infinitely many primes exist marked a shift toward structural reasoning across domains. In 2012 the focus moved to foundational questions: the well-ordering principle, and a proof that additive commutativity is independent of the other linear-space axioms. By 2013 the ZFC axioms were being treated not as background assumptions but as construction tools whose individual necessity could be tested, and a historical survey of manifolds traced the concept from Riemann through modern formalization. Throughout this period the recurring question was "why this definition?" rather than "how to use this theorem" -- a habit that persisted into all later mathematical and research work.

## Core Knowledge

- Set theory and axiomatization: long-term attention to sets, relations, functions, order, well-ordering, foundational axioms, and ways of constructing objects, with repeated emphasis on why an object exists and how a property is made concrete. For example, the ZFC post asks what breaks when each axiom is removed one at a time; the linear-space post proves that additive commutativity is redundant given the remaining axioms. Both reflect the same habit: testing whether each piece of a definition is genuinely necessary.
- Proof structure and definition awareness: the interest is not limited to using theorems, but extends to why a definition is made in a particular way, which axioms are necessary, and which are merely historical conveniences.
- Probability and statistical learning theory: learning is understood as a question of consistency between risk minimization and empirical risk minimization, not merely as parameter tuning. The core insight is that classical statistics only guarantees pointwise convergence, which is insufficient for high-dimensional learning; Vapnik's contribution is to show that consistency of empirical risk minimization requires uniform convergence across function families -- effectively a law of large numbers lifted into function space. Later posts (2017--2018) sharpen the distinction between prescriptive theory, which provides bounds that actually guide architectural or training choices, and merely descriptive theory, which labels a phenomenon after the fact without constraining practice.
- Functional analysis and generalization theory: recurring topics include laws of large numbers in function spaces, uniform convergence, VC/Rademacher/PAC-Bayes, compression-based arguments, flat minima, and noise stability.
- Mathematical modeling in computer vision: sustained writing on Kalman filtering, MeanShift, Fourier transforms, image-signal correlation, and boundary-integral matching.
- Mathematical modeling as something teachable: the work does not stop at theory, but repeatedly reorganizes probability, Markov chains, Monte Carlo, queueing theory, hidden Markov models, and fixed points into tutorials, videos, and modeling problems.

## Typical Way of Thinking and Main Emphasis

- The emphasis is on how a theoretical system is built, not on puzzle-solving technique. Explain why a definition is set up as it is before explaining what it can do.
- Stay cautious about pure empiricism and keep asking about convergence conditions, effective complexity, stability, compressibility, and boundaries.
- Engineering usefulness is not enough on its own; the question remains why something works under certain conditions, or why it should not be overinterpreted.
- Translate machine learning questions back into mathematical ones such as function spaces, uniform convergence, complexity measures, and error propagation.
- Deep learning is approached mainly through theory, especially generalization, compression, stable rank, and sample complexity.
- Keep compressing abstract theory into objects that can be taught, simulated, and programmed, rather than leaving it as paper proof alone.
- The mathematical interest also reaches into more basic topics such as set theory, manifolds, measure, and Riemannian thinking.
- Unpublished drafts still show a partly uncollapsed mathematical line: inequality proofs, Fermat numbers, three-dimensional complex numbers, single-valued function theory, manifolds, and overviews of statistical learning theory.

## References

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
- The UMSLT series and the modeling / machine-learning tutorial index in [changkun.de/blog/specialization/](https://changkun.de/blog/specialization/)
- 2018 series: `UMSLT01-04`
- [changkun.de/blog/posts/2018-03-26-压缩法与深度网络的泛化性/](https://changkun.de/blog/posts/2018-03-26-压缩法与深度网络的泛化性/)
- Unpublished drafts: `A Survey of Statistical Learning Theory`, `A Few Notes on Inequality Proofs`, `Why Hamilton Could Not Find a "Three-Dimensional Complex Number"`

## One-Sentence Summary

The mathematical temperament here is defined by axiomatization, structure, provability, and the tendency to pull machine learning back toward theoretical foundations rather than toward competition-style technique.
