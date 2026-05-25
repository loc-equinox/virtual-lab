## 程序验证

回顾“实验室研究方向”一节中的介绍，我们需要对待证明的语言、待证明的程序、待证明的性质、以及证明的过程进行形式化的建模，因此我们可以大致按照这个框架开展学习。你也可以把这一节的内容发给 AI，让它扩充一下你感兴趣或不太理解的地方，形成更适合你的学习路线。

### 学习路线
+ 首先我们要学习如何使用证明助理（Proof assistant）。证明助理有很多，也分为不同的技术路线，我们建议从 Rocq（Coq）开始。[https://softwarefoundations.cis.upenn.edu/](Software Foundations) 系列是这方面的经典教材。不过注意，这套教材并不需要按顺序学。一条合理的快速上手路线是 Vol1 -> Vol2(Equiv-StlcProp) -> Vol6(Basic-Wand 的 First Pass 部分)。
+ 接下来，根据你感兴趣的内容，我们可以采取不同的学习路线：

#### 路线1: 应用端-真实系统验证
+ 真实系统往往涉及并发，而 Software Foundations 里面都是单线程的程序，所以我们需要扩展我们的理论工具。并发程序有不同的建模方式，以 [https://iris-project.org/](Iris) 为代表的**并发分离逻辑**是其中一种，建议阅读网站上的 Iris lecture notes，辅以 Iris tutorial in Rocq 获得一些上手的体验。如果你还意犹未尽，想进行更深入的理论学习，可以继续阅读 Iris from the ground up 论文。
+ Software Foundations 在 Rocq 里面定义了待证明的程序，但真实系统的验证需要处理像 C 这样的实际语言。SF Vol5 的 VST 是很经典的技术，不过你也可以直接学习 [https://gitee.com/cstarlang](CStar) 或者上海交通大学团队研发的 QCP（目前 AI 可能不知道 CStar 或 QCP，所以你可能要和组里同学多交流）。
