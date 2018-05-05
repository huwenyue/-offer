# -offer
## 二进制中1的个数
相关题目：1）用一条语句判断一个整数是不是2的整数次方：  

一个整数若是2的整数次方，则它的二进制表示中有且仅有一位是1，则把这个整数减去1之后再和它自己做与运算，结果为0.  

2）输入两个整数m和n，计算需要改表m的二进制表示中的多少位才能得到n： 

如10的二进制表示为1010，13的二进制表示为1101，需要改变1010中的3位才能得到1101.我们可以分为两步来解决这个问题：第一步求两个数的异或（相同为0，不同为1），第二步统计异或结果中1的位数。  

## 插入排序  

1）将开头元素视为已排序  

2）从第二个元素(i)开始，从已排序部分的末尾(i-1)开始，将所有比它大的元素向后移动一个单位  

3）将第二个元素插入空位  

4）循环  

稳定排序：只将比v大的元素向后平移，不相邻的元素不会直接交换位置  

算法复杂度为O(N^2),考虑最坏情况：每个i循环都需要执行i次移动，总共需要1+2+...+N-1=(N^2-N)/2次移动  

若输入数据为生序，则数据不需要移动，只需要经历N次比较。故插入排序的优势为处理相对有序的数据。

## 冒泡排序
1）从数组末尾开始依次比较相邻两个元素，若大小相反则交换位置。  

是稳定排序：因为值相同的元素不会改变顺序，但是将比较运算A[j]<A[j-1]改为A[j]<=A[j-1]，算法将失去稳定性。  

复杂度：需要对相邻元素进行(N-1)+(N-2)+...+1=(N^2-N)/2次比较，故O(n^2).
