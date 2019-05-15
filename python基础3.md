1. Dict字典
1） 定义
字典(Dict)，是可变的无序集合，同时是一种以键值对为基本元素的可以存储各种数据类型的集合，用大括号({})表示字典的开始和结束，元素之间用逗号(，)隔开。
2） 创建
a.直接创建，冒号隔开;
My_dict = {‘key’:'value,‘hi’:‘hei’,…};
b.连接键值对;
My_dict = dict(key1=value1,key2=value2…)
c.创建一个空的，慢慢赋值;
My_dict={}
My_dict[key1]=value1
My_dict[key2]=value2
d.利用zip压缩两个序列里面的值，组成键值对
keys = [a,b,c,d]
values = [e,f,g,h]
My_dict = dict(zip(keys,values))
f.可全部初始化为一个值，然后需要的时候修改
list = [a,b,c,d]
My_dict = dict.fromkeys(list,‘?’)
其中?可以是任何你想要的值。
3） 字典的方法
1.dict.clear()
删除字典内所有元素

2.dict.copy()
返回一个字典的浅复制

3.dict.fromkeys(seq[, val])
创建一个新字典，以序列 seq 中元素做字典的键，val 为字典所有键对应的初始值

4.dict.get(key, default=None)
返回指定键的值，如果值不在字典中返回default值

5.dict.has_key(key)
如果键在字典dict里返回true，否则返回false

6.dict.items()
以列表返回可遍历的(键, 值) 元组数组

7.dict.keys()
以列表返回一个字典所有的键

8.dict.setdefault(key, default=None)和get()类似, 但如果键不存在于字典中，将会添加键并将值设为default

9.dict.update(dict2)
把字典dict2的键/值对更新到dict里

10.dict.values()
以列表返回字典中的所有值
11.pop(key[,default])
删除字典给定键 key 所对应的值，返回值为被删除的值。key值必须给出。
否则，返回default值。

12. popitem()
随机返回并删除字典中的一对键和值。

2. 集合
1） 特性
a.有的可变，有的不可变；元素无次序，不可重复。
b.集合中的元素不能重复，可作为一种简单高效的元素去重方式。
c.集合没有索引，它的元素无次序，不是序列。
d.利用set()和{}建立集合时，要求集合中的元素必须是可哈希(hsshable)的，即在利用set()和{}创建集合的时候，集合中的元素必须是不可变的。
f.利用set()创建的集合是可变集合，它的类型是不可哈希(unhashable)的。对于这句话的理解是，set()创建的集合，整体上是可变的，可以增、删；但集合中的元素(个体)是不可变(hashable)的，不能被修改，且集合中的元素不能是列表、字典等可变类型的对象。
2） 创建
可以使用大括号 { } 或者 set() 函数创建集合，注意：创建一个空集合必须用 set() 而不是 { }，因为 { } 是用来创建一个空字典。
创建格式：
parame = {value01,value02,…}或者set(value)
3） 方法
clear()移除集合中的所有元素

copy()拷贝一个集合


difference()返回多个集合的差集


difference_update()移除集合中的元素，该元素在指定的集合也存在。
discard()删除集合中指定的元素


intersection()返回集合的交集
intersection_update()
删除集合中的元素，该元素在指定的集合中不存在。


isdisjoint()判断两个集合是否包含相同的元素，如果没有返回 True，否则返回 False。


issubset()判断指定集合是否为该方法参数集合的子集。
issuperset()判断该方法的参数集合是否为指定集合的子集

pop()随机移除元素

remove()移除指定元素


symmetric_difference()返回两个集合中不重复的元素集合。
symmetric_difference_update()
移除当前集合中在另外一个指定集合相同的元素，并将另外一个指定集合中不同的元素插入到当前集合中。

union()返回两个集合的并集update()给集合添加元素

3. 判断语句（要求掌握多条件判断）
if <条件判断1>:
    <执行1>
elif <条件判断2>:
    <执行2>
elif <条件判断3>:
    <执行3>
else:
    <执行4>

4. 三目表达式
为真时的结果 if 判定条件 else 为假时的结果

5.循环语句
while 语句用于循环执行程序，即在某条件下，循环执行某段程序，以处理需要重复处理的相同任务。其基本形式为：
while 判断条件： 执行语句……
while 语句时还有另外两个重要的命令 continue，break 来跳过循环，continue 用于跳过该次循环，break 则是用于退出循环，此外"判断条件"还可以是个常值，表示循环必定成立
Python for循环可以遍历任何序列的项目，如一个列表或者一个字符串。
