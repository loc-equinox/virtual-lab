这里整理了一些可以在短期内动手完成的模块化任务。

## 自动算子合成
### 基于 AKO4ALL 的 SOL-ExecBench 跑分
通过这个小任务，你可以体验到 Agentic Kernel Optimization 的流程。

[AKO4ALL](https://github.com/TongmingLAIC/AKO4ALL#) 非常简单，提供了一个最小的环境，你需要在这个 repo 里提供你想要优化的 kernel，目标 benchmark（这里用 [Sol-ExecBench](https://github.com/NVIDIA/SOL-ExecBench)）和其他你认为有必要的工具，并选用一个 coding agent 在这个 repo 上进行优化，最后提交到 [Sol-ExecBench 官网](https://research.nvidia.com/benchmarks/sol-execbench) 进行评测。

Tips:

+ 你可以去智星云租一台有 GPU 的 Linux 机器。
+ 关于 Coding Agent，我们建议使用 Claude Code，搭配 Opus-4.6，这样效果比较好。国内有一些购买 Claude Code API 的站点。