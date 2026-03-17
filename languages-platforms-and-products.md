# Knowledge: Programming Languages, Platforms, and Product Judgment

[![中文](https://img.shields.io/badge/Language-%E4%B8%AD%E6%96%87-0A66C2)](zh/languages-platforms-and-products.md)

Programming languages, platform ecosystems, and product experience form another long-running line of observation.

If the [systems page](systems-and-engineering.md) is more concerned with runtime, kernels, performance, and deployment, this page is more concerned with how software is designed, packaged, delivered, and experienced.

Within the foundation layer, this page fills in what the systems page leaves less developed: language design, platform migration, and product boundaries.

## View of Programming Languages

In [changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/](https://changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/), the emphasis falls on:

- differences in runtime mechanisms
- static versus dynamic binding
- the division of responsibility between compile time and run time
- the design ideas behind different paradigms

Languages function here as an entry point into how programs are organized, and they shape system judgment as well.

## Platform Migration Experience

The Apple and Mac line runs for a long time.

- Product-level trust in Apple starts with the iPhone.
- A systematic early reflection appears in [changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/](https://changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/).
- WatchKit, Swift, Apple Watch interaction, and platform constraints all receive quick and concrete follow-up.

What matters more here is:

- a habit of comparing whole-platform experience with toolchain ecology
- a tendency to look at platform capability and user-experience boundaries together
- early recognition that hardware, systems, and interaction design move together

## Interaction Prototypes and Device Experiments

- Demo pages, the bachelor's thesis, and projects like AugmentedTouch all point to an earlier device-interaction line.
- Early work includes a Windows gesture-recognition demo, later contact-free smartwatch control, thesis-related prototypes, and interaction-technology projects such as AugmentedTouch.
- Product judgment therefore appears directly in hands-on work with cameras, gestures, wearables, and interaction prototypes.

## From Devices to Platform Products

- The 2016 internship already includes a cross-platform desktop application, which connects directly to later blog clients and Electron practice.
- In 2017-2018, a real-time voice bot for language learners was built across the web and Amazon Alexa, bringing real engineering experience with voice, platform constraints, and product feedback into this line.
- In 2018-2019, remote desktop proxying, multi-cloud resource management, containers, and hybrid instance-management services show that product judgment also appears in how complex platform capability is abstracted.
- After 2022, this line extends into enterprise products: AI chat interfaces, self-service agent builders, low-code platforms, document-processing pipelines, and knowledge systems.
- Throughout this line, the blog itself has repeatedly been treated as a product: blog clients, desktop clients, mobile-client experiments, RESTful APIs, and sidebar downloads on the site. A systematic retrospective on Electron-based cross-platform clients shows that product-engineering issues were fully worked through. "Build a product for oneself" is a durable tendency here.
- Product judgment here therefore spans device interaction, desktop software, voice interfaces, cloud platforms, and enterprise AI tooling rather than settling on a single terminal or framework.

## Product Judgment

Much of this judgment sits behind technical writing rather than in front of it.

- There is a sustained interest in Apple products and industrial design.
- Early yearly summaries already mention learning about industrial design and business through device reviews, Google I/O, WWDC, and similar material.
- After formal HCI training, product judgment shifts from aesthetic preference toward a clearer understanding that people should be placed first. Wearables, voice systems, browsing behavior, and self-service agent builders all show this change.

## References

- [changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/](https://changkun.de/blog/posts/2013-09-19-从Windows到Macintosh/)
- [changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/](https://changkun.de/blog/posts/2014-03-22-谈谈对编程语言的一般性认识/)
- [changkun.de/blog/posts/2014-11-20-WatchKit框架与WatchApp交互初窥/](https://changkun.de/blog/posts/2014-11-20-WatchKit框架与WatchApp交互初窥/)
- [changkun.de/blog/posts/2016-05-11-swiftapi/](https://changkun.de/blog/posts/2016-05-11-swiftapi/)
- [changkun.de/blog/demo/](https://changkun.de/blog/demo/)
- [changkun.de/blog/bachelorthesis/](https://changkun.de/blog/bachelorthesis/)
- [changkun.de/blog/augmentedtouch/](https://changkun.de/blog/augmentedtouch/)
- [changkun.de/blog/clients/](https://changkun.de/blog/clients/)
- Unpublished draft: `Several Practices for Building Cross-Platform Clients with Electron`
- [changkun.de/blog/posts/2016-09-04-博客客户端发布/](https://changkun.de/blog/posts/2016-09-04-博客客户端发布/)
- [changkun.de/blog/posts/2017-03-14-Electron-深度实践总结/](https://changkun.de/blog/posts/2017-03-14-Electron-深度实践总结/)

## One-Sentence Summary

The interest in languages and platforms is, at root, a way of understanding how software should be designed and used through toolchains, interaction forms, and product boundaries.
