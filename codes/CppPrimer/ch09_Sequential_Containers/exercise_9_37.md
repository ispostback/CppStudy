> 练习9.37：为什么list或array没有capacity成员函数？

---

为什么vector需要？vector需要兼顾性能，如果每添加一个元素，就执行一次内存分配和释放操作，性能会很慢。为了避免这种代价，vector会预留一些空间备用，可以用来保存更多的元素，capacity就是用来返回当前可用空间的函数。

但是list的空间不是连续存储的，不需要有预留空间。

array的空间不能改变，因此也没有必要有预留空间。
