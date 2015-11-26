---
title: '译见｜谋定而后动，将应用 Docker 化之前的 4 道必答题'
---

<!-- reviewed by fiona -->

![](http://7xi8kv.com5.z0.glb.qiniucdn.com/yijian-8-1.jpg)

> 译见系列｜DaoCloud 现推出「译见」系列，每周为开发者提供国外精品译文，主要关注云计算领域的技术和前沿趋势。本系列由 Fiona 翻译。


#### 译者注
欧洲 DockerCon 大会将于今天在巴塞罗那开幕，届时又会有诸多重磅新闻。毫无疑问，在过去的两年里，Docker 容器技术的风靡，证明了它的价值。然而喧嚣背后，如何在企业中使用 Docker，这是横亘在首席执行官们面前最重要的议题。

#### 作者介绍

Jason Mckay，Logicworks 公司高级副总裁兼首席技术官。Logicworks 是一家云计算战略与管理咨询公司。创立于 1983 年，总部位于纽约，提供世界级的复杂 IT 解决方案，他们的客户包括美国最大的卫生保健、法律和公共部门。

---

Docker 因使用简单而闻名。然而对于采用一体化应用同时对 Docker 感兴趣的企业来说，缺乏实际使用 Docker 的相关信息。甚至在敏捷爱好者当中，对于微服务模型是否值得一试也存在巨大争议。

如果你希望提升已有的一体化应用的灵活性，如何来决定 Docker 是最佳答案？容器部署的收益是否能够抵扣切割或重写应用的工作？以下列出了 4 个问题，你需要在容器化应用之前好好想想。

### 1. 你希望采用 Docker 或微服务吗？

Docker 是高效部署微服务的解决方案，但是它并不能自动创建微服务进程或者团队。在你开始使用 Docker 之前，你得决定自己是否能够全盘接受微服务的优点和风险。然后你得在构建或重构微服务应用的道路上不断尝试，Docker 只是其中的一小部分。

也就是说，一体化应用的某些组件是能够容器化的。独立或单一功能的组件，特别是不需要保持本地状态的组件，尤其适合进行 Docker 的早期尝试。这些服务成熟快，能够横向扩展，也能在简单的部署包中打包复杂的功能。

 

### 2. 你是否准备好管理多个语言/库/镜像仓库？

去年，我们遇到的一个机构部署了模块化应用，同时允许自己的开发人员随个人喜好来构建单一组件。想法虽好，最后却变成了噩梦——单纯追逐模块化设计的理想，却毫不考虑这一复杂性给运营带来的影响。

尽管该组织后来对使用 Docker 减轻部署压力大有兴趣，我们还是强烈建议他们在解决根本问题之前不要使用 Docker。对于长期维护应用所需的部署栈所带来的困难，简化不同应用的部署并非一剂解药。

 

### 3. 你是否已经有了日志、监控或者成熟的部署方案？

如果你们的应用早已采用了传输日志、在正确时间将数据备份到正确位置的框架，那大有机会。要使用 Docker，你不仅要重复虚拟机环境里的日志行为，还要让你的合规团队为这些变化做好准备。Docker 社区一向都有新工具加入，然而在稳定性和成熟度方面，它们比不上现有方案。部分更新、回滚和其它常见的部署任务可能需要重新设计，从而符合容器化部署。

不破不立。如果你已经在构建持续集成/持续交付的流水线上投入了大量的时间，那容器化那些遗留应用可能是得不偿失。

 

### 4. 云端自动化将会压倒容器化？

在11月举行的 AWS Re：Invent 大会上，亚马逊首席技术官 Werner Vogels 在自己的主题演讲中，用大量篇幅介绍了 AWS Lambda，一款基于代码部署基础设施的自动化工具。Vogels 也提及了 AWS 的容器服务，不过他强调对于开发者来说，Lambda 对零基础设施的处理，更适合配置和部署容器。

容器技术在业界迅速风靡，必将成为许多专业持续集成/持续交付流水线的重要组成部分。然而身为技术专家和首席技术官，你的职责是迎接新技术和新服务的挑战，妥善权衡早期采用的风险。我相信 Docker 对于理解容器化后果的组织来说非常有效，前提是你能正确回答我提出的这些问题。

 