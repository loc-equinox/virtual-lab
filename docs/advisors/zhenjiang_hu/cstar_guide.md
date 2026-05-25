由于 CStar 目前的文档不太成熟，所以这个模块主要承担如下功能：
+ 记录 CStar 使用的各个环节中一些需要注意的问题，以便后续使用科研实习室的同学们进行 troubleshooting。
+ 对一些证明案例进行讲解和分析

TODO：这个模块目前的组织形式还不是很清晰，需要后续同学进行一些整理

+ 当报错 `cannot obtain verification condition` 而没有给具体报错行列号的时候，建议通过把代码片段注释掉的方式来查找出问题的地方。

+ 写 `[[cst::require]]` 和 `[[cst::ensure]]` 时注意常数要标注类型，比如应该是 `0i` 而不是 `0`。
+ 对于如下 `.h` 文件中的代码：
    + ``` c
        void assign_p2(int *loc)
        [[cst::require(`data_at loc Tint 0i`)]]
        [[cst::ensure(`emp`)]]
        ;
      ```
    + 注意 `[[cst::require]]` 不能包含全局变量，也就是说不能这样：
    + ``` c
        int *loc;

        void assign_p2()
        [[cst::require(`data_at loc Tint 0i`)]]
        [[cst::ensure(`emp`)]]
        ;
      ```
    + 同时注意这么写相当于是默认这个函数符合这个规约（有点像公理），这时候不需要写函数体，而是直接在 `[[cst::ensure]]` 后接一个分号。
