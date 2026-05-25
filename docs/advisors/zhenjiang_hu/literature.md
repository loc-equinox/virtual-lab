## 程序验证

回顾“实验室研究方向”一节中的介绍，我们需要对待证明的语言、待证明的程序、待证明的性质、以及证明的过程进行形式化的建模，因此我们可以大致按照这个框架开展学习。你也可以把这一节的内容发给 AI，让它扩充一下你感兴趣或不太理解的地方，形成更适合你的学习路线。

### 学习路线
+ 首先我们要学习如何使用证明助理（Proof assistant）。证明助理有很多，也分为不同的技术路线，我们建议从 Rocq（Coq）开始。[Software Foundations](https://softwarefoundations.cis.upenn.edu/) 系列是这方面的经典教材。不过注意，这套教材并不需要按顺序学。一条合理的快速上手路线是 Vol1 -> Vol2(Equiv-StlcProp) -> Vol6(Basic-Wand 的 First Pass 部分)。
+ 接下来，你可以根据自己感兴趣的内容采取不同的学习路线：

#### 路线1: 应用端-真实系统验证
+ 真实系统往往涉及并发，而 Software Foundations 里面都是单线程的程序，所以我们需要扩展我们的理论工具。并发程序有不同的建模方式，以 [Iris](https://iris-project.org/) 为代表的**并发分离逻辑**是其中一种，建议阅读网站上的 Iris lecture notes，辅以 Iris tutorial in Rocq 获得一些上手的体验。如果你还意犹未尽，想进行更深入的理论学习，可以继续阅读 Iris from the ground up 论文。
+ Software Foundations 在 Rocq 里面定义了待证明的程序，但真实系统的验证需要处理像 C 这样的实际语言。SF Vol5 的 VST 是很经典的技术，不过你也可以直接学习 [CStar](https://gitee.com/cstarlang) 或者上海交通大学团队研发的 QCP（目前 AI 可能不知道 CStar 或 QCP，所以你可能要和组里同学多交流）。

## 双向变换

代表论文：

+ BiOOP（OOPSLA 2023）：首个双向面向对象语言，支持对对象的程序化和直接操作

+ Biparsers （POPL 2025）：支持 exact-printing 的双向解析器框架

+ Effectful Lenses （ICFP 2025）：允许在 get 和 put 中使用不同单子的 effectful lenses

## 领域特定语言

### 基础知识
+ 理论方面：形式逻辑、类型理论、范畴论、计算理论
+ 实践方面：
    + 对不同分支的函数式语言都能有一定了解
    + Haskell, Scheme, Rocq 都是很好的学习对象

### 代表论文

+ Think like a vertex, behave like a function! a functional DSL for vertex-centric big graph processing (ICFP 2016)
    + 核心问题：语法糖翻译到 host language 会导致抽象泄露，错误信息可能引用用户从未写过的术语
    + 解决方案: 使用语义提升框架，从 host language 语义和 desugaring 规则静态推导出自包含的求值规则

+ A Lazy Desugaring System for Evaluating Programs with Sugars (FLOPS 2022)

+ Semantics Lifting for Syntactic Sugar (OOPSLA 2024)

## 程序综合与优化

### 代表论文

+ Superfusion (PLDI 2024)
    + 研究背景：中间数据结构是函数式编程效率低下的常见原因
    + 核心问题：组合式函数的效率问题、传统融合技术的局限（基于预定义重写规则）、可扩展性挑战
    + 技术方案：
        1. superfusion 方法: 基于归纳程序综合消除中间数据结构
        2. Ghost compression function: 分解联合 sketch 填充问题为独立子问题
        3. SuFu 工具: 解决 264/290 任务

+ Decomposition-based Synthesis（TOPLAS 2024）
    + 研究背景：分治 (D&C) 等算法范式难以应用到实际任务
    + 核心问题：语法重写限制使应用困难、子程序间依赖关系难以分解
    + 技术方案
        1. AutoLifter 系统: 不依赖语法重写的综合器
        2. 两种分解方法: component elimination & variable elimination
        3. Lifting problems: 捕获 D&C 类范式应用的形式化问题
