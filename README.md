
# algorithm
数据结构与算法学习笔记


### 03 | 复杂度分析（上）：如何分析、统计算法的执行小路和资源消耗？

#### 一、什么是复杂度分析？

复杂度分析（时间、空间复杂度分析）是用于衡量编写的算法代码的执行效率的。数据结构和算法本身解决的是“快”和“省”的问题，即如何让代码运行得更快，更省存储空间，而执行效率正是算法一个非常重要的考量指标。<br>

#### 二、为什么需要复杂度分析？

（1）测试结果非常依赖测试环境

（2）测试结果受数据规模的影响很大

#### 三、怎么分析复杂度？

**大O复杂度表示法**
1. **时间复杂度分析**

时间复杂度的全称是渐进时间复杂度，表示算法的执行时间与数据规模之间的增长关系。

> (1) 只关注循环执行次数最多的一段代码
> 
> (2) 加法法则：总复杂度等于量级最大的那段代码的复杂度 
> T(n) = T1(n) + T2(n) = max(O(f(n)), O(g(n))) = O(max(f(n), g(n)))
>
> (3) 乘法法则：嵌套代码的复杂度等于嵌套内外代码复杂度的乘积
> T(n) = T1(n) * T2(n) = O(f(n)) * O(g(n)) = O(f(n) * g(n))
> 
>   **常见时间复杂度量级：**
>   * O(1)
>   * O(logn) 、O(nlogn)
>   * O(m+n)、O(m*n)
  
2. **空间复杂度分析**

空间复杂度的全称是渐进空间复杂度，表示算法的存储空间与数据规模之间的增长关系。

>   **常见的空间复杂度量级：**
>   O(1)、O(n)、O(n2)等