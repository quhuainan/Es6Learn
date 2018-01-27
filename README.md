# Es6Learn
1. 迭代器： 
    - 使用 for of 循环替代foreach 与for in
    - return 与break 不能跳出 foreach 循环
    - for in循环无序切会打印出多余属性

2. 生产器：
    - yield 关键字能够暂停函数执行，再次调用next()方法会继续执行
    - 生产器函数 命名后需要加* function*

3. 字符串模版：
    - 反撇号包围``
    - ``内的内容如果不是字符串会调用起object.toString()方法

4. 可变参数:
    - 使用...表示
    - 默认参数：在函数参数内直接申明参数取值，带有默认参数的值可以不传
    - 可选参数：在参数名后加上？表示该参数可传可不传

    ```
    funtion(arg1="1",arg2?:string,....arg3){}
    ```
5. 解构：
    - 数组解构:用[]包围变量值
    ```
     [var1,var2,....var3] =array
    ```
    - 对象解构:用{}包围变量值，并且解构的变量名称要与对象属性名称一致
    ```
        class Person{
            name:string,
            age:int,
        }
        let {name,age}=new Person("张三",27)
    ```

6. 箭头函数：可以省略funtion ,reuturn,小括号，分号
    - 简洁写法 value =》a=value
    - 常规写法 (value)=》{return value}
    -> 为了防止{}空对象 与{}空代码块的区别时，返回{}对象时需要在{}外层加上（）

7. Symbols:js第七种原始类型（Undefined,Null,Boolean,Number,String,Object)
    - symbol 是程序创建并且可以用作属性键的值,并且它能避免命名冲突的风险。

8. Babel: 将Es6代码转译为浏览器能够兼容的代码 ，Broccoli:对文件进行混淆与压缩

9. set与map:大部分性质与java 中相同
    - map 与set 中的元素顺序 就是元素插入的顺序
 