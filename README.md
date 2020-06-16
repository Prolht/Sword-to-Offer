# 算法汇总

[toc]

#### 给定一个没有重复数字的序列，返回其所有可能的全排列。
```py
from typing import List
import itertools
def permute(nums: List[int]) -> List[List[int]]:
        return list(itertools.permutations(nums))
nums = [1,2,3]
permute(nums)
```


#### **面试题4：二维数组中的查找**
[代码](./bin/04.py)
题目：在一个二维数组中，每一行都按照从左到右递增的顺序排列，每一列都按照从上倒下递增的顺序排列。请完成一个函数，输入这样的一个二位数组和一个整数，判断数组中是否含有该整数。

#### **面试题5：替换空格**
[代码](./bin/05.py)
题目：请实现一个函数，把字符串中的每个空格替换成%20。例如，输入“we are happy”，则输出“we%20are%20happy”。

#### **面试题6：从尾到头打印链表**
[代码](./bin/06.py)
题目：输入一个链表的头结点，从尾到头反过来打印出每个节点的值。
链表节点的定义为：

```
class Node:
    '''
    定义节点类
    data:数据
    _next:下一个数据
    '''
    def __init__(self,data,_next = None):
        self.data = data
        self._next = _next
    def __repr__(self):
        '''
        用来定义Node的字节输出
        '''
        return str(self.data)
```
#### **面试题7：重建二叉树**
[代码](./bin/07.py)
题目：输入某二叉树的前序遍历和中序遍历的结果，请重建该二叉树。假设输入的前序遍历和中序遍历的结果中都不含重复的数组。例如，输入前序遍历序列[1,2,4,7,3,5,6,8]和中序遍历序列[4,7,2,1,5,3,8,6]，则重建如图所示的二叉树并输出它的头节点。二叉树节点的定义如下：
```
class Node:
    def __init__(self,data):
        self.data = data
        self.left = None
        self.right = None
```
#### **面试题9：用两个栈实现队列**
[代码](./bin/09.py)
题目：用两个栈实现一个队列。请实现队列的两个函数appendTail和deleteHead，分别完成在队列尾部插入节点和在队列头部删除节点的功能

#### **面试题10：斐波那契数列**
题目一：求斐波那契数列的第n项。
[代码](./bin/10.py)
写一个函数，输入n，求斐波那契数列的第n项。斐波那契数列的定义如下：
```
f(n)={  
        0                n=0
        1                n=1
        f(n-1)+f(n-2)    n>1
    }
```
题目二：青蛙跳台阶问题。
[代码](./bin/10-2.py)
一只青蛙一次可以跳上1级台阶，也可以跳上2级台阶。求该青蛙跳上n级台阶总共有多少种跳法。

#### **面试题11：旋转数组的最小数字**
[代码](./bin/11.py)
题目：把一个数组做开始的若干个元素搬到数组的末尾，我们称之为数组的旋转。输入一个递增排序的数组的一个旋转，输出旋转数组的最小元素。例如，数组[3，4，5，1，2]为[1,2,3,4,5]的一个旋转，该数组的最小值为1.

#### **面试题12：矩阵中的路径问题**
[代码](./bin/12.py)

#### **面试题14：剪绳子**
[代码](./bin/14.py)
题目：给你一根长度为n的绳子，请把绳子剪成m段（m，n都是证书，n>1并且m>1），每段绳子的长度记为k[0],k[1]，···，k[m]。请问k[0]*k[1]*···*k[m]可能的最大乘积是多少？例如，当绳子的长度是8时，我们把它剪成长度分别为2，3，3的三段，此时得到的最大乘积是18。
#### **面试题15：二进制中1的个数**
[代码](./bin/15.py)
题目：请实现一个函数，输入一个整数，输出该数二进制表示中1的个数。例如，把9表示成二进制是1001，有2位是1.因此，如果输入9，则该函数输出2。
#### **面试题16：数值的整数次方**
[代码](./bin/16.py)
题目：实现函数Power(base,exponent)，求base的exponent次方。不得使用库函数，同时不需要考虑大数问题。
#### **面试题17：打印从1到最大的n位数**
[代码](./bin/17.py)
题目：输入数字n，按顺序打印出从1到最大的n位十进制数。比如输入3，则打印1，2，3一直到最大的3位数999.
#### **面试题18：删除链表的节点**
[代码](./bin/18.py)
**题目一** ：在O(1)时间内删除链表节点
给定单项链表的头指针和一个节点指针，定义一个函数在O(1)时间内删除该节点。链表节点与函数的定义如下：
```
class Node:
    '''
    定义节点类
    data:数据
    _next:下一个数据
    '''
    def __init__(self,data,_next = None):
        self.data = data
        self._next = _next
    def __repr__(self):
        '''
        用来定义Node的字节输出
        '''
        return str(self.data)
```
**题目二**：删除链表中重复的节点。
在一个排序的链表中，如何删除重复的节点？
#### **面试题19：正则表达式匹配**
[代码](./bin/19.py)
#### **面试题20：表示数值的字符串**
[代码](./bin/20.py)
#### **面试题21：调整数组顺序使奇数位于偶数后面**
[代码](./bin/21.py)
#### **面试题22：链表中倒数第k个节点**
[代码](./bin/22.py)
#### **面试题23：链表中环的入口节点**
[代码](./bin/23.py)
#### **面试题24：反转链表**
[代码](./bin/24.py)
思路：当前节点Node，上一个节点为prevNode，下一个节点为nextNode。先取一个节点Node，令Node.next=prevNode，再令prevNode=Node,Node=nextNode,最后将其放入while循环中。
#### **面试题25：合并两个排序的链表**
[代码](./bin/25.py)
思路：创建一个新的head，对原始的两个head1，head2进行比较，head=比较小的那个，然后调用递归函数，对下一个节点重新判断。
#### **面试题26：树的子结构**
[代码](./bin/26.py)
思路：先在大树上找与小树相同的根节点，若找不到，则返回False，若找得到，调用函数判断剩下的节点与小树的节点是否相等，相等则返回True。  
#### **面试题27：二叉树的镜像**
[代码](./bin/27.py)
思路：先前序遍历这棵树的每个结点，如果遍历到的结点有子结点，就交换它的子结点。当交换完所有非叶子结点的左右子结点之后，就得到了树的镜像
#### **面试题28：对称的二叉树**
[代码](./bin/28.py)
思路：可以与自身的副本进行比较，左右都相等则为对称。
#### **面试题29：顺时针打印矩阵**
[代码](./bin/29.py)
#### **面试题30：包含min函数的栈**
[代码](./bin/30.py)
#### **面试题31：栈的压入、弹出序列**
[代码](./bin/31.py)
题目：输入两个整数序列，第一个序列表示栈的压入顺序，请判断第二个序列是否为栈的弹出顺序。
思路：创建辅助栈，使第一个栈弹出并压入辅助栈，若辅助栈与l2相等，则为True
#### **面试题32：从上到下打印二叉树**
[代码](./bin/32.py)
#### **面试题33：二叉搜索树的后序遍历序列**
[代码](./bin/33.py)
二叉搜索树的特点为左子结点小于根节点，右子结点大于根结点
#### **面试题34：二叉树中和为某一值的路径**
[代码](./bin/34.py)
#### **面试题35：复杂链表的复制**
[代码](./bin/35.py)
#### **面试题36：二叉搜索树与双向链表**
[代码](./bin/36.py)
#### **面试题37：序列化二叉树**
[代码](./bin/37.py)
#### **面试题38：字符串的排列**
[代码](./bin/38.py)
#### **面试题39：数组中出现次数超过一半的数字**
[代码](./bin/39.py)
#### **面试题40：最小的k个数**
[代码](./bin/40.py)
#### **面试题41：数据流中的中位数**
[代码](./bin/41.py)
#### **面试题42：连续子数组的最大和**
[代码](./bin/42.py)
#### **面试题43：1~n整数中1出现的次数**
[代码](./bin/43.py)
#### **面试题44：数字序列中某一位的数字**
[代码](./bin/44.py)
#### **面试题45：把数组排成最小的数**
[代码](./bin/45.py)
#### **面试题46：把数组翻译成字符串**
[代码](./bin/46.py)
#### **面试题47：礼物的最大价值**
[代码](./bin/47.py)
思路：先将第一行第一列的利用一个辅助矩阵buff表示出来（buff表示从左上角走到位置为(i,j)处最大路径的和），然后开始对行和列进行递增循环，当到达（i，j）位置时，此时buff的值为该位置左边或者上边之中最大的值加上原来矩阵的值。
#### **面试题48：最长不含重复字符串的子字符串**
[代码](./bin/48.py)
#### **面试题49：丑数**
[代码](./bin/49.py)
#### **面试题50：第一个只出现一次的字符**
[代码](./bin/50.py)
#### **面试题51：数组中的逆序对**
[代码](./bin/51.py)
#### **面试题52：两个链表的第一个公共节点**
[代码](./bin/52.py)
#### **面试题53：在排序数组中查找数字**
[代码](./bin/53.py)
#### **面试题54：二叉搜索树的第k大节点**
[代码](./bin/54.py)
#### **面试题55：二叉树的深度**
[代码](./bin/55.py)
#### **面试题56：数组中数字出现的次数**
[代码](./bin/56.py)
#### **面试题57：和为s的数字**
[代码](./bin/57.py)
#### **面试题58：反转字符串**
[代码](./bin/58.py)
#### **面试题59：队列的最大值**
[代码](./bin/59.py)
#### **面试题60：n个骰子的点数**
[代码](./bin/60.py)
#### **面试题61：扑克牌中的顺子**
[代码](./bin/61.py)
#### **面试题62：圆圈中最后剩下的数字**
[代码](./bin/62.py)
#### **面试题63：股票的最大利润**
[代码](./bin/63.py)
#### **面试题64：求1+2+3+···+n**
[代码](./bin/64.py)
#### **面试题65：不用加减乘除做加法**
[代码](./bin/65.py)
#### **面试题66：构建乘积数组**
[代码](./bin/66.py)
#### **冒泡排序：**
[代码](./bin/bubbleSort.py)
1、从第一个数据开始，与第二个数据相比较，如果第二个数据小于第一个数据，则交换两个数据的位置。
2、指针由第一个数据移向第二个数据，第二个数据与第三个数据相比较，如果第三个数据小于第二个数据，则交换两个数据的位置
3、依此类推，完成第一轮排序。第一轮排序结束后，最大的元素被移到了最右面。
4、依照上面的过程进行第二轮排序，将第二大的排在倒数第二的位置。
5、重复上述过程，没排完一轮，比较次数就减少一次。
#### **插入排序**
[代码](./bin/insert_sort.py)
插入排序是简单排序中最快的排序算法，虽然时间复杂度仍然为O(n*n)，但是却比冒泡排序和选择排序快很多。
原理：
1、将指针指向某个元素，假设该元素左侧的元素全部有序，将该元素抽取出来，然后按照从右往左的顺序分别与其左边的元素比较遇到比其大的元素便将元素右移，直到找到比该元素小的元素或者找到最左面发现其左侧的元素都比它大，停止；
2、此时会出现一个空位，将该元素放入到空位中，此时该元素左侧的元素都比它小，右侧的元素都比它大；
3、指针向后移动一位，重复上述过程。每操作一轮，左侧有序元素都增加一个，右侧无序元素都减少一个。
#### **桶排序**
[代码](./bin/bucketSort.py)
找到列表中最大的元素
创建全部位0的列表作为桶，桶的大小位最大元素的大小
把列表中的元素放入桶中，即对应元素+1
然后再将其从桶中取出
时间复杂度：O(N+C)，其中C=N*(logN-logM) 
#### **快速排序**
[代码](./bin/quicksort.py)
快速排序使用分治法策略来把一个序列分为两个子序列。
步骤：
从数列中挑出一个元素，称为"基准"（pivot），
重新排序数列，所有元素比基准值小的摆放在基准前面，所有元
素比基准值大的摆在基准的后面（相同的数可以到任一边）。在这个
分割结束之后，该基准就处于数列的中间位置。这个称为分割
（partition）操作。
递归地（recursive）把小于基准值元素的子数列和大于基准值
元素的子数列排序。
