---
title: Set and Multiset in STL
comments: true
date: 2017-09-14 09:21:38
updated: 2017-11-15 09:21:38
tags: [Set STL,Multiset STL]
categories: C/C++
permalink:
---
# 关联式容器概述

set和multiset是一种关联式容器，关联式容器依据特定的排序准则，自动为元素排序。所有的关联式容器都有一个可供选择的template参数，指明排序准则。排序准则以函数的形式呈现，用于比较元素值或元素键，默认情况下，从小到大排列。
主要的关联式容器包括set,multiset,map,multimap.其中set可以视为一种特殊的map，它的元素的值就是键的值。前两种需要包含set头文件，后两种要包含map头文件。

    set关键词和数据是同一个值，set容器中的所有的元素必须具有唯一值，不可重复。set对象可以一定的次序存储数据。
    multiset是另一种类型的容器，其关键词和数据元素也是同样的值。与set不同的是，它可以包含重复的元素。同样的multiset中的数据也是有次序的。
    map是一种包含成对数据的容器，一个值是实际的数据值，另一个值是用来寻找数据的关键值。一个特定的关键值只能与一个元素相联系。map中同一对键值只能出现一次.同样的其中的键值对也是按照特定的顺序排列的。
    multimap是允许重复键值的出现。