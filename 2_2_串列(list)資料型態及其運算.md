列表|串列(list)資料型態及其運算
Python Arrays??
Python does not have built-in support for Arrays, but Python Lists can be used instead.

For details please see below

https://www.w3schools.com/python/python_arrays.asp

建立list
# -*- coding: utf-8 -*-

list1 = list() 
list2 = list([2, 3, 4])

list2 = [2, 3, 4] 
list3 = list(["red", "green", "blue"]) 
list4 = list(range(3, 6))
list5 = list("abcd") 

list1 = list() 
list1

list3 = list(["red", "green", "blue"])
list3

list4 = list(range(3, 6))
list4

List的各種運算(1)
下列範例會產生何種結果

list1 = [21, 33, 14, 12, 32,98]

len(list1)
max(list1)
min(list1)
sum(list1)

list1 = [21, 33, 14, 12, 32,98]
len(list1)
List的各種運算(2)串列的加法|乘法運算
下列範例會產生何種結果

list1 = [21, 23, 25]
list2 = [11, 92]

list3 = list1 + list2
list3
list4 = 3 * list1
list4
List的各種運算(3)切片運算(Slice)
list5 = list3[2:4]
list5
list的還有各種函數:
加一元素到串列的尾端:append()
回傳元素x 出現於串列的次數:count()
附加在l中所有元素於串列:extend()
回傳在串列中第一次出現元素x的索引:index()
將串列中的元素加以反轉:reverse()
由小至大排序串列中的元素:sort()
list的超強大功能:序列拆解

a=[12,212,321,325]
x,y,z,k = a
z

List comprehension 列表推導式: list的超強大功能
A list comprehension consists of brackets containing an expression followed by a for clause, 
then zero or more for or if clauses. 
The result will be a new list resulting from evaluating the expression 
in the context of the for and if clauses which follow it. 

https://en.wikipedia.org/wiki/List_comprehension
list1 = [x for x in range(0,5)] 
list1

list2 = [0.5 * x for x in list1] 
list2

list3 = [x for x in list2 if x <= 1.5]
list3
List comprehension�列表推導式的應用
阿基米德與圓王比賽下棋， 國王說要是自己輸了的 話，阿基米德想要什麼他都可以拿得出來。 阿基米德說那就要點米吧！ 
棋盤一共 64 個小格子，在第一個格子放 l粒米，第二個格子放 2 粒米，第三個格子放 4 粒米，第四個格子放 8粒米，餘依此頡推，
後面每個格子的米都是前一個格子的 2 倍，一直把 64 個格子都放滿。

到底需要多少粒米呢

sum([2**i for i in range(5)])

sum([2**i for i in range(64)])
