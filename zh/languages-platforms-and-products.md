# 知识：编程语言、平台与产品感

[![English](https://img.shields.io/badge/Language-English-111827)](../languages-platforms-and-products.md)

编程语言、平台生态和产品体验，构成了另一条长期稳定的观察线。

如果系统页更关注软件如何运转，这一页更关注软件如何被设计、包装、交付和体验。

在基础层里，这一页补的是系统页较少展开的部分：语言设计、平台迁移和产品边界。

## 编程语言观

在 [changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/](https://changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/) 里，重点落在：

- 语言的运行时机制差异
- 静态绑定与动态绑定
- 编译期与运行期的职责划分
- 不同范式背后的设计思想

语言在这里也是理解程序组织方式的入口，同时影响对系统的判断。

## 平台迁移经验

Apple 和 Mac 这条经验线延续了很长时间。

- 从 iPhone 开始，对 Apple 产品建立了产品层面的信任。
- 很早就系统写过 [changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/](https://changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/)。
- 对 WatchKit、Swift、Apple Watch 交互、平台限制等都做过快速而具体的跟进。

这里更有价值的是：

- 会主动比较平台的整体体验与工具链生态。
- 会把平台能力和用户体验边界放在一起看。
- 很早就意识到硬件、系统和交互设计之间是相互联动的。

## 交互原型与设备实验

- Demo、本科论文与 AugmentedTouch 这类项目页共同指向一条更早的设备交互线。
- 早期做过 Windows 手势识别软件 Demo，后来又做了智能手表非接触式控制、本科论文相关原型，以及 AugmentedTouch 这样的交互技术项目。
- 这说明“产品感”也直接落在摄像头、手势、可穿戴设备和交互原型上的实践中。

## 从设备到平台产品

- 2016 年的实习经历里已经出现跨平台桌面应用，这和后面写博客客户端、实践 Electron 的路线是接上的。
- 2017-2018 年做过面向语言学习者的实时语音机器人，覆盖 Web 与 Amazon Alexa，这让语音、平台限制和产品反馈之间的真实工程经验也进入了这条线。
- 2018-2019 年又做过 remote desktop proxy、多云资源管理和容器、实例混合管理服务，说明产品感也体现在复杂平台能力的抽象方式上。
- 2022 年之后则把这条线推进到企业产品层：AI 对话界面、自助式智能体构建器、低代码平台、文档处理流水线、知识系统。
- 这里的“产品感”因此跨过了设备交互、桌面端、语音端、云平台与企业 AI 工具链，并未停留在某一种终端或某一个框架上。

## 产品判断

这类判断往往隐藏在技术文背后。

- 对 Apple 产品和工业设计有持续兴趣。
- 在早年总结中提到，自己通过大量设备评测、Google I/O、WWDC 等内容逐渐接触工业设计与商业。
- 在人机交互学习之后，产品感逐渐从审美偏好转化为“人应被放在第一位”的理解；可穿戴、语音、浏览行为和自助式智能体构建器这些经历里都能看到这一点。

## 小型产品实验

博客多次被当作产品来做，文章只是其中一种内容形态。

- 做过博客客户端。
- 做过桌面客户端。
- 做过移动客户端相关尝试。
- 做过 RESTful API 与站点侧边栏下载入口等产品化小实验。
- 还曾系统总结过 Electron 跨平台客户端实践，说明这种实践经过了完整复盘，认真处理过产品工程化中的问题。

“给自己做一个产品”在这里是一种长期倾向。

## 这一页和系统页的区别

- 系统页更偏运行时、内核、性能、部署。
- 这一页更偏语言设计、平台体验、产品边界与交互手感。

## 参考文章与页面

- [changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/](https://changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/)
- [changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/](https://changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/)
- [changkun.de/blog/posts/2014-11-20-WatchKit框架与WatchApp交互初窥/](https://changkun.de/blog/posts/2014-11-20-WatchKit框架与WatchApp交互初窥/)
- [changkun.de/blog/posts/2016-05-11-swiftapi/](https://changkun.de/blog/posts/2016-05-11-swiftapi/)
- [changkun.de/blog/demo/](https://changkun.de/blog/demo/)
- [changkun.de/blog/bachelorthesis/](https://changkun.de/blog/bachelorthesis/)
- [changkun.de/blog/augmentedtouch/](https://changkun.de/blog/augmentedtouch/)
- [changkun.de/blog/clients/](https://changkun.de/blog/clients/)
- 未发布草稿《基于 Electron 编写跨平台客户端的若干实践》
- [changkun.de/blog/posts/2016-09-04-博客客户端发布/](https://changkun.de/blog/posts/2016-09-04-博客客户端发布/)
- [changkun.de/blog/posts/2017-03-14-Electron-深度实践总结/](https://changkun.de/blog/posts/2017-03-14-Electron-深度实践总结/)

## 一句话总结

这里的语言与平台兴趣，本质上是通过工具链、交互方式和产品边界去理解软件应当怎样被设计和使用。
