## 自动算子合成
### 基础知识
+ 基本概念：CUDA（nvcc, cuBLAS, cuDNN），ROCm，PyTorch，Triton，TVM，TileLang 等等，建议和大模型对话几轮，熟悉一下上述概念。
+ CUDA 推荐教材：Programming Massively Parallel Processors
+ Triton 推荐教程：[https://triton-lang.org/main/getting-started/tutorials/index.html](https://triton-lang.org/main/getting-started/tutorials/index.html)，不需要 PyTorch 先修，因为这个教程也是对比 PyTorch 和 Triton 的性能差距，所以也能借此学会 PyTorch 的语法。

### 相关论文
+ 经典论文：[KernelBench: Can LLMs Write Efficient GPU Kernels?](https://arxiv.org/abs/2502.10517) (ICML '25)
+ 组内最新工作：[KernelBand: Steering LLM-based Kernel Optimization via Hardware-Aware Multi-Armed Bandits](https://arxiv.org/abs/2511.18868)
+ Nvidia 近期工作，部分 workload 上性能超越专家手写库：[AVO: Agentic Variation Operators for Autonomous Evolutionary Search](https://arxiv.org/abs/2603.24517)
+ Nvidia 最新 benchmark：[SOL-ExecBench: Speed-of-Light Benchmarking for Real-World GPU Kernels Against Hardware Limits](https://arxiv.org/abs/2603.19173)
