一、Java 基础

1.JDK 和 JRE 有什么区别？

* JDK是Java运行环境，JRE是可执行文件（JDK的压缩版）

2.== 和 equals 的区别是什么？

* ==是判断两个变量的地址是否相同，equals是判断两个变量的值是否相同

**答：都是判断两个对象的地址是不是相等（object比较两个对象的内存地址）。类覆盖了equals()方法，一般是两个对象内容是否相等。***

​		注：String中的equals方法是重写过的

3.两个对象的 hashCode()相同，则 equals()也一定为 true，对吗？、

* 不一定，两个值相同则hashcode一定相同，但hashcode相同，值不一定相同

4.final 在 java 中有什么作用？

* 定义不允许修改的变量和方法

5.java 中的 Math.round(-1.5) 等于多少？

* 

6.String 属于基础的数据类型吗？

* 不是基础的数据类型，基础的数据类型有 int、float、double、char、boolean，String是char数组

7.java 中操作字符串都有哪些类？它们之间有什么区别？

* StringBuffer String。。。

8.String str="i"与 String str=new String(“i”)一样吗？

* 第一个是把str的地址指向i，第二个是创建一个值为i的字符串对象

9.如何将字符串反转？

* 

10.String 类的常用方法都有那些？

* trim
* length
* charAt

11.抽象类必须要有抽象方法吗？

* 不必要的（不确定）

12.普通类和抽象类有哪些区别？

* 继承了抽象类的子类，必须实现抽象方法

13.抽象类能使用 final 修饰吗？

* 不能（不知道问什么）

14.接口和抽象类有什么区别？

* 继承抽象类，实现接口

  

15.java 中 IO 流分为几种？

* InputStream
* OutputStream
* BufferStream
* FileStream

16.BIO、NIO、AIO 有什么区别？

* 

17.Files的常用方法都有哪些？

* 

二、容器

18.java 容器都有哪些？

* List Set Map

19.Collection 和 Collections 有什么区别？

20.List、Set、Map 之间的区别是什么？

* list：链表数组，有序
* set：集合，无序
* map：键值对 key-value

21.HashMap 和 Hashtable 有什么区别？

* 

22.如何决定使用 HashMap 还是 TreeMap？

* 有排序需求使用TreeMap

23.说一下 HashMap 的实现原理？

* 用链表存储，冲突Hash值用数组存储，超过xx，用红黑二叉树实现

24.说一下 HashSet 的实现原理？

25.ArrayList 和 LinkedList 的区别是什么？

* arraylist 数据集合
* linkedlist 双向链表

26.如何实现数组和 List 之间的转换？

* list.asArray (list转数组)
* 循环add

27.ArrayList 和 Vector 的区别是什么？

* arraylist是不同步的 线程不安全的
* Vector是同步的，线程安全的

28.Array 和 ArrayList 有何区别？

* 

29.在 Queue 中 poll()和 remove()有什么区别？

* poll移除最先添加到队列中的元素
* remove移除任意位置的元素

30.哪些集合类是线程安全的？

* Vector
* ConcurrentHashMap

31.迭代器 Iterator 是什么？

32.Iterator 怎么使用？有什么特点？

33.Iterator 和 ListIterator 有什么区别？

34.怎么确保一个集合不能被修改？

* 加锁