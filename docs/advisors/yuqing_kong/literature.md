## 知识库与实验场

### 核心知识库
在孔老师的组里并不需要非常硬核的前置知识，但是如果你想快速上手，也可以先把下面这些经典内容过一遍：

1. 同行评审中的机制设计（Peer Prediction）。其实核心逻辑万变不离其宗：我们要设计一套“激励相容”的博弈机制。因为没有“标准答案（No ground truth）”，系统只能根据大家提交的答案互相印证。通过巧妙地利用信息论和概率论（比如 Mutual Information 互信息、Logarithmic Market Scoring Rules 等），让说真话、给出高质量信息的人能够获得最高的回报期望。

2. 未完待续

### 新手练级小任务
不要上来就被一堆公式吓跑！你可以挑下面这两个方向的一个练练手：

1. **推导路线（偏向理论）**：从实验室早期的论文或者经典文献里挑 2 个定理，重新梳理并推演一遍核心算法的证明。

2. **复现路线（偏向动手）**：找一篇组里最近做的论文，跑通他们的实验。


### 代码与算力游乐场
由于实验室主要是做理论，所以大部分时间不需要大量的"代码"和"算力"。
不过，现在组里也在做大模型相关的应用实验。


## 相关论文
以下是根据孔老师推荐的经典轮转任务整理的论文清单：

+ [Dominantly Truthful Multi-task Peer Prediction with a Constant Number of Tasks](https://arxiv.org/abs/1911.00272) (SODA 2020) - 孔老师关于机制设计的核心理论突破。
+ [An Information-Theoretic Framework For Designing Information Elicitation Mechanisms That Reward Truth-telling](https://dl.acm.org/citation.cfm?doid=3309879.3296670) (TEAC 2019)
+ [Water from Two Rocks: Maximizing the Mutual Information](https://arxiv.org/abs/1802.08887) (EC 2018)
+ [LDMI: A Novel Information-theoretic Loss Function for Training Deep Nets Robust to Label Noise](https://arxiv.org/abs/1909.03388) (NeurIPS 2019) - 用信息论做 Loss 去解决 Label 噪声问题。
+ [Max-MIG: an Information-Theoretic Approach for Joint Learning from Crowds](https://openreview.net/forum?id=BJg9DoR9t7) (ICLR 2019)
+ [BONUS! Maximizing Surprise](https://arxiv.org/abs/2107.08207) (WWW 2022) - 孔老师组把经济学 Surprise 理论引入计算机博弈机制的有趣工作。
+ [False Consensus, Information Theory, and Prediction Markets](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.ITCS.2023.81) (ITCS 2023)