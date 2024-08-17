# cpp_interview_related

## todo list
- [ ] [深信服最经典20道C++面试题，腾讯、百度也适用](https://mp.weixin.qq.com/s/p_EP1JTSkx2xwuDF5CfN0w)
- [ ] 动手自己实现红黑树：[红黑树的c++实现](https://github.com/Neo-ZK/RB_Tree)，[红黑树的详细实现](https://blog.csdn.net/code_peak/article/details/120643910)

## note

### hashmap和map的区别，底层数据结构算法是什么
在C++中，HashMap和Map的概念没有直接对应的标准库接口，但是可以通过使用 unordered_map 和 map 来实现类似的功能。

区别如下：
- unordered_map是哈希表的实现，map是红黑树（Red-Black Tree）的实现。
- unordered_map不保证元素的顺序，而map按照键的自然顺序进行排序。
- unordered_map允许键和值为null（C++11开始支持），而map不允许键为空。

底层数据结构算法：
- unordered_map使用散列函数将键映射到存储桶中，并使用链式地址法解决哈希冲突。
- map使用红黑树作为底层数据结构，保证元素有序，并提供了 O(log N)时间复杂度的插入、删除和查找操作。