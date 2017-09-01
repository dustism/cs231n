finish KNN training

date: 2017/8/28

还完全不熟悉python的语法，花了很长的时间配了github，折腾了半天终于能够写上代码了，感叹一下jupyter还是挺好用的

KNN是cs231n assignment1的第一个task，难度上来说比较小吧，主要的workload都被我浪费在查python的语法上面了。

主要的任务就是完成KNN的三种求dist的方式（2重循环，1重循环，不用循环），不用循环的那个参考了hint里面说的用矩阵乘法，很快就想出来了。然后是进行交叉验证的部分，参考了http://www.bijishequ.com/detail/435374?p= 的解答，之前一直都没有搞清楚题目到底想让我干啥。python真是个神奇的语言


date: 2017/9/1

这几天疯狂摸鱼，结果就写掉SVM和softmax。这两个东西本质上都是通过矩阵乘法搞得线性的classifier，要用到很多的矩阵操作，非常的玄学，再次感叹python的vertor的优化真是好，明明遍历矩阵也需要一次循环，但是就是能很好地优化复杂度。softmax和svm核心概念一个是loss，一个是grad。loss就是用来评判（惩罚）一个W是不是好的一个函数，然后在对loss求导得到grad，学着CV真的发现自己的线性代数没有学好，算梯度下降的时候如同弱智。梯度下降的方法参考http://blog.csdn.net/yc461515457/article/details/51924604还有https://zhuanlan.zhihu.com/p/21478575 可以说是非常清晰具体了
