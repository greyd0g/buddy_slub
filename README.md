buddy and slub
================
从Linux Kernel中提取出来的buddy/slub算法实现。buddy/slub是Linux内核中的内存管理算法。
buddy防止内存的“外碎片”，即防止内存块越分越小，而不能满足大块内存分配的需求。
slub防止内存的“内碎片”，即尽量按请求的大小分配内存块，防止内存块使用上的浪费。

实现代码针对x86_64平台

执行方式：
echo 3 > /proc/sys/vm/nr_hugepages
cat /proc/meminfo | grep Huge
./root

