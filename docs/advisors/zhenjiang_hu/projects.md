这里整理了一些可以在短期内动手完成的模块化任务。

## 领域特定语言
### 基于 Rocq 的 Imp DSL

+ 项目背景： 希望在一个足够强大的 host language 上构建一个 DSL, 使得 DSL 内部既可以描述计算, 也可以书写程序规范和性质证明。
+ 参考路线：
    1. 定义一个简单的 imperative language (下称 Imp)。
    2. 为 Imp 设计相应的规范命题和证明语言 (可高度简化)。
    3. 在 Rocq 中将 Imp 构建为一个内嵌的 DSL。
    4. 在 Rocq 中实现 Imp 的规范和证明的书写功能。

### Hygienic Macro 实现

+ 项目目标: 实现一个简单的卫生宏系统
+ 项目内容:
    1. Kohlbecker’s Algorithm（时间戳重命名）
    2. Syntax Closures（显式指定标识符解析环境）
    3. 基本宏系统（模式匹配和替换）