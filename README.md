# Cloud Computing 101 创作背景

随着云计算技术与服务逐渐变成我们生活中的“水”和“电”，并且开源催生了非常多的基础设施软件，让任何人都可以快速在自己的本地环境尝试，这让云计算技术的普及变得更加“平民化”，为不计其数企业与个人带来了便利。

然而，云计算领域的技术概念与软件生态非常庞杂，云计算产品与服务也层出不穷，对于非技术与科班出身的人士理解起来并非易事。即使是全球最为流行的容器技术 Kubernetes 与 Docker，在大多数专业技术从业人士来看，[复杂度也依然是最大的挑战](https://www.cncf.io/wp-content/uploads/2020/11/CNCF_Survey_Report_2020.pdf)。

最近我身边也有越来越多的新同事初入云计算行业，面对专业和复杂的云计算与云原生相关产品与技术，在自学过程中也会有些许地感到无从入手，网上找到的文档与视频学习资料大多是面向工程师人群，而对于从事云计算行业的运营、市场、文档、销售、渠道等角色，或是萌新实习生来说，这些资料很难系统地帮助到非技术人士入门和了解云计算产品与技术，大部分官方文档对于非技术背景出身的人群通常较为晦涩难懂。

## 什么是 Cloud Computing 101

Cloud Computing 101 旨在面向上述背景中提到的**非技术背景的云计算从业者，以及对云计算与云原生产品与技术感兴趣的同学**。作者希望以**在线视频会议、原创图文以及动手实验**的方式，尽可能地将晦涩的产品技术以更加通俗的语言传达给受众，并搜集与汇总内外网相关的优质学习资源，给目标受众提供自学方向的引导。

此次系列教程受 [self-taught-guide-to-cloud-computing](https://github.com/madebygps/self-taught-guide-to-cloud-computing) 的启发，教程内容将围绕以下的几个目标进行协作输出：

### Goal

- 整理与总结云计算领域的知识图谱，重点聚焦到云原生领域的开源项目与技术
- 帮助目标受众了解云计算与云原生领域常见的概念、术语，了解最基本的使用场景
- Talk is cheap，本教程将通过互动实验的形式帮助初学者快速上手与实践
- 通过类似 [100 Days of Kubernetes](https://100daysofkubernetes.io/overview.html) 的形式打卡完成学习路线
- 希望通过开源与开放协作的方式输出教程内容（欢迎讲师自愿加入）

### Non-goal

- 本系列教程的目标并非将目标受众培养为专业的工程师
- 本系列教程不提供一对一的技术支持（遇到实际问题可以在此仓库的 GitHub issue 提出）

## 开始前

对于非计算机专业出身的同学来说，你可以根据个人时间与兴趣先对大学计算机基础补补课，提前了解一下大学计算机相关专业必修的四门课程涉及的内容，实际上还有《数据结构与算法》这门课程。如果你的发展方向不是专业的工程师，那么这些大学计算机基础课程非 100% 必须项，你可以把它们当做“字典”，在遇到相关概念或问题时，自行查阅相关教材与书籍📚，或在[中国大学慕课网](https://www.icourse163.org/)观看各大名校计算机专业教授的课程。

> 注：此图出自[大学计算机知识要点总结_思维导图](https://www.processon.com/view/61162a510e3e7407d39eeee5?fromnew=1)。

![大学计算机知识要点总结](/images/computer-science-fundamentals.jpg)

## 知识图谱

我们将对以下知识图谱中涉及到的云计算与云原生相关技术产品和开源项目的基本概念、应用场景、使用示例进行讲解，此知识图谱主要根据[青云公有云](qingcloud.com)和 [KubeSphere](kubesphere.io) 涉及的产品与生态软件进行归类，目前还是一份初稿，后续将会横向与纵向地延展，欢迎大家对内容提供建议与反馈。后期的使用教程也会主要使用[青云公有云](qingcloud.com)与 [Katacoda](katacoda.com) 这两个平台作为示例来演示。

![云计算与云原生](/images/cloud-computing-mind-map.jpg)

## 推荐书籍

推荐大家下载这本电子书：[《图解云计算架构：基础设施和 API》](https://yunify.anybox.qingcloud.com/s/YIlLFSXbk4Vcke0vKV32myPbAAHzTwyh)

## 排期

| 时间  | 课程内容 | 分享人 |
|  ----  | ----  | ---- |
| 2021.11.24 | 01 云计算基础 - 什么是 IaaS、PaaS 和 SaaS | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2021.12.1  | 02 云计算基础 - Docker 与 Kubernetes 容器云 | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2021.12.3  | 03 计算 - 了解虚拟化技术 | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2021.12.8  | 04 计算 - CPU、GPU、云服务器 | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2021.12.15  | 05 存储 - 概念：文件存储、对象存储、块存储、集中存储与分布式存储 | 冯相东 - 存储产品负责人 |
| 2021.12.22  | 06 存储 - 公有云实操：文件存储、对象存储、块存储 | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2022.1.5  | 07 云基础 - 什么是 API、SDK、CLI、Console | 周鹏飞 - Cloud Computing 101 发起人，KubeSphere 社区经理 |
| 2022.1.12  | 08 网络 - 软件定义网络 SDN 入门 | 赵天宇 - 网络产品经理 |
| 2022.1.19  | 09 数据库 - 数据库的基本概念、发展史和分类（上） | 管长龙 - KCN 数据库社区经理 |
| 2022.1.26  | 10 数据库 - 数据库的基本概念、发展史和分类（下） | 管长龙 - KCN 数据库社区经理 |
| 2022.7.6   | 特别篇 英语技术文档写作 | 刘玲玲 - KCN 海外运营&文档工程师 |
| 2022.8.3  | 11 消息队列与中间件 - 浅入浅出消息中间件 | 汪媛媛 - KCN 数据库产品经理 |
| 2022.8.24  | 特别篇 软件测试了解一下 | 丁源 -  PXD 高级测试工程师 |


待分享议题：
- 12 大数据
- 13 云安全  

## 课件

- 01 02 03 04 06 07 的 [PPT](https://docs.google.com/presentation/d/1dIKQQPvRuTxwcgfLKtU1rtnckkddrJhPZj4Hf7PNkBE/edit?usp=sharing)
- 05 08 09 10 文档篇 11 测试篇 的 [PPT](./slides/)

视频可在 **北森 OA** 的学习中心检索 *Cloud Computing 101* 查看回放。

## 贡献者讲师（欢迎加入）

- [Feynman Zhou](https://github.com/FeynmanZhou/)
- 相东
- 朱波
- 赵天宇
- [管长龙](https://github.com/KID-G)
- [刘玲玲](https://github.com/hayleyling)
- 汪媛媛
- [丁源](https://github.com/dingyuan408)
