 ### 一、关于Object类
      1).Object类是所有类的父类，位于java.lang包中。
      2).数组也是Object类的子类。
      3).Object类的常用方法有：
               toString()：
                    *将任何一个对象转换成字符串返回，System.out.println()会调用toString()方法，打印对象。
                    *在类中如果不重写toString()方法， 结果会打印一个对象的哈希码值，地址的字符串，十六进制
                    *在类中重写toString()方法，结果会打印出对象的属性
                equals()：
                     *java当中所有类都是继承与Object这个基类，在Object的基类中定义了一个equals()的方法，这个方法的初始行为
                      是比较对象的内存地址，但是在一些类库中这个方法被覆盖掉了，如String,Integer,Date在这些类中equals()方法
                      有其自身的实现，覆盖了Object基类的equals()方法，会进行对象中内容详细的比较
                     *情况一：当某个类没有覆盖equals()方法，当通过equals()方法比较两个对象时，等价于“==”，即比较两个对象的内存地址。
                     *情况二：当某个类覆盖了equals()方法时，当通过equals()方法比较两个对象时，这时比较的是俩个对象的内容。
                 hashCode()：
                     *获取对象的哈希码值，为16进制
        4)Object类的使用：
                 Object类在java.lang包下，是所有类的根。任何类的对象，都可以调用Object类中的方法，包括数组对象。
