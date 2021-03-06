# [机器学习笔记] Note1--机器学习简介

> 阅读本文大约需要 2 分钟

**本文结构：**

[TOC]

这是学习 Andrew Ng 在 Coursea 上的[机器学习课程](https://www.coursera.org/learn/machine-learning)所做的笔记。

### 什么是机器学习

 对于机器学习，并没有一个一致认同的定义，一个比较古老的定义是由`Arthur Samuel`在 1959 年给出的：

> 机器学习研究的是如何赋予计算机在没有被明确编程的情况下仍能够学习的能力。(Field of study that fives computers the ability to learn without being explicily programmed.)

随后他编写了一个跳棋游戏的程序，并且让这个程序和其自身玩了几万局跳棋游戏，并且记录下来棋盘上的什么位置可能会导致怎样的结果，随着时间的推移，计算机学会了棋盘上的哪些位置可能会导致胜利，并且最终战胜了设计程序的 Samuel。

另一个比较现代且形式化的定义是由`Tom Mitchell`在 1998 年给出的：

> 对于某个任务T和表现的衡量P，当计算机程序在任务T的表现上，经过P的衡量，随着经验E而增长，我们便称计算机程序能够通过经验E来学习该任务。

在上述的跳棋游戏的例子中，任务 T 是玩跳棋游戏，P 是游戏的输赢，而经验E 则是一局局的游戏。

一些机器学习的应用例子：

- 数据挖掘
- 一些无法通过手动编程来编写的应用：如自然语言处理，计算机视觉
- 一些自助式的程序：如推荐系统
- 理解人类是如何学习的

### 监督学习(Supervised Learning)

监督学习是什么呢？

下面我们用一个房价的例子来介绍下监督学习，如下所示:

![](http://7xrluf.com1.z0.glb.clouddn.com/FkTNm0ZRPQdxlQs2iraf9IHmG2KQ)

即通过给出房子面积和房价的一些数据，来预测一个新的房子面积所能卖出的房价。

所以，监督学习是指给出标记的数据集，并且已知输入和输出的关系，然后计算一个模型，可以对新的输入预测对应的输出结果。

**监督学习分为两类问题，分别是回归问题和分类问题**。回归问题的输出是一个连续值，比如在预测房价这个例子中，预测房价是一个回归问题，其结果是连续值。而分类问题是得到一个离散值的输出，比如同样是预测房价的例子，如果问题从预测卖出的房价变成卖出的房价是偏高还是偏低，就是属于分类问题，因为其答案可以用 0 或 1 表示高了或者低了。

课程中给出另一个例子说明分类问题，如下图所示：
![](http://7xrluf.com1.z0.glb.clouddn.com/FurKMwwrDt_NqXJmZcWqLjuvB6eZ)
问题是假设预测一个乳腺癌是否是恶性的，图中坐标轴横轴表示肿瘤的大小，纵轴表示病人的年龄，以 O 表示良性肿瘤，以X表示恶性肿瘤。所以问题就是判断是良性还是恶性肿瘤，这就是一个分类问题。

### 非监督学习(Unsupervised Learning)

在监督学习中，无论是回归问题还是分类问题，数据集都有一个明确的结果。

但非监督学习中，数据并没有一个结果，有的只是特征，即非监督学习要解决的问题是这些数据是否可以分成不同的组。

因此，非监督学习中典型的例子就是聚类问题。例如对一个大型的数据中心的网络传输数据情况进行分析，发现那些多数时候是在协作的计算机。

### 课程小结

这是第一节课程的内容，主要介绍了机器学习是什么，以及机器学习的两大学习问题--监督学习和非监督学习。

本节课程比较简单，但介绍的内容还是很重要的，后面介绍的大多数机器学习算法都属于监督学习或者非监督学习，当然实际上机器学习还不只有这两种学习问题，比如最近一两年开始热门起来的强化学习问题，以及半监督学习问题，但在吴恩达老师这门入门课程中并不会介绍这些内容。






