# -offer
## 二进制中1的个数
相关题目：1）用一条语句判断一个整数是不是2的整数次方：  

一个整数若是2的整数次方，则它的二进制表示中有且仅有一位是1，则把这个整数减去1之后再和它自己做与运算，结果为0.  

2）输入两个整数m和n，计算需要改表m的二进制表示中的多少位才能得到n： 

如10的二进制表示为1010，13的二进制表示为1101，需要改变1010中的3位才能得到1101.我们可以分为两步来解决这个问题：第一步求两个数的异或（相同为0，不同为1），第二步统计异或结果中1的位数。
