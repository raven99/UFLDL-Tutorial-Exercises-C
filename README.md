UFLDL-Tutorial-Exersices
========================
GitHub上已经有小伙伴给出了关于Andrew Ng深度学习教程(UFLDL tutorial) 练习比较完整的实现( https://github.com/dkyang/UFLDL-Tutorial-Exercise )。这个repo将部分练习用C++实现，包括sparse autodecoder和stacked autodecoder，后续有需要还会继续改写。

矩阵运算使用了eigen3，L-BFGS优化使用了libLBFGS( https://github.com/chokkan/liblbfgs )， 显示feature map 时调用了opencv，程序调用的数据都源自于.mat文件。Project Properties 里提供了64位系统上的工程属性配置文件，仅供参考。log.txt和Weight Map.jpg是运行结果。

stacked autodecoder的实际运行速度对比matlab实现慢了两倍多（两者代码中矩阵运算并行度是一样的）==|||，具体是libLBFGS还是eigen3的原因暂未测试。
