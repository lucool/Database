# Day1

### 

### 一、计算机简介

> 计算机的组成部分：输入设备，输出设备，存储器，运算器和控制器
>
> 输入设备：鼠标键盘【告诉电脑需要执行什么样的操作】
>
> 输出设备：显示屏和音响
>
> 机箱：主板【连接其他所有设备的载体】
>
> 	主板：cpu,内存，显卡，硬盘
>
> ​		cpu:中央处理单元【Central  Processing Unit】,也被称为处理器，是计算机 的运算核心和控制核心，让计算机中的各个部件顺利工作，能够协调的作用
>
> ​		内存：负责硬盘等硬件设备上的数据和cpu之间的交互，缓存程序运行的临时数据
>
> ​		显卡：显示屏想要显示画面
>
> ​		硬盘：存储资料和软件等数据，特点：容量大，关机后不会丢失数据，被称为数据仓库

### 二、软件开发的简介

#### 1.什么是软件

> 一系列按照特定顺序组织起来的计算机指令或者数据
>
> 软件的分类：
>
> ​	系统软件：Windows,Linux,Mac oS等操作系统
>
> ​		注意：系统软件是电脑底层的软件，可以控制计算机运行的程序并管理整个计算机的资源，是计算机硬件和应用程序之间的桥梁
>
> ​	应用软件：一系列浏览器，一系列播放器等

#### 2.什么是开发

> 简单来说，就是制作软件的过程
>
> 软件的出现实现了人与计算机之间的交互
>
> ​	交互方式：
>
> ​		图形化界面：
>
> ​		命令行方式：在终端输入指定的命令，计算机会根据命令做出相应的操作

#### 3.DOS命令

> DOS命令：一系列操作系统的命令，面向磁盘，主要包括目录操作或者文件操作等
>
> 按下windows + r 打开输入框，输入cmd【commad命令】打开终端
>
> ```Python
> cd xxx     :切换到指定路径下 【change directory】
> cd..	   ：退回到上一级目录
> cd..\..    :退回到上上一级目录
> cd/        :退回到根目录
> 
> 相对路径：从当前路径开始的路径,在实际项目开发中，特别是团队开发，一般采用相对路径，例如：cd Desktop
> 绝对路径：从盘符开始的路径，例如：cd C:\Users\Administrator\Desktop
> 
> dir       :列出当前路径下所有的内容
> 
> #目录
> md  xxxx      :在指定的路径下创建一个名字为xxx的文件夹【make  directory】
> rd  xxxx      :移除指定的目录，注意：只能删除空目录【remove directory】
> rd  /s  xxxx  :删除指定的目录，不管是否为空，会提示是否需要删除，输入y确定删除【交互式删除】  
> rd /s /q  xxx  :强制删除指定的目录，不会出现询问，删除之后没有任何痕迹
> 
> #文件
> #>：重定向符，将原本默认的输出路径改变为指定的路径
> cd>xxx.txt    :将cd输出的结果输出到xxx.txt文件中，注意：文件中默认有一行内容，为当前的路径
> type nul>xxx.txt  ：创建一个空文件
> copy nul>xxx.txt   :创建一个非空文件，注意：文件中默认有一行内容，为已复制一个文件
> echo xxxx>xxx.txt   :创建一个非空文件，文件中的内容可以自定义
> del xxxx.txt       ；强制删除指定文件
> del /p  xxxx.txt   ；在删除之前会询问是否需要删除
> 
> #复制移动
> copy 源路径  目标路径     ：将源路径下的内容拷贝到目标路径下
> 	注意：copy分为同名拷贝和异名拷贝
> 
> move 源路径  目标路径     ：将源路径下的内容移动到目标路径下
> 
> #重命名
> ren old  new  :将旧文件名称用新文件名称替换
> ```

### 三、Python简介

#### 1.编程语言

> 学习编程语言其实就是学习语法规则

#### 2.Python

2.1发展史

> 1989年被发明的
>
> 1991年，1.0版本发行【Java:1995年】
>
> 1999年，支持网站开发【Web开发】
>
> 2000年，2.0版本发布，构成了现在Python语言的基本框架
>
> 2004年，2.4版本发布，同时Python的web框架Django诞生
>
> 2008年.10，2.6版本发布
>
> 2008年.12，3.0版本发布，【3.0的版本和原来的2.x版本完全不兼容】
>
> 为了保留原来的项目，小版本更新2.6.1,2.6.2.....2.7
>
> 2010年，2.7版本发布

#### 2.2特点

> a.解释型语言【开发过程中没有了编译这个环节，直接运行即可，类似于php等】
>
> b.交互式语言【可以在终端通过Python命令进入命令模式，直接互动执行程序】
>
> c.面向对象的语言【Python支持面向对象的编码风格或者具有面向对象语言的特点：封装，继承，多态】注意：面向对象只是一种编程思想，并不是一门编程语言
>
> d.跨平台的语言【Python代码可以运行在Windows上，也可以运行在LInux上，同时也可以运行到Mac os上，类似Java，一处编写，多处运行】

2.3优缺点

> 优点：
>
> ​	a.简单易学【较少的关键字，语法比较简单】
>
> ​	b.易于阅读，易于维护
>
> ​	c.封装了很多的库
>
> ​	d.可扩展性【可以使用c或者c++完成Python不可能完成的功能，然后在Python程序中调用c程序或者c++程序】
>
> ​	e.可移植性【跨平台，一个Python程序可以被移植到不同的平台上】
>
> ​	f.数据库【mysql,MongoDB,Redis扥在Python中已经内置】
>
> ​	g.GUI编程【图形化界面编程】
>
> ​	h.可嵌入式【可以将Python程序嵌入到c或者c++中，让你的程序拥有shell脚本的能力】
>
> 缺点：
>
> ​	a.运行速度慢【和c程序比较慢，因为Python是解释型语言，代码在执行的时候会一行一行翻译成cpu能识别的机器码，但是，c程序是先编译，然后执行，所以速度较快】
>
> ​	b.代码不能加密【发布Python程序的时候发布的是源代码，任何解释型语言都有该特点】

2.4应用领域

> Python擅长的领域：web开发，爬虫，数据分析，自动化测试，运维，人工智能【人脸识别，车牌识别，语音识别等】

### 四、数据的存储

#### 1.思考问题

> a.计算机的作用
>
> ​	存储数据，快速处理数据
>
> b.数据存储在计算机的什么位置？
>
> ​	数据存储在内存中
>
> c.计算机怎样存储数据的？
>
> ​	搞清楚计算机怎样存储数字

#### 2.内存

> 内存是计算机重要的组成部分之一，是与cpu之间进行沟通，计算中所有程序的运行都是在内存中完成的
>
> 内存，Memory,也被称为内存储器，作用的是暂时存放cpu的运算数据，以及和硬盘等外部设备之间进行交互
>
> 帮助理解：内存中存储的数据采用的是开关原理，用0和1表示【一个房间----》8个开关，这个房间被称为一个字节，每个开关被称为比特或者位】
>
> 字节：计算机中处理数据的最小单位，用Byte表示，简写为B
>
> 比特【位】：计算机中表示数据的最小单位，用bit表示，简写为b
>
> 单位换算：
>
> ​	1B = 8b
>
> ​	B，KB,MB,GB,TB,PB,EB....DB
>
> ​	1KB= 1024B
>
> 总结：
>
> ​	计算机的内存中以二进制的方式存储数据的	

#### 3.进制

3.1什么是进制

> a.进制就是进位制，是已经被规定好的进位方法【十进制逢十进一，二进制逢二进一】
>
> b.常见的进制：二进制【0~1】，八进制【0~7,使用数字0表示】，十进制【0~9】，十六进制【0~9，a~f/A~F，使用数字0x或者0X表示】

3.2进制的特点

> a.每种进制都有特定的字符集
>
> b.每种进制采用的都是位置表示法
>
> ​	举例：
>
> ​		175-----》100-----》10（2）
>
> ​		 715----》10-----》10（1）
>
> ​                 751---》1------》10（0）
>
> ​          	 175 = 1 * 10（2） + 7 * 10（1） +5 * 10（0）
>
> c.进制之间的计算
>
> ​	举例：
>
> ​		19 + 2 = 21
>
> ​	0 + 0 = 0
>
> ​	1 + 0= 1
>
> ​	0 + 1 = 1
>
> ​	1 + 1 = 10
>
> ​	11 + 1 = 100

3.3进制之间的转换

> 3 + 5 = 8
>
> a.十进制-----》二进制
>
> 转换原理：
>
> ​	整数：对十进制整数除2取余运算，直到商为0，将每步得到的余数倒着写出来
>
> ​	小数：小数部分乘以2取整运算	，直到整数部分为1，然后将每步得到的整数顺着写出来
>
> b.二进制------》十进制
>
> ​	转换原理：将二进制按权【位置表示法】展开相加
>
> ​	举例：
>
> ​	0000 0110------》1 * 2（2） + 1 * 2（1） + 0 * 2（0） = 6
>
> ​	1001 0110 ----》150
>
> c.二进制-----》八进制
>
> ​	转换原理：将二进制从右往左进行分组，每三位为一组，不够时补0，然后将每组的二进制转换为十进制，连接起来就是对应的八进制
>
> ​	举例：
>
> ​	1001 0110-----》010   010   110------》2 2 6----》0226
>
> ​	1010001----》001   010   001----》1 2  1 -----》0121
>
> d.二进制------》十六进制
>
> ​	转换原理：将二进制从右往左进行分组，每四位为一组，不够时补0，然后将每组的二进制转换为十进制，连接起来就是对应的十六进制
>
> ​	10010110----》1001    0110----》9  6  ----》0x96
>
> ​	1010001----》0101     0001-----》5  1---->0x51
>
> ​	10111110-----》1011   1110-----》11 14  -----》b   e---->0xbe
>
> ​	111011----》0011   1011------》3   11----->3  b----->0x3b
>
> e.十进制-----》八进制或者十六进制
>
> ​	转换原理：
>
> ​		方式一：先将十进制转换为二进制，然后再将二进制转化为八进制或者十六进制
>
> ​		方式二：对十进制进行除以8或者16的运算，获取余数
>
> f.八进制或者十六进制------》十进制
>
> ​	转换原理：将八进制或者十六进制按权展开，相加即可
>
> 总结：
>
> ​	a.计算机存储数据，先开辟空间	，再存储数据【计算机开辟空间的最小单位为字节】	
>
> ​	b.数值是正负之分，计算机通过符号位区分正负数，用最高位表示符号位，0表示正数，1表示负数

#### 4.原码反码补码

> 表示方式：
>
> ​	原码：一个数的二进制形式，1表示负数，0表示正数
>
> ​	反码：将原码除了符号位之外其他位取反【0---》1,1----》0】
>
> ​	补码：在反码的基础加1【0000 0001】
>
> 注意：原码反码补码的求法主要针对的负数，正数的原码反码补码是同一个，都是该数的二进制
>
> ```
> 原码反码补码的求法：
> 6【正数】：
> 	0000 0110【原，反，补】
> 
> -6【负数】：
> 	0000 0110【6的二进制】
> 	1000 0110【-6的原码】
> 	1111 1001【-6的反码】
> 	1111 1010【-6的补码】
> ```
>
> ```
> 思考：计算机的底层存储数据采用的二进制【原反补】，计算机中存储数据采用的是原码？反码还是补码？
> 
> 验证：10 + （-10） = 0【以8位为例】
> 
> 10：
> 	0000 1010【原，反，补】
> -10：
> 	0000 1010【10的二进制】
> 	1000 1010【-10的原码】
> 	1111 0101【-10的反码】
> 	1111 0110【-10的补码】
> 	
> a.原码
>  0000 1010
>   + 1000 1010
>   -----------
>     1001 0100-----》结论：计算机底层处理数据采用的不是原码
>     
> b.反码
> 	0000 1010
> +    1111 0101
> ---------------
> 	1111 1111----》结论：计算机底层处理数据采用的不是反码
>  0000 0001【1原】-----》1000 0001【-1原】----》1111 1110【-1反】----》1111 1111【-1补码】    
>  
> c.补码
> 	0000 1010
> +    1111 0110
> ----------------
>     0000 0000------》溢出
>   
> 结论：计算机中处理数据采用的补码的形式
> 注意：计算机中只存在补码，补码给计算机识别的，对于而言，能够识别的是原码
> 
> 练习：
> 模拟计算机的运算过程，计算-5 + 3 = ？
> -5:0000 0101----》1000 0101---》1111 1010----》1111 1011
> 3:0000 0011
> 
> 1111 1011
> 0000 0011
> ----------
> 1111 1110【补】----》1111 1101【反】-----》1000 0010【-2的原】
> ```

#### 5.编码

> 在计算机中只能存储二进制数据，如果想要将文本，不同类型的文件存储在计算机中，通过一定格式的映射关系将这些数据转换为数字，最终不管是什么类型的数据，在计算机中都是以二进制的方式存储
>
> 举例：
>
> ​	a----->0001
>
> ​	b----->0010
>
> ​	....
>
> ​	z------>1111 1111
>
> ASCII码表，0~65535
>
> ​	48----》字符0
>
> ​	65----》大写字母A
>
> ​	97----->小写字母a
>
> UTF-8/utf8:国际编码
>
> GBK：中国编码
>
> Python2.x:默认编码为ASCII
>
> Python3.x:默认编码为Unicode，也默认支持中文

### 五、输入输出

#### 1.输出print

> ```Python
> import  sys
> 
> #print:打印，用于向控制台上输出任何类型的数据
> 
> #1.输出一个数据
> #注意：一个文本在代码中存在，只能以两种方式存在：注释和字符串
> print("hello world")   #字符串
> print('hello world~~~1111')  #字符串
> print(18)  #数字【整数】
> print(18.23)  #数字【浮点数】
> 
> #2.输出多个数据
> #注意：输出多个数据，到控制台上默认使用空格分隔
> print("hello world",'hello world~~~1111',18,18.23)
> 
> #3.使用占位符%进行格式化输出
> """
> %s:目前代表字符串
> %d:代表整数
> %f:代表浮点数
> """
> print("姓名：%s,年龄：%d,身高：%f")
> print("姓名：%s,年龄：%d,身高：%f" % ("zhangsan",18,173.2))
> 
> print("%s %s %d %f" % ("hello world",'hello world~~~1111',18,18.23))
> #\n:换行符
> print("%s\n%s\n%d\n%f" % ("hello world",'hello world~~~1111',18,18.23))
> 
> print("姓名：%s,年龄：%d,身高：%f" % ("zhangsan",18,173.23454))
> 
> #%.nf,保留小数点后n位，同时也会四舍五入
> print("姓名：%s,年龄：%d,身高：%.2f" % ("zhangsan",18,173.23454))
> print("姓名：%s,年龄：%d,身高：%.2f" % ("zhangsan",18,173.23754))
> 
> #4.sep关键字，表示分隔符,默认为空格，可以自定义为任意的字符串
> print("jack",18,18.23,"dance")
> print("jack",18,18.23,"dance",sep="*******")
> 
> #5.end关键字，表示结束符，默认为\n,可以自定义为任意的字符串，将不会自动换行
> print("1111")
> print("2222")
> 
> print("3333",end="*****")
> print("44444")
> 
> #注意：end和sep之间的区别
> print("jack",18,18.23,"dance",sep="*******")
> #print("jack",18,18.23,"dance",end="*******")
> 
> #6.file关键字，表示内容输出的位置，默认为控制台,可以自定义内容输出的位置
> #file关键字表示重定向print需要输出的数据
> print("hello~~~111")
> print("hello~~~2222",file=sys.stdout)
> 
> #a.打开文件
> f = open("file1.txt","w",encoding="utf-8")
> #写入数据
> print("hello~~~3333",file=f)
> #c.关闭文件
> f.close()
> ```

#### 2.输入input

> ```Python
> #input输入
> 
> 
> #注意：当代码执行到input，会出现阻塞，通过回车键解除阻塞
> """
> input()
> input("xxxxx"),xxxx表示提示性文字
> """
> 
> #1.
> # username = input("请输入你的姓名：")
> # print("姓名：%s" % (username))
> 
> print("over")
> 
> #2.
> num = input("请输入一个数字：")
> num1 = int(num)    #int(xxx）将xxx转换为整数
> print(num1 + 1)
> 
> 
> #结论：不管从控制台输入什么类型的数据，通过input获取后的类型都是字符串
> ```

### 六、其他

#### 1.第一个Python程序

> ```Python
> #命令行方式
> C:\Users\Administrator>python
> Python 3.6.0 (v3.6.0:41df79263a11, Dec 23 2016, 08:06:12) [MSC v.1900 64 bit (AMD64)] on win32
> Type "help", "copyright", "credits" or "license" for more information.
> >>> print("hello world")
> hello world
> >>> print(4343)
> 4343
> >>> import random
> >>> random.choice(range(10))
> 5
> >>> exit()
> 
> C:\Users\Administrator>cd Desktop
> 
> C:\Users\Administrator\Desktop>cd XA-Python1904
> 
> C:\Users\Administrator\Desktop\XA-Python1904>cd Day1
> 
> C:\Users\Administrator\Desktop\XA-Python1904\Day1>cd 代码
> 
> C:\Users\Administrator\Desktop\XA-Python1904\Day1\代码>dir
> 驱动器 C 中的卷没有标签。
> 卷的序列号是 DAFF-9D5E
> 
> C:\Users\Administrator\Desktop\XA-Python1904\Day1\代码 的目录
> 
> 2019/07/23  16:08    <DIR>          .
> 2019/07/23  16:08    <DIR>          ..
> 2019/07/23  16:09                20 first.py
> 2019/07/23  16:08                 0 新建文本文档.txt
>             2 个文件             20 字节
>             2 个目录  4,674,711,552 可用字节
> 
> #直接运行文件
> C:\Users\Administrator\Desktop\XA-Python1904\Day1\代码>python first.py
> hello world
> ```

#### 2.编码规范

> a.一行书写一条语句
>
> b.一旦使用到运算符【+-*/等】，尽量在运算符的前后添加空格
>
> ​    举例： 3 + 5 = 8
>
> c.一行代码尽量不超过80个字符，否则会导致代码可读性降低，可维护性降低
>
> d.使用缩进表示代码块【if语句，while语句等】
>
> ​	注意：四个空格表示一个缩进【pycharm可使用一个tab键】
>
> e.文件，项目以及变量等的命名尽量不要使用中文和空格

#### 3.注释

> ​	注释是写程序的时候，程序员给代码做的一个提示性文字，作用：能提高代码的可读性
>
> ​        特点：运行代码的时候，注释会被跳过，不做任何处理
>
> 表示方式：
>
> ​	a.单行注释：#xxxxx
>
> ​	b.多行注释："""xxxxxx"""    '''xxxxxx'''

#### 4.关键字和标识符

> 关键字：在Python中，已经被赋予了特殊含义的一些英文单词，例如：break，continue，finally，import等
>
> 标识符：在Python中，自定义的一些符号
>
> 定义合法标识符的规则【规则必须遵守，否则代码会报错】：
>
> ​	a.由数字，字母和下划线组成
>
> ​	b.不能使用空格和除了下划线以外的其他特殊符号
>
> ​	c.不能使用关键字和系统的函数名
>
> ​	d.不能以数字开头
>
> ​	e.严格区分大小写
>
> 定义标识符的规范【可以不遵守，但是代码不规范】：
>
> ​	a.尽量做到见名知意
>
> ​	b.表示形式
>
> ​		形式一：Python官方推荐的写法：所有的单词全部小写，不同单词之间使用下划线相连，举例：stu_score
>
> ​		形式二：驼峰命名法【大驼峰和小驼峰】
>
> ​			大驼峰：所有单词的首字母大写，类名一般采用大驼峰，举例：StuScore
>
> ​			小驼峰:除了第一个单词，其他单词的首字母大写，变量名和函数名一般采用小驼峰，举例：stuScore
>

# Day2

### 一、回顾

#### 1.默写题目

> 1.将十进制数15转化为二进制    1111【原反补】
>
> 2.求-20的补码    11101100
>
> 3.简述Python的特点
>
> 4.简述定义合法标识符的规则和规范
>
> 5.让用户从控制台输入姓名和年龄，并格式化输出【格式为：姓名：xxxx,年龄：xxx】
>
> ```Python
> name = input("请输入你的姓名：")
> age = input("请输入你的年龄：")
> #通过input获取的数据全部都是字符串
> 
> print("姓名：%s,年龄：%s" % (name,age))
> print("姓名：%s,年龄：%d" % (name,int(age)))
> ```

#### 2.知识点回顾

> 1.计算机组成
>
> ​	主板：cpu，内存，显卡，硬盘
>
> 2.软件开发
>
> ​	分类：应用软件和系统软件
>
> ​	DOS命令：了解
>
> 3.Python简介
>
> ​	Python的特点：解释型，交互式，面向对象，跨平台
>
> ​	Python的优缺点：
>
> ​		优：简单易学，易于维护，易于扩展，嵌入式，易于移植
>
> ​		缺：运行速度慢，代码不能加密
>
> 4.数据的存储
>
> ​	二进制【原码反码补码】
>
> ​	结论：数据在计算机中是以二进制的补码的形式存在的
>
> ​	           计算机中存储数据，需要给对应的数据开辟空间
>
> 5.其他
>
> ​	注释
>
> ​	关键字和标识符
>
> 6.输入输出
>
> ​	input()
>
> ​	print()

### 二、常量和变量

#### 1.Python原生的数据类型

> 计算机是用来存储数据，运算数据的，计算机能处理的数据不仅有数值，还有图片，音视频，网页等，处理不同的数据，需要不同的类型来表示不同的数据
>
> Python原生的数据类型：
>
> ​	number:数字型【整型int：整数，浮点型float：小数，复数：a + bj】
>
> ​	string:字符串型【str】
>
> ​	boolean:布尔型【True和False】
>
> ​	None:空值
>
> ​	数据结构：列表list，字典dict，元组tuple，集合set
>
> 说明：
>
> 整型：Python3.x中可以处理任意大小的整数【Python2.x中将整数分为int和long】
>
> 浮点型：在计算机的底层，浮点数使用科学计数法表示，举例：123.4567----》1.234567e2
>
> 字符串型：使用单引号或者双引号括起来的任意文本【包括数字，字母，中文，特殊符号】
>
> 布尔型：只有两个值，分别为True和False，一般用来表示判断结果，一般结合if语句或者while语句使用

#### 2.常量

> 在代码运行的过程中，值永远不会发生改变的标识符，举例;圆周率
>
> ```Python
> #常量
> 
> #整型
> print(18)
> 
> #浮点型
> print(10.34)
> 
> #字符串
> print("常量normal124324#￥%……")
> print('常量normal124324#￥%……')
> 
> #None
> print(None)
> ```

#### 3.变量

##### 3.1概念

> 在代码运行的过程中，值可以随时发生改变的标识符
>
> 在程序设计中，使用变量来进行存储数据，变量是一种存储数据的载体，但是，一个变量一次只能存储一个数据

##### 3.2定义

> 语法：变量名 = 值
>
> 说明：
>
> ​	a.变量名其实就是一个标识符，遵守标识符的规则和规范即可，也被称为引用
>
> ​	b.第一次给变量赋的值被称为初始值
>
> ​	c.定义变量的本质：在内存中开辟了空间，将特定类型特定数值的数据存储起来
>
> ```Python
> #1.需求：定义一个变量，表示一个人的年龄，初始值为18
> #=被称为简单赋值运算符
> age = 18
> print("age:%d" % (age))
> 
> #注意：一个变量必须定义之后才能使用，否则会报错
> #print(num)   #NameError: name 'num' is not definednum变量未被定义，
> # NameError表示一个类，表示异常
> 
> #2.变量的命名
> people_name = "zhangsan"
> peopleName = "zhangsan"
> 
> #3.其他类型的变量
> b1 = True
> b2 = False
> f1 = 1.234
> 
> #4.获取变量的类型：type()
> print(type(age))  #<class 'int'>
> print(type(people_name))  #<class 'str'>
> print(type(b1))   #<class 'bool'>
> print(type(f1))  #<class 'float'>
> 
> #5.给变量重新赋值
> #Python是一个弱类型的语言【一个变量被定义完成之后，在代码运行的过程，可以在更改数值的同时更改数据类型】
> #Python是一个动态类型的语言
> #Java, int num = 19
> num1 = 19    #初始值
> print(num1,type(num1))
> num1 = 20
> print(num1)
> num1 = "19"
> print(num1,type(num1))
> 
> #6.多个变量的定义
> #6.1定义多个变量，拥有同一个初始值
> num1 = num2 = num3 = 100
> # num1 = 100
> # num2 = 100
> # num3 = 100
> print(num1,num2,num3)
> 
> #6.2定义多个变量，拥有不同的初始值
> num1,num2,num3 = 11,22,33
> print(num1,num2,num3)
> 
> #7.常量的定义
> #常量命令法：所有的单词的字母全部大写，不同单词之间使用下划线分隔
> #在编程语言中，一般将常量用变量表示，但是标识符全大写，只是为了标记该变量是一个常量
> PI = 3.14
> print(PI)
> l1 = 10 * 2 * PI
> print(l1)
> 
> # PI = 100
> # print(PI)
> 
> 
> #8.变量的好处:可以存储数据，方便计算，简化了代码
> PI = 3.14
> radius = 20
> l1 = radius * 2 * PI
> print(l1)
> l1 = radius * 2 * PI
> print(l1)
> l1 = radius * 2 * PI
> print(l1)
> l1 = radius * 2 * PI
> print(l1)
> l1 = radius * 2 * PI
> print(l1)
> ```

##### 3.3内存中的变量

> 内存的划分：
>
> ​	寄存器：主要分配系统的资源，在代码中控制不了
>
> ​	栈：存储的变量的引用
>
> ​	堆：存储的是实体
>
> ​	方法区：
>
> ​		静态域：存储静态的数据【静态变量或者静态函数】
>
> ​		常量池：存储的是常用的常量
>
> ```Python
> name1 = "zhangsan"
> name2 = name1
> print(name1,name2)
> 
> #id(),获取一个变量在内存中的地址
> print(id(name1) == id(name2))
> 
> name1 = "jack"
> print(name1,name2)
> 
> print(id(name1) == id(name2))
> ```
>
> 总结;
>
> ​	在内存的堆空间中存储的实体一旦没有引用指向它，则该实体占用的空间会被释放掉【该实体会被销毁】
>
> ​	变量被销毁的工作原理：内存中的数据占用的空间不会自动释放，在Python的内部，有一个类似检测器的东西，会定时检测内存中有哪些变量没有指向，统一作出处理【没有指向的变量会被系统当做垃圾进行回收】
>
> Python的垃圾回收机制：Python内部使用引用计数，来保持追踪内存中的实体，一旦定义一个变量，该变量自带了一个引用计数，该变量每被重复使用，则引用计数会递增1，当指定的实体不被需要时，该对象的引用计数会变为0，则只能等待系统的垃圾回收机制回收，通过sys.getrefcount()	获取引用计数

##### 3.4删除变量

> 语法：del   变量名
>
> 作用：在程序未运行完成之前，可以手动删除变量，该变量对应的内存空间也会被释放掉
>
> 注意：一个变量一旦被删除，相当于该变量未被定义
>
> ```Python
> num1 = 66
> print(num1)
> 
> #手动删除变量，强制释放内存
> del num1
> 
> print(num1)   #NameError
> 
> print("over")
> ```

##### 3.5类型转换

> int(xx):将xx转换为整型
>
> float(xx)；将xx转换为浮点型
>
> str(xx)：将xx转换为字符串型
>
> chr(xx)：将一个整数转换为编码之后的字符【ASCII码】
>
> ord(xx)：将一个字符转换为编码之前的数字【ASCII码】
>
> ```Python
> #1.int(xx)
> num1 = 100
> print(type(num1))  #<class 'int'>
> 
> #a
> str1 = "123"
> int1 = int(str1)
> print(int(str1),type(int(str1)))
> print(int1,type(int1))
> 
> #b
> str1 = "123abc"
> #int1 = int(str1)   #ValueError: invalid literal for int() with base 10: '123abc'
> #print(int1,type(int1))
> 
> #c
> str1 = "+123"
> #str1 = "12+3"
> int1 = int(str1)
> print(int1,type(int1))
> 
> str1 = "-123"
> int1 = int(str1)
> print(int1,type(int1))
> 
> #d
> f1 = 18.93
> int1 = int(f1)
> print(int1,type(int1))
> 
> #e
> b1 = True
> int1 = int(b1)
> print(int1,type(int1))
> 
> print(True + 1)
> print(False + 1)
> 
> #注意：int(xx),xx可以是字符串，但是字符串中的字符只能由数字和正负号组成，但是，正负号只能出现的字符串的首位
> #xx也可以是float，相当于取整，不涉及四舍五入
> #xx也可以是布尔值，True相当于是1，False相当于0
> 
> #2.float(xx)
> #a
> int1 = 10
> f1 = float(int1)
> print(f1,type(f1))
> 
> #b
> str1 = "1023."   #0.1023 <class 'float'>
> f1 = float(str1)
> print(f1,type(f1))
> 
> #c
> str1 = "+10.23"
> #str1 = "1+0.23"  #ValueError: could not convert转化 string to float: '1+0.23'
> f1 = float(str1)
> print(f1,type(f1))
> 
> str1 = "-10.23"
> f1 = float(str1)
> print(f1,type(f1))
> 
> #d
> str1 = True
> f1 = float(str1)
> print(f1,type(f1))
> 
> #总结：float(xx),xx可以是整型，转化为float之后得到的结果为xx.0
> #也可以是字符串，字符串可以包含数字，点和正负号，但是，正负号只能出现在首位
> #也可以是布尔值，True是1.0，False是0.0
> 
> #3.str(xx)
> print(str(353))
> print(str(23.55))
> 
> 
> #4.chr()和ord()
> print(chr(65))
> #注意：ord其中的字符串的长度只能为1
> print(ord("b"))
> 
> #需求：从控制台输入一个大写字符，输出对应的小写字符，举例：E------》e
> ch = input("请输入一个大写字母：")
> #print(ch)
> num1 = ord(ch)   #TypeError: ord() expected a character, but string of length 9 found
> num1 = num1 + 32
> ch1 = chr(num1)
> print("%s-%s" % (ch,ch1))
> 
> ```

### 三、运算符和表达式【第一部分】

> 表达式：由运算符和操作数组成的式子被称为表达式

#### 1.算术运算符

> ```
> +    -    *    /      %【求余】    //【取整】   **【求幂】
> ```
>
> ```Python
> num1 = 5
> num2 = 3
> 
> print(num1 + num2)
> print(num1 - num2)
> print(num1 * num2)
> print(num1 / num2)
> print(num1 % num2)   #求余数
> print(num1 // num2)  #取整【取整数部分】
> print(num1 ** num2)
> print(num2 ** num1)
> 
> #注意:在算术运算符中，**的优先级最高
> #优先级的排序：** > * /  %  // >+  -
> print(2 ** 5 * 3)   #96
> print(2 * 5 ** 3)
> print((2 * 5) ** 3)
> ```

#### 2.赋值运算符

> ```
> 简单赋值运算符：=
> 复合赋值运算符：+=   -=   *=  /=   %=   //=   **= 
> 			由简单赋值运算符和算术运算符组成
> 
> ```
>
> ```Python
> num1 = 10
> 
> #注意：赋值运算符出现在一个表达式中，先计算=的右边，然后给=的左边进行赋值
> num1 = num1 + 23
> 
> """
> 在计算机的底层的工作原理:
> num1 = num1 + 23
> 
> 第一步：temp = num1 + 23
> 第二步：num1 = temp
> """
> 
> #等价于
> num1 += 23  #在加法运算的同时赋值
> 
> ```

#### 3.关系运算符

> 关系运算符，被称为条件运算符，比较运算符
>
> ```
> >    <    >=    <=     ==【恒等于，注意区别=】   !=【不等于】
> 
> 注意：关系运算符运算完成之后得到的结果都是布尔值，要么成立【True】，要么不成立【False】
> 使用场景：一般结合if语句，while语句使用
> 
> ```
>
> ```Python
> num1 = 10
> num2 = 20
> 
> print(num1 > num2)
> print(num1 == num2)
> print(num1 != num2)
> print(num1 <= num2)
> 
> 
> #练习
> #需求：从控制台输入一个年龄，假设一个人能活到100岁，计算还能活多少年
> age = input("请输入你的年龄：")
> DEATH_AGE = 100
> 
> #isdigit()判断一个字符串是否是由全数字组成
> if age.isdigit():
>     age = int(age)
>     if age >= 0 and age <= 100:
>         total = DEATH_AGE - age
>         print("还剩下%d年" % (total))
>     else:
>         print("你输入的年龄超出了界限")
> else:
>     print("输入有误")
> 
> ```

#### 4.位运算符【了解】

> ```
> &【按位与】   |【按位或】    ^【按位异或】   ~【取反，注意区分反码】
> <<【左移】   >>【右移】
> 
> ```
>
> 1为真，0为假
>
> ```Python
> print(6 & 3)
> print(8 & 4)
> 
> print(6 | 3)
> print(8 | 4)
> 
> print(6 ^ 3)
> 
> print(~6)
> 
> print(6 << 2)
> print(8 << 3)
> 
> print(6 >> 2)
> print(8 >> 3)
> 
> print(-6 >> 2)
> print(-8 >> 3)
> 
> ```

### 四、分支语句-if语句【重点掌握】

#### 1.概念

> 代码在执行的过程中，遇到了分支语句，根据条件的成立与否决定执行哪些代码

#### 2.使用

##### 2.1if语句：单分支

> 语法：
>
> ​	if  表达式：
>
> ​		语句
>
> 说明：
>
> ​	a.工作原理：如果表达式成立【表达式的结果为真】，则执行语句；如果不成立，则直接跳过整个if语句执行后面的代码
>
> ​	b.表达式可以是常量，变量或者运算表达式
>
> ​	c.何为真假？
>
> ​		假：0   0.0     “”    False     None   []   ()   {}
>
> ```Python
> import  random
> 
> 
> #单分支
> #1.需求：根据条件给变量重新赋值
> num1 = 10
> num2 = 20
> 
> #a.表达式是运算符表达式：比较运算符
> if num1 == num2:
>  num1 = 100
> 
> print(num1)
> 
> #b,表达式是常量
> if 1:
>  print("ok~~111")
> 
> #c,表达式是变量
> n = 0
> if n:
>  print("ok~~~222")
> 
> #2.需求：从控制台输入一个数，判断该数是否是偶数
> num1 = int(input("请输入一个数："))
> 
> if num1 % 2 == 0:
>  print("%s是一个偶数" % (num1))
> 
> #print("%s是一个奇数" % (num1))
> 
> #3.需求：模拟彩票【随机获取一个数，和控制台输入的数比较，如果相等，则中奖】
> """
> 随机数的获取
> 第一步：导入模块，import random
> 第二步：获取随机数，random.choice(range(100))
> 
> random.choice(range(start,end,step))
>  start:开始，可以省略，默认为0
>  end：结束数字，end取不到值
>  step：步长，可以省略，默认为1
> 
>  [start,end)
> 
> 举例：
> random.choice(range(100)) 获取0~99之间的整数随机数
> random.choice(range(20,100))获取20~99之间的整数随机数
> random.choice(range(1,100,2))获取1~99之间的奇数随机数
> #random.choice(range(100,2)) 错误写法
> """
> 
> #获取随机数
> num1 = random.choice(range(1000))
> print(num1)
> #获取输入的数
> num2 = int(input("请输入一个数:"))
> #比较
> if num1 == num2:
>  print("中奖")
> 
> ```

##### 2.2if-else语句：双分支

> 语法：
>
> ​	if  表达式：
>
> ​		语句1
>
> ​         else:
>
> ​		语句2
>
> 说明：
>
> ​	如果表达式成立，则执行语句1，如果不成立，则执行语句2，实现了二选一的操作
>
> ```Python
> import  random
> 
> """
> #1.需求：从控制台输入一个数，判断该数是否是偶数
> num1 = int(input("请输入一个数："))
> 
> if num1 % 2 == 0:
>  print("%s是一个偶数" % (num1))
> else:
>  print("%s是一个奇数" % (num1))
> 
> # 2.需求：模拟彩票【随机获取一个数，和控制台输入的数比较，如果相等，则中奖】
> # 获取随机数
> num1 = random.choice(range(1000))
> print(num1)
> # 获取输入的数
> num2 = int(input("请输入一个数:"))
> # 比较
> if num1 == num2:
>  print("中奖")
> else:
>  print("谢谢参与")
> """
> 
> #3.从控制台输入一个年龄，输出对应的阶段
> age = int(input("请输入你的年龄："))
> if age > 18:
>  print("成年")
> else:
>  print("未成年")
> 
> ```

##### 2.3if-elif-else语句：多分支

> 语法：
>
> ​	if  表达式1：
>
> ​		语句1
>
> ​        elif 表达式2:
>
> ​		语句2
>
> ​       elif 表达式3:
>
> ​		语句3
>
> ​	。。。。
>
> ​         else:
>
> ​		语句n
>
> 说明：
>
> ​	实现多选一的操作【注意：不管if-elif-else语句中有多少个条件成立，都只会执行其中的一个分支】，从上往下依次进行判断，一旦遇到一个条件成立，则执行对应的分支，然后整个语句全部结束
>
> ```Python
> #1.从控制台输入一个年龄，输出对应的阶段
> age = int(input("请输入你的年龄："))
> if age < 0:
>  print("输入有误，年龄不能为负数")
> elif age <= 3:
>  print("婴儿")
> elif age <= 12:
>  print("儿童")
> elif age <= 18:
>  print("少年")
> elif age <= 35:
>  print("青年")
> elif age <= 60:
>  print("中年")
> elif age <= 100:
>  print("老年")
> else:
>  print("老妖怪")
> 
> #2.需求：从控制台输入成绩，输出成绩的等级
> """
> 90~100  优秀
> 80~90  良好
> 70~80   一般
> 60~70  合格
> 60以下   加油吧，少年
> """
> score = float(input("请输入一个成绩："))
> if score > 100:
>  print("满分100")
> elif score >= 90:
>  print("优秀")
> elif score >= 80:
>  print("良好")
> elif score >= 70:
>  print("一般 ")
> elif score >= 60:
>  print("合格")
> elif score >= 0:
>  print("加油吧，少年")
> 
> ```
>
> ```Python
> #三者之间的区别
> n = 3
> 
> #多分支：多选一
> if n > 1:
>  print("a")
> elif n > 2:
>  print("b")
> elif n > 3:
>  print("c")
> else:
>  print("d")
> 
> #单分支：要么执行，要么不执行
> if n > 1:
>  print("a")
> if n > 2:
>  print("b")
> 
> #双分支：二选一
> if n > 3:
>  print("c")
> else:
>  print("d")
> 
> ```

##### 2.4嵌套if语句

> 嵌套if语句是单分支，双分支和多分支之间可以进行任意的嵌套，从理论上来说，嵌套的层数没有限制，但是，为了代码的可读性和后期的可维护性，嵌套的层数不要超过三层
>
> ```Python
> #注意：在嵌套if语句中，注意语句的缩进，弄明白语句属于哪个if
> 
> score = float(input("请输入一个成绩："))
> #1.双分支
> if score >= 0:
>  #2.单分支
>  if score <= 100:
>      #3.多分支
>      if score >= 90:
>          print("优秀")
>      elif score >= 80:
>          print("良好")
>      else:
>          print("加油")
>  print("111")
> else:
>  print("成绩不能为负数")
> 
> ```

# Day3

### 一、上堂回顾

#### 1.默写题目

> 1.列出Python常用的数据类型
>
> ```Python
> number,string,boolean,None,list,tuple,dict,set
> 数字型，字符串型，布尔型，空值，列表，元组，字典，集合
> ```
>
> 2.定义一个整型变量，将其转换为字符串类型，最后删除该变量
>
> ```Python
> num = 38
> str1 = str(num)
> del num
> 
> num = 38
> num = str(num)
> del num
> ```
>
> 3.从控制台输入一个数，判断该数是否是奇数
>
> ```Python
> num = int(input("xxx"))
> if num % 2 == 0:
>  print("偶数")
> else:
>  print("奇数")
>  
> if num % 2 == 1:
>  print("奇数")
> else:
>  print("偶数")
>  
> if num % 2 != 0:
>  print("奇数")
> else:
>  print("偶数")
> ```

#### 2.知识点回顾

> 1.变量
>
> ​	定义
>
> ​	内存中的变量：变量的引用存储在栈空间中，实体存储在堆空间中
>
> ​	Python的垃圾回收机制：引用计数
>
> ​	删除变量：del  变量名
>
> ​	类型转换：int()    str()
>
> 2.运算符
>
> ​	算术：% 【求余，取模】     //【取整】     **【求幂】
>
> ​	赋值：复合【作用：运算的同时赋值】
>
> ​	关系：运算完的结果都是布尔值
>
> 3.if语句
>
> ​	单分支：要么执行，要么不执行
>
> ​	双分支：二选一
>
> ​	多分支：多选一

#### 3.作业讲解

> ```Python
> #1.x 为 0-99 取一个数,y 为 0-199 取一个数,如果 x>y 则输出 x， 如果 x 等于 y 则输出 x+y，否则输出y
> import  random
> 
> x = random.choice(range(100))
> y = random.choice(range(200))
> 
> if x > y:
>  print(x)
> elif x == y:
>  print(x + y)
> else:
>  print(y)
> 
> #2.从控制台输入三个数，输出较大的值
> #假设法：定义一个新的变量，初始值为三个数中的任意一个，用该变量记录三个数中的最大值
> num1 = int(input("one"))
> num2 = int(input("second"))
> num3 = int(input("third"))
> 
> maxValue = num1
> 
> if num2 > num1:
>  maxValue = num2
> 
> if num3 > maxValue:
>  maxValue = num3
> 
> print(maxValue)
> 
> #3.从控制台输入一个三位数，如果是水仙花数就打印“是水仙花数”，否则打印“不是水仙花数”
> #例如：153=1^3+5^3+3^3
> 
> num = int(input("请输入一个三位数："))
> 
> gw = num % 10
> sw = num % 100 // 10
> bw = num // 100
> 
> result = gw ** 3 + sw ** 3 + bw ** 3
> #result1 = pow(gw,3) + pow(sw,3) + pow(bw,3)
> 
> if num == result:
>  print("%d是一个水仙花数" % (num))
> ```

### 二、运算符和表达式【第二部分】

#### 1.逻辑运算符

> 作用：进行逻辑运算的，用于判断，运算完成之后得到一个布尔值，一般结合if语句使用
>
> ```
> 逻辑与：and       逻辑或：or     逻辑非：not
> ```
>
> 基本使用
>
> ```Python
> #1.and
> num1 = 10
> num2 = 20
> 
> """
> 表达式1  and  表达式2  = ？
> 
> True and True = True
> True and False = False
> False and True = False
> False and False = False
> 
> 规律：全真为真，一假为假
> """
> #a.常量或者变量充当表达式
> #算术运算符可以和逻辑运算符使用
> if num1 and num2 - 20:
>  print("ok")
> else:
>  print("no ok")
> 
> #赋值运算符结合逻辑运算符使用-----》不能
> # if num1 += 1 and num2 - 20:
> #     print("ok")
> # else:
> #     print("no ok")
> 
> #关系运算符结合逻辑运算符使用-----》不能
> if num1 > num2 and num1 == num2:
>  print("ok")
> else:
>  print("no ok")
> 
> 
> #2.or
> """
> 表达式1  or  表达式2  = ？
> 
> True or True = True
> True or False = True
> False or True = True
> False or False = False
> 
> 规律：全假为假，一真为真
> """
> if num1 or num2 - 20:
>  print("ok")
> else:
>  print("no ok")
> 
> if num1 > num2 or num1 == num2:
>  print("ok")
> else:
>  print("no ok")
> 
> 
> #3.not
> """
> not  表达式  = ？
> 
> not True = False
> not False = True
> """
> if not num1 > num2:
>  print("成立")
> else:
>  print("不成立")
> 
> 
> #练习：实现用户的登录过程
> #让用户从控制台输入用户名和密码，当用户名为admin并且密码为123，则登录成功
> username = input("请输入用户名：")
> password = input("请输入密码：")
> 
> #方式一
> if username == "admin" and password == "123":
>  print("登录成功")
> else:
>  print("登录失败")
> 
> #方式二
> if username == "admin":
>  if password == "123":
>      print("登录成功")
>  else:
>      print("密码错误")
> else:
>  print("用户名错误")
> ```
>
> 短路原则
>
> ​	a.A and B,如果A为False，不需要计算B的值，直接得出整个表达式的值为False
>
> ​	b.A or B,如果A为True，不需要计算B的值，直接得出整个表达式的值为True
>
> ​	c.and和or混用
>
> ​		1>表达式从左往右进行运算，如果or的左侧为True，则会短路or后面所有的表达式【不管后面的表达式使用and还是or连接】，整个表达式的值为True
>
> ​		2>表达式从左往右进行运算，如果and的左侧为False，则会短路后面所有的and，直到or出现，接着计算
>
> ​		3>表达式从左往右进行运算，如果or的左侧为False，and的左侧为True，则不符合短路原则，只能挨个判断
>
> ```Python
> # def test():
> #     print("hello")
> #     return False
> # t = test()
> # print(t)
> 
> #1.运算符全部是and，第一个表达式的值为False
> def a():
>  print("A")
>  return False
> def b():
>  print("B")
>  return True
> def c():
>  print("C")
>  return False
> def d():
>  print("D")
>  return True
> def e():
>  print("E")
>  return False
> 
> #and的左边为False，则会短路后面所有的表达式，整个表达式的值为False
> if a() and b() and c() and d() and e():
>  print("ok~~~1111")
> 
> print("*" * 30)
> 
> #2.运算符全部是and，第一个表达式的值为True
> def a():
>  print("A")
>  return True
> def b():
>  print("B")
>  return True
> def c():
>  print("C")
>  return False
> def d():
>  print("D")
>  return True
> def e():
>  print("E")
>  return False
> """
> True and True and False  and True and False
> True  and False  and True and False ------>打印A,B
> False and True and False ------>打印C
> 整个表达式的值：False
> """
> 
> """
> True and True and True  and True and False
> """
> if a() and b() and c() and d() and e():
>  print("ok~~~222")
> 
> print("*" * 30)
> 
> #3.运算符全部是or，第一个表达式的值为True
> def a():
>  print("A")
>  return True
> def b():
>  print("B")
>  return True
> def c():
>  print("C")
>  return False
> def d():
>  print("D")
>  return True
> def e():
>  print("E")
>  return False
> 
> #True or True or False or True or False
> #or的第一个表达式为True，则会短路后面所有的表达式，整个表达式的结果为True
> if a() or b() or c() or d() or e():
>  print("ok~~~3333")
> 
> print("*" * 30)
> 
> #4.运算符全部是or，第一个表达式的值为False
> def a():
>  print("A")
>  return False
> def b():
>  print("B")
>  return False
> def c():
>  print("C")
>  return False
> def d():
>  print("D")
>  return True
> def e():
>  print("E")
>  return False
> 
> """
> False or True or False or True or False
> True or False or True or False----->打印A,B
> 整个表达式的为True
> """
> 
> """
> False or False or False or True or False
> False or False or True or False----->打印A,B
> False  or True or False----->打印C
> True or False----->打印D
> 整个表达式的为True
> """
> if a() or b() or c() or d() or e():
>  print("ok~~~44444")
> 
> print("*" * 30)
> 
> #5.
> def a():
>  print("A")
>  return False
> def b():
>  print("B")
>  return False
> def c():
>  print("C")
>  return True
> def d():
>  print("D")
>  return False
> def e():
>  print("E")
>  return True
> def f():
>  print("F")
>  return False
> def g():
>  print("G")
>  return False
> def h():
>  print("H")
>  return False
> def i():
>  print("I")
>  return True
> def j():
>  print("J")
>  return False
> #   A        B         C         D         E          F          G            H           I       J
> #False and False and True  and  False or True and   False  or   False   and  False  and True or False
> 
> """
> False and False and True  and  False or True and   False  or   False   and  False  and True or False
> False  or True and   False  or   False   and  False  and True or False ----->打印A
> True and   False  or   False   and  False  and True or False---->打印E
> False or   False   and  False  and True or False ---->打印F
> False and  False  and True or False ---->打印G
> False or False  ---->打印J
> 整个表达式的结果为False
> """
> if a() and b() and c() and d() or e() and f() or g() and h() and i() or j():
>  print("ok~~~~555")
> """
> AE  ok
> AEFG
> """
> 
> print("*" * 30)
> 
> #6.
> def a():
>  print("A")
>  return False
> def b():
>  print("B")
>  return False
> def c():
>  print("C")
>  return True
> def d():
>  print("D")
>  return False
> def e():
>  print("E")
>  return True
> def f():
>  print("F")
>  return True
> def g():
>  print("G")
>  return False
> def h():
>  print("H")
>  return True
> 
> #  A           B        C          D         E        F        G        H
> #False  and  False and True  and  False  or True and True or False and True
> 
> """
> False  and  False and True  and  False  or True and True or False and True
> False or True and True or False and True--->打印A
> True  and True or False and True---->打印E
> True  or False and True----->打印F
> 
> 整个表达式的值为True
> """
> #AEFGH   ok
> #AEF   ok
> #AE   ok
> if a() and b() and c() and d() or e() and f() or g() and h():
>  print("ok~~~~666")
> ```

#### 2.成员运算符

> 作用：判断一个数据在一个容器中是否存在
>
> in:判断一个数据在容器中是否存在，如果存在，结果为True
>
> not in :判断一个数据在容器中是否不存在，如果不存在，结果为True

#### 3.身份运算符

> 作用：用于比较两个实体的存储地址
>
> is:判断两个变量的地址是否一致【判断两个标识符是否引用自同一个对象】
>
> is not：判断两个变量的地址是否不一致【判断两个标识符是否引用自不同的对象】
>
> 【区别is和==】
>
> ```Python
> a = 10
> b = 10
> 
> #1
> print(a == b)
> print(id(a) == id(b))
> print(a is b)
> 
> 
> #2.
> b = 20
> 
> print(a == b)
> print(id(a) == id(b))
> print(a is b)
> 
> """
> 结论：
>  a.==比较的是内容，is比较的是地址
>  b.两个变量的地址相同，则两个变量的内容一定相同的，但是，两个变量的内容相同，则地址不一定相同
> """
> ```

#### 4.三目运算符【三元运算符】

> Guido Van Rossum
>
> Python中的三元运算符的实现：
>
> ​	a.利用逻辑运算符的短路原则
>
> ​	b.if语句
>
> ```Python
> #三目运算符：实现二选一的操作，简化if-else代码
> 
> a = 10
> b = 20
> 
> #1.
> #语法：bool  and 数据1 or  数据2
> #如果bool为真，整个表达式的值为数据1；如果bool为假，整个表达式的值为数据2
> result = (3 == 5) and a or b
> result = False and a or b
> print(result)
> 
> result = 0
> if True:
>  result = a
> else:
>  result = b
> 
> 
> #2.
> 
> result = False and a or b
> print(result)
> 
> result = a if False else b
> print(result)
> 
> 
> #练习1:判断一个数是否是偶数
> num = 18
> #方式一
> result = ""
> if num % 2 == 0:
>  #print("偶数")
>  result = "偶数"
> else:
>  #print("奇数")
>  result = "奇数"
> print(result)
> 
> #方式二
> result = (num % 2 == 0) and "偶数" or "奇数"
> print(result)
> 
> #方式三
> result = "偶数" if (num % 2 == 0) else "奇数"
> print(result)
> 
> 
> #练习2：判断一个年份是否是闰年
> year = 2000
> 
> result = ((year % 4 == 0 and year % 100 != 0)  or  year % 400 == 0)  and "闰年" or "平年"
> 
> result = "闰年" if ((year % 4 == 0 and year % 100 != 0)  or  year % 400 == 0) else "平年"
> ```
>
> 运算符的优先级：
>
> ​	a.实现逻辑比较复杂的代码，尽量分步执行
>
> ​	b.在具有多种运算符的表达式中，尽量使用括号区分优先级

### 三、循环语句-while语句【重点掌握】

#### 1.概念

> 在满足条件的情况下，反复执行某一段代码，在编程语言中出现这种现象被称为循环，这段被重复执行的代码被称为循环体
>
> 问题：当反复执行某段代码，需要在合适的时机将条件改为假，从而结束循环，否则会形成死循环
>
> Python中的循环语句：while语句和for语句

#### 2.基本使用

> 语法：
>
> if  表达式：
>
> ​	语句
>
> while 表达式：
>
> ​	语句
>
> 说明：
>
> ​	a.在条件成立的前提下，if语句只会被执行一次，但是，while语句至少执行一次
>
> ```Python
> #1.需求：打印10遍hello world
> # if True:
> #     print("hello world")
> #
> # while True:
> #     print("hello world")
> 
> #问题：控制循环的次数
> #书写一个完整的循环，需要四个要素
> #a.初始化表达式
> #定义一个变量，用于控制循环的次数
> n = 0
> 
> #b。条件表达式
> while n < 10:
>  #c。循环体
>  print("hello world")
>  #d.循环之后的操作表达式
>  n += 1
> 
> print("over")
> 
> #2.需求：打印0~9的数字
> n1 = 0
> while n1 <= 9:
>  print(n1)
>  n1 += 1
> 
> #3.需求：打印一个字符串中的每个字符
> str1 = "abcd123hserhsreh"
> #print(str1)
> 
> index = 0
> while index < len(str1):
>  #字符串名[下标]
>  ch = str1[index]
>  print(ch)
>  index += 1
> ```

#### 3.死循环

> 使用场景：如果不能确定循环的次数，则直接使用死循环
>
> 语法：
>
> while True:
>
> ​	循环体
>
> while 1:
>
> ​	循环体

#### 4.else分支

> 语法：
>
> ​	while 条件：
>
> ​		循环体
>
> ​	else:
>
> ​		语句
>
> ```Python
> #1.在if语句中，只有当条件不成立时，else才会被执行
> # a = 1
> # if a < 3:
> #     print("aaa")
> # else:
> #     print("else被执行了")
> 
> 
> #2,在while语句中，不管条件是否成立，else都会被执行
> #如果条件成立的情况下，当while语句中的循环体执行完毕，最后才执行else
> a = 1
> while a > 3:
>  print("aaa")
>  a += 1
> else:
>  print("else被执行了")
> 
> print("over")
> ```

#### 5.嵌套循环

> ```Python
> #1
> n = 0
> m = 0
> while n < 3:    #n:0,1,2
>  while m < 5:  #m:0,1,2,3,4
>      print("%d=%d" % (n,m))
>      m += 1
>  n += 1
> 
> #2
> n = 0
> while n < 3:    #n:0,1,2
>  m = 0
>  while m < 5:  #m:0,1,2,3,4
>      print("%d=%d" % (n,m))
>      m += 1
>  n += 1
> 
> #3.打印九九乘法表
> """
>                                                  行       列
> 1x1=1                                               1         1
> 1x2=2  2x2=4                                        2           2
> 1x3=3 2x3=6 3x3=9                                   3           3
> .....
> 
> 1x9=9 2x9=18    ......   8x9=72 9x9=81              9         9
> 
> 规律：
>  1.表达式的格式：列x行=乘积
>  2.列数的最大值是当前行的行数
>  3.行数的取值范围：1~9
> """
> 
> #外层循环：控制的是行
> line = 1
> while line <= 9:
> 
>  #内层循环：控制每行中的列
>  colum = 1
>  while colum <= line:
>      print("%dx%d=%d" % (colum,line,line * colum),end=" ")
> 
>      colum += 1
> 
>  #换行
>  print()
>  line += 1
> 
> 
> #练习：打印图形
> """
> *
> **
> ***
> ****
> *****
> """
> #方式一
> i = 1
> while i <= 5:
>  j = 1
>  while j <= i:
>      print("*",end="")
>      j +=1
>  print()
>  i += 1
> 
> #方式二
> print("*" * 30)
> 
> i = 1
> while i <= 5:
>  print("*" * i)
>  i += 1
> ```

#### 6.练习

> ```Python
> #练习：
> #1.求1~100之间所有整数的和
> n1 = 1
> #定义一个新的变量，用于记录和
> total1 = 0
> while n1 <= 100:
>  #求和
>  total1 += n1
>  n1 += 1
> print(total1)
> 
> #2.求1~100之间所有偶数的和
> #方式一
> n2 = 1
> total2 = 0
> while n2 <= 100:
>  if n2 % 2 == 0:
>      total2 += n2
>  n2 += 1
> #方式二
> n21 = 0
> total21 = 0
> while n21 <= 100:
>  total21 += n21
>  n21 += 2
> 
> # 3.求10的阶乘【10*9*8.。。。*1】
> n3 = 1
> result = 1
> while n3 <= 10:
>  result *= n3
>  n3 += 1
> 
> # 4.统计100~1000之间能被6整除的数的个数
> n4 = 100
> count1 = 0
> while n4 <= 1000:
>  if n4 % 6 == 0:
>      count1 += 1
>  n4 += 1
> 
> # 5.求100~1000之间7的倍数的和
> n5 = 100
> total5 = 0
> while n5 <= 1000:
>  if n5 % 7 == 0:
>      total5 += n5
>  n5 += 1
> 
> # 6.求1-2+3-4+5-6.....+99-100的结果
> n6 = 1
> total6 = 0
> while n6 <= 100:
>  if n6 % 2 == 0:
>      total6 -= n6
>  else:
>      total6 += n6
>  n6 += 1
> 
> print(total6)
> ```

### 四、break，continue语句【重点掌握】

#### 1.pass

> 对于代码块而言，pass相当于是一个占位符，为了让当前的代码正常执行，可以使用pass语句，为了保证程序结构的完整性
>
> ```Python
> if True:
>  pass
> 
> while True:
>  pass
> ```

#### 2.break

> 作用：在Python中，break语句只能使用在循环语句中，表示结束整个循环【结束当前循环】
>
> ```Python
> #1.break应用在单循环中
> n = 0
> while n < 10:
> 
>  #注意1：break只能使用在循环语句中，此处的if语句仅仅条件的限制
>  if n == 3:
>      #注意2：break是一个关键字，同时也可以单独作为一条语句使用
>      break
> 
>  print(n)
>  n += 1
> 
> 
> #2.break应用在嵌套循环中
> #注意3：break应用在嵌套循环中，跳出的是当前循环
> n = 0
> while n < 3:
>  m = 0
>  while m < 5:
>      if m == 3:
>          break
>      print("%d=%d" % (n,m))
>      m += 1
>  n += 1
> 
> 
> #3.特殊情况：当while循环中出现break，则else不会被执行
> n = 0
> while n < 10:
>  if n == 3:
>      break
>  print(n)
>  n += 1
> else:
>  print("else被执行了")
> ```

#### 3.continue

> 作用：结束当前正在执行的循环，继续下一次循环
>
> ```Python
> #1.continue应用在单循环中
> n = 0
> while n < 10:
>  if n == 3:
>      n += 1
>      continue
>  print(n)
>  n += 1
> 
> #2.continue应用在嵌套循环中
> n = 0
> while n < 3:
>  m = 0
>  while m < 5:
>      if m == 3:
>          m += 1
>          continue
>      print("%d=%d" % (n,m))
>      m += 1
>  n += 1
> ```

#### 4.练习

> ```Python
> import  random
> 
> #练习：模拟猜数字的游戏
> """
> 计算机出一个1~100之间的随机数由人来猜
> 计算机根据人猜的数字分别给出   大一点/小一点/猜中了    的提示
> """
> #获取随机数
> num1 = random.choice(range(1,101))    #80
> 
> #定义一个变量，用于记录猜的次数
> counter = 0
> 
> while True:
>  counter += 1
>  # 引导用户输入数字
>  num2 = int(input("请输入1~100之间的数字"))  #50
> 
>  if num2 >= 1 and num2 <= 100:
>      if num1 > num2:
>          print("大一点")
>      elif num1 < num2:
>          print("小一点")
>      else:
>          print("猜中了")
> 
>          #结束游戏【跳出循环】
>          break
>  else:
>      print("输入的范围有误，正确的范围应该为1~100")
> 
> print("你总共猜了%d次" % (counter))
> if counter > 7:
>  print("你的智商余额不足，请充值")
> ```

# Day4

### 一、上堂回顾

#### 1.默写题目

> 1.求1~100之间能被6整除的数的和
>
> ```Python
> #方式一
> n1 = 1
> total1 = 0
> while n1 <= 100:
> if n1 % 6 == 0:
>  total1 += n1 
> n1 += 1
> 
> #方式二
> n2 = 0
> total2 = 0
> while n2 <= 100:
> total2 += n2
> n2 += 6
> ```
>
> 2.打印九九乘法表
>
> ```Python
> i = 1
> while i <= 9:
>  j = 1
>  while j <= i:
>      
>     print("%dx%d=%d" % (j,i,i * j),end=" ")
>  
>     j += 1
>  print()     
>  i += 1       
> ```

2.知识点回顾

> 1.运算符和表达式
>
> ​	逻辑运算符：and or not     短路原则
>
> ​	 身份运算符：is       is not  地址
>
> ​	 三目运算符
>
> 2.while循环
>
> ​	四要素
>
> ​	break【直接跳出当前循环】和continue【结束当前正在执行的循环，继续下一次循环】

### 二、列表list

#### 1.概念

> 变量：使用变量存储数据，但是，缺点：变量一次只能存储一个数据
>
> 思考问题：如果一次性存储多个数据，该怎么做？
>
> 需求：存储5个人的年龄，求他们的平均年龄
>
> ```Python
> age1 = 10
> age2 = 47
> age3 = 16
> age4 = 19
> age5 = 29
> 
> average = (age1 + age2 + age3 + age4 + age5) / 5
> ```
>
> 解决方案：采用列表
>
> 作用：列表相当于是一个容器，可以同时存储多个数据
>
> 本质：列表是一种有序的集合【有序：数据的存放顺序和内存中的存储顺序是相同的，列表中的数据在内存中的地址是连续的】

#### 2.创建列表

> 说明：列表是一种数据类型，创建列表相当于定义一个列表类型的变量
>
> num = 10
>
> 语法：
>
> ​	列表名  = 列表
>
> ​	列表名= [数据1，数据2，数据3.。。。。]
>
> 说明：
>
> ​	a.列表名是一个合法的标识符即可，但是，不要将列表名称命名为list【系统有一个函数为list】
>
> ​	b.[]是列表的标志
>
> ​	c.列表中的多个数据之间使用逗号隔开，这些数据被称为元素【element】
>
> ​	d.列表中的元素从头到尾被自动进行了编号，编号从0开始，这些编号被称为索引，下标，角标等
>
> ​	e.索引的取值范围：0    ~   元素的个数 - 1 【列表的长度 - 1】 ：从左往右获取
>
> ​					   -1   ~   -元素的个数：从右往左获取
>
> ​		注意：一旦超过索引取值范围，则代码会报错IndexError【索引越界】
>
> ```Python
> #1.创建空列表
> list1 = []
> print(list1)
> print(type(list1))
> 
> #2.创建非空列表
> #注意1:列表是有序的
> #注意2：列表中可以存储重复元素
> list2 = [12,4,34,34,34,54,54]
> print(list2)
> 
> #3.注意:3：在同一个列表中可以存储不同类型的数据
> list3 = [12,"fagg",True,10.43,[4367,43,3]]
> print(list3)
> 
> #4.问题：向列表中存储数据不需要考虑列表的的大小，如果数据量很大的情况下，在进行存储数据的时候，列表的底层会进行自动的扩容
> #工作原理：列表的底层维护了栈，栈是一个线性表，初期理解为一个开口向上的容器，栈的特点：先进后出，后进先出
> #元素的添加和删除都是在表的尾部进行的
> ```

#### 3.元素的访问

> 获取和修改
>
> ```Python
> #元素的访问：通过下标获取元素
> 
> list1 = [11,22,33,44,55]
> 
> 
> #1.获取
> #语法：列表名[索引]
> num1 = list1[2]
> print(num1)
> print(list1[2])
> 
> #注意:索引不能超过范围,索引的取值范围：0~4  或者 -1 ~ -5
> #print(list1[5])   #IndexError: list index out of range
> print(list1[-1])
> print(list1[-2])
> #print(list1[-6])   #IndexError: list index out of range
> print(len(list1))
> 
> #2.修改
> #语法：列表名[索引] = 值
> list1 = [11,22,33,44,55]
> #list1[2]相当于是一个变量名【引用】，指向了33
> print(list1[2])  #33
> print(id(list1))
> 
> list1[2] = 100
> print(list1[2])
> print(list1)
> print(id(list1))
> 
> """
> 总结：
>  a.len(列表名):获取指定列表元素的个数
>  b.索引的取值范围：0~len - 1  或者 -1 ~ -len
>  c.列表是一种可变的数据类型
>  d.列表中存储的数据的地址【列表中存储的是变量】
> """
> ```

#### 4.列表的操作

##### 4.1列表组合

##### 4.2元素的重复

##### 4.3判断元素是否存在

> ```Python
> #1.组合:+
> print(3 + 5)  #数学运算   8
> print("hello" + "world")   #拼接  helloworld
> #print(3 + "hello")   #TypeError: unsupported operand type(s) for +: 'int' and 'str'
> 
> list1 = [1,2,3]
> list2 = [4,5,6]
> print(list1 + list2)
> print(list1)
> print(list2)
> #注意：列表之间可以进行加法运算，表示将两个以上列表中的元素生成一个新的列表，原列表不受任何影响
> 
> #2.列表元素的重复：*
> print("*" * 30)
> print(list1 * 3)
> print(list1)
> 
> #注意：将一个指定列表中的元素重复出现指定的次数，生成了一个新的列表
> 
> #3.判断元素是否存在:成员运算符
> #注意：一般结合if语句
> print(2 in list1)
> print(10 in  list1)
> print(2 not in list1)
> print(10 not in  list1)
> 
> #4.删除列表：del   xxx
> list1 = [3,3,5,45,45]
> print(list1)
> del list1
> print(list1)   #ameError: name 'list1' is not defined
> ```

##### 4.4列表切片【重点掌握】

> ```Python
> #列表的切片：列表的截取，从一个已知的列表中获取一个子列表
> """
> [23,4,4,5,45,454]---->[23,4,45]
> """
> 
> #语法：列表名[start:end:step]
> """
>  start:开始下标
>  end：结束下标
>  step；步长
> 
>  注意：通过开始下标，结束下标和步长共同获取一个列表中的某些特定的元素，生成一个新的子列表
>        start,end和step根据具体额的需求都可以省略
> """
> 
> #获取元素
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[3])
> 
> #1.已知start，省略end和step
> #从start开始，获取到结尾，包含start，step默认为1
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[3:])  #[44, 55, 66, 77, 88]
> 
> #2.已知end，省略了start和step
> #从0开始，获取到end，但是，不包含end
> 
> #在Python中，涉及到区间，包头不包尾
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[:3])  #[11, 22, 33]
> 
> #3.已知start和end，省略step,step默认为1
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[2:5])  #[33, 44, 55]
> 
> #4.已知start、end,step
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[0:7])  #[11,22,33,44,55,66,77]
> print(list1[0:7:1])  #[11,22,33,44,55,66,77]
> print(list1[0:7:2])  #[11,33,55,77]
> 
> 
> #5.获取全部元素
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[:])
> 
> #注意
> print(list1[0:7])   #[11, 22, 33, 44, 55, 66, 77]
> print(list1[0:])   #[11, 22, 33, 44, 55, 66, 77, 88]
> 
> #6.start和end为负数，step为正数
> list1 = [11,22,33,44,55,66,77,88]
> #a.start大于end，结果为[]
> print(list1[-1:-4])
> #b，start小于end，结果从左往右进行获取，同样遵循包头不包尾
> print(list1[-4:-1])  #[55, 66, 77]
> 
> #7.start，end和step为负数
> list1 = [11,22,33,44,55,66,77,88]
> #a。start大于end，结果从右往左进行获取，同样遵循包头不包尾
> print(list1[-1:-4:-1])  #[88,77,66]
> #b.start小于end,结果为[]
> print(list1[-4:-1:-1])  #[]
> 
> #8.start和end为正数，step为负数
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[1:4:-1])  #[]
> print(list1[4:1:-1])  #[55, 44, 33]
> 
> #【面试题】
> #特殊情况一
> list1 = [11,22,33,44,55,66,77,88]
> #print(list1[100])  #IndexError
> print(list1[100:])  #[]
> 
> print(list1[4:100])  #[55, 66, 77, 88]
> print(list1[4:])
> 
> #特殊情况二
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[0:-1])   #[11, 22, 33, 44, 55, 66, 77]
> print(list1[0:7])
> 
> print(list1[0:-1:2])  #[11, 33, 55, 77]
> print(list1[0:7:2])  #[11, 33, 55, 77]
> 
> #特殊情况三
> list1 = [11,22,33,44,55,66,77,88]
> #顺序获取列表中的所有元素
> print(list1[:])  #[11,22,33,44,55,66,77,88]
> #倒序获取列表中的所有元素
> print(list1[::-1])  #[88, 77, 66, 55, 44, 33, 22, 11]
> 
> #特殊情况四
> list1 = [11,22,33,44,55,66,77,88]
> print(list1[0:-1:1])  #[11,22,33,44,55,66,77]
> print(list1[0:-1:-1])  #[]
> 
> 
> #练习：
> list1 = ["a","b","c","d","e","f","g"]
> print(list1[2])   #c
> 
> print(list1[2:])   #c","d","e","f","g"
> print(list1[:2])   #"a","b"
> print(list1[1:4])  #"b","c","d"
> 
> print(list1[1:4:2])   #bd
> print(list1[-1:-4:2])  #[]
> print(list1[-1:-4:-2])  #g e
> 
> print(list1[-4:-1:2])   #d  f
> print(list1[-4:-1:-2])   #[]
> print(list1[0:-1])   #["a","b","c","d","e","f"]
> 
> print(list1[10:])   #[]
> print(list1[1:10])  #"b","c","d","e","f","g"
> print(list1[0:-1:-2])   #[]
> print(list1[::-1])   #全部倒序
> ```

#### 5.列表功能

> ```Python
> #列表功能
> #注意：在列表功能中，增删的操作都是在原列表的基础上直接操作的
> 
> #1.增：append（）
> #在列表的末尾追加元素
> list11 = [11,22,33,44]
> print(list11)
> #追加单个元素
> list11.append(55)
> print(list11)
> 
> #追加多个元素，只能以容器的方式追加
> list11.append([66,77])
> print(list11)
> 
> #2.删：
> #a。 remove(),移除列表中的指定元素
> list2 = [11,22,33,44,22,22,22]
> print(list2)
> #注意：remove从左往右依次进行查找，只删除匹配到的第一个元素
> result = list2.remove(22)
> print(list2)
> print(result)
> # list2.remove(22)
> # print(list2)
> # list2.remove(22)
> # print(list2)
> # list2.remove(22)
> # print(list2)
> 
> #需求：删除[11,22,33,44,22,22,22]列表中的重复元素22
> list1 = [11,22,33,44,22,22,22]
> n = 0
> key = 44
> while n < 4:
>  if key in list1:
>      list1.remove(key)
>  n += 1
> print(list1)
> 
> #注意：当指定的元素在列表中不存在，使用remove函数则会报错ValueError: list.remove(x): x not in list
> 
> #b.clear()
> list1 = [11,22,33,44,22,22,22]
> print(list1)
> list1.clear()
> print(list1)
> 
> #c。pop()：移除列表中指定位置的元素，注意：如果不指明位置，默认删除的是列表中的最后一个元素
> list1 = [11,22,33,44,22,22,22]
> print(list1)
> #注意：pop删除完元素，返回被删除的元素,remove没有任何返回，默认为None【空值】
> r0 = list1.pop()
> print(list1)
> print(r0)
> 
> list1.pop(2)
> print(list1)
> 
> #3.改
> #反转：reverse()
> #方式一:切片；生成了一个新的列表
> list3 = [11,22,33,44,22,22,22]
> print(list3[::-1])
> print(list3)
> #方式二：reverse():修改原列表
> list3 = [11,22,33,44,22,22,22]
> list3.reverse()
> print(list3)
> 
> #排序：sort()
> list3 = [2,43,12,100,45,6]
> print(list3)
> #a。升序
> list3.sort()
> print(list3)
> 
> #b.降序
> #方式一：
> list3 = [2,43,12,100,45,6]
> list3.sort()
> list3.reverse()
> print(list3)
> 
> #方式二：
> list3 = [2,43,12,100,45,6]
> list3.sort(reverse=True)
> print(list3)
> 
> #4.查【获取】
> list3 = [2,43,12,100,45,6,100,12,100]
> #a.len()获取长度
> print(len(list3))
> 
> #b.max()/min() 获取最值
> print(max(list3))
> print(min(list3))
> 
> #c.count():统计一个元素在列表中出现的次数
> print(list3.count(100))
> 
> #d.index():从左往右进行检测，查找一个指定元素在列表中的第一次出现的位置
> index1 = list3.index(100)
> print(index1)
> 
> #print(list3.index(200))     #ValueError: 200 is not in list
> 
> #优化需求：删除[11,22,33,44,22,22,22]列表中的重复元素22
> list1 = [11,22,33,44,22,22,22]
> n = 0
> key = 22
> count1 = list1.count(key)
> while n < count1:
>  if key in list1:
>      list1.remove(key)
>  n += 1
> print(list1)
> ```

#### 6.二维列表

> 实质还是一个一维列表，只不过该列表的元素仍然为一个列表
>
> 举例：
>
> 1根            一个变量
>
> 一包           一维列表【20个变量】
>
> 一条	   二维列表【10个一维列表】
>
> ```Python
> list1 = [[23,43],[1,2,2,3,4],[3]]
> print(list1[1])  #[1,2,2,3,4]
> print(list1[1][0])
> ```

### 三、循环语句-for循环

#### 1.基本用法

> 语法：
>
> while语句：
>
> 初始化表达式
>
> while  条件表达式:
>
> ​	循环体
>
> ​	循环之后的操作表达式
>
> for语句：
>
> for  变量名  in   容器：
>
> ​	循环体
>
> 说明：for循环主要用于遍历可迭代对象【Iterable】或者迭代器【Iterator】
>
> ​    	     遍历：依次访问列表中的每一个元素，获取每个元素值
>
> 工作原理：按照顺序访问容器中的每一个元素，将这些元素赋值给变量名，如此循环往复，直到容器中的元素被获取完毕，循环会自动停止
>
> ```Python
> #1.需求：获取列表中所有的元素
> list1 = [11,22,33]
> #方式一
> # print(list1[0])
> # print(list1[1])
> # print(list1[2])
> 
> #方式二:操作的是索引，通过索引获取元素
> n = 0
> while n < len(list1):
>  print(list1[n])
>  n += 1
> 
> #方式三：直接操作的是元素
> for num in list1:
>  print(num)
> 
> 
> #2.需求：打印列表中下标为偶数的元素
> n = 0
> while n < len(list1):
>  if n % 2 == 0:
>      print(list1[n])
>  n += 1
> 
> 
> for i in range(len(list1)):
>  if i % 2 == 0:
>      print(list1[i])
> 
> ```

#### 2.遍历列表

> ```Python
> #列表的遍历
> 
> list1 = [23,4,34,3,443]
> 
> #方式一:操作的是索引，通过索引获取元素
> n = 0
> while n < len(list1):
>  print(list1[n])
>  n += 1
> 
> #方式二：使用for循环,直接操作的是元素
> for num in list1:
>  print(num)
> 
> #方式三：使用for循环，操作索引
> #range(start,end,step)
> # result = range(100)
> # print(result)
> # print(type(result))
> # l1 = list(result)
> # print(l1)
> # print(type(l1))
> #
> # for i in list(range(len(list1))):
> #     print(i)
> 
> for i in range(len(list1)):
>  print(i,list1[i])
> 
> #方式四：enumerate()，枚举
> # e = enumerate(list1)
> # print(e)
> # print(type(e))
> 
> # for result in e:
> #     print(result)
> 
> for i,num in enumerate(list1):
>  print(i,num)
> 
> # num1,num2,num3 = (10,20,33)
> # print(num1)
> # print(num2)
> # print(num3)
> ```

#### 3.练习

> ```Python
> #练习
> #1.遍历二维列表
> list1 = [[23,43],[1,2,2,3,4],[3]]
> #方式一
> for i in list1:
>  #print(i)
>  for j in i:
>      print(j)
> 
> #方式二
> i = 0
> while i < len(list1):
>  j = 0
>  while j < len(list1[i]):
>      print(list1[i][j])
>      j += 1
>  i += 1
> 
> #2.求1~100之间所有整数的和
> total1 = 0
> for num1 in range(1,101):
>  total1 += num1
> 
> #3.统计100~1000之间能被6整除的数的个数
> count1 = 0
> for num2 in range(100,1000):
>  if num2 % 6 == 0:
>      count1 += 1
> 
> #4.计算1到100以内能被7或者3整除但不能同时被这两者整除的数的个数
> n = 1
> count2 = 0
> while n <= 100:
>  if (n % 7 == 0 or n % 3 == 0) and  not(n % 3 == 0 and n % 7 == 0):
>      count2 += 1
>  n += 1
> 
> n = 1
> count2 = 0
> while n <= 100:
>  if (n % 7 == 0 or n % 3 == 0) and n % 21 != 0:
>      count2 += 1
>  n += 1
> 
> count3 = 0
> for num in range(1,101):
>  if (num % 7 == 0 or num % 3 == 0) and num % 21 != 0:
>      count3 += 1
> 
> #4.打印九九乘法表
> for i in range(1,10):
>  for j in range(1,i + 1):
>      print("%dx%d=%d" % (j,i,i * j),end=" ")
>  print()
> 
> #5.打印图形
> """
> *
> **
> ***
> ****
> *****
> 
>  *
> **
> ***
> ****
> *****
> 
>  *
> ***
> *****
> *******
> *********
> 
> """
> 
> #注意；如果定义的变量在循环体中并未使用，则可以定义为_
> for _ in range(10):
>  print("hello world")
> 
> 
> row = int(input("请输入行数："))
> 
> for i in range(1,row + 1):
>  print("*" * i)
> 
> 
> """
> 行：1 2 3 4 5
> *：1 2 3 4 5    2n - 1
> 空格  4 3 2 1 0    5 - n
> """
> for i in range(1,row + 1):
>  #空格
>  print(" " * (row - i),end="")
>  #*
>  print("*" * i)
> 
> 
> """
> 行：0 1 2 3 4
> *: 1 3 5 7 9
> 空格：4 3 2 1 0
> 
> """
> for i in range(1,row + 1):
>  #空格
>  print(" " * (row - i),end="")
>  #*
>  print("*" * (2 * i - 1))
> ```

# Day5

### 一、上堂回顾

#### 1.默写题目

> 1.使用三目运算符判断一个数是否是偶数
>
> ```Python
> #1.逻辑运算符
> num = 19
> 
> result1 = (num >= 0 and num % 2 == 0) and "偶数" or "奇数"
> 
> #2.if语句
> result2 = "偶数" if (num >= 0 and num % 2 == 0 else "奇数"
> ```
>
> 2.自定义一个非空列表，获取偶数下标对应的元素
>
> ```Python
> list1 = []
> 
> for i in range(len(list1)):
> if i  % 2 == 0:
>  print(list1[i])
>  
> for i,element in enumerate(list1):
> if i % 2 == 0:
>  print(element)
> ```
>
> 3.定义一个非空列表，使用系统功能完成下面操作：
>
> ​	a.获取列表的长度
>
> ​	b.向列表中添加一个任意元素
>
> ​	c.删除列表中的最后一个元素
>
> ​	d.获取某个元素在列表中第一次出现的位置
>
> ```Python
> list1 = [0,1,2,3,3,4,5,3]
> l = len(list1)
> list1.append(67)
> list1.pop()
> list1.index(3)
> ```

#### 2.知识点回顾

> 1.list
>
> ​	增：append
>
> ​	删：pop，remove，clear
>
> ​	改：reverse,sort
>
> ​	查【获取】：len，max，min，index,count
>
> 2.for
>
> ​	一般用于遍历列表

#### 3.作业讲解

> ```Python
> #判断一个数是否是质数
> #假设法：不管该数是否是质数，假设是，寻找合适的条件推翻假设
> 
> #最小的质数就是2
> 
> num = int(input("请输入一个数："))
> 
> #判断num的正负性
> if num <= 1:
>  print("不是质数")
> else:
>  #定义一个变量，用于记录该数是否是质数【bool】
>  flag = True
> 
>  #寻找条件：只要在2~num-1之间找到一个数能将num整除，该数就不是质数
>  for i in range(2,num):
>      if num % i == 0:
>          flag = False
>          #只要得到预期的结果，可以提前结束循环
>          break
> 
>  if flag:
>      print("%d是一个质数")
>  else:
>      print("%d不是一个质数")
> ```

### 二、list列表

#### 1.列表功能

##### 1.1增加

> 增：append，extend,insert
>
> ```Python
> #1.append(),追加
> list1 = [11,22,33,44,55]
> print(list1)
> 
> #追加单个元素
> list1.append(66)
> print(list1)
> 
> #追加多个元素
> #list1.append(77,88)   #TypeError: append() takes exactly one argument (2 given)
> #print(list1)
> list1.append([77,88])
> print(list1)  #[11, 22, 33, 44, 55, 66, [77, 88]]
> 
> 
> #2.extend（），扩展，打碎加入
> list1 = [11,22,33,44,55]
> print(list1)
> 
> #添加单个元素
> # list1.extend(66)    #TypeError:整型不是一个可迭代对象【能用for循环遍历的数据】
> # print(list1)
> list1.extend([66])
> 
> #添加多个元素
> list1.extend([77,88])
> print(list1)
> 
> """"
> 【面试题：简述append和extend之间的区别和联系】
> 相同点：
>  a.都是在列表的末尾添加元素
>  b.添加多个元素，二者都是以容器的方式添加
> 不同点：
>  a.添加单个元素，append可以直接添加，extend只能以容器的方式打碎加入
>  b.当以容器的方式添加元素的时候，append将整个容器作为整体添加进去，extend只添加元素
> """
> 
> #3.insert（索引，被插入的元素），插入
> list1 = [11,22,33,44,55]
> print(list1)
> 
> #插入单个元素
> list1.insert(2,66)
> print(list1)
> 
> #插入多个元素,类似于append，将列表整体插入
> list1.insert(3,[77,88])
> print(list1)
> 
> #注意
> #如果下标超过索引的范围，如果是正数，则默认插入到列表末尾；如果是负数，则默认插入到列表开头
> list1.insert(100,99)
> print(list1)
> list1.insert(-100,99)
> print(list1)
> 
> 
> #需求：删除一个列表中的任意的重复元素
> #1.remove:问题：只能删除指定的重复元素
> list1 = [11,22,22,33,33,11,44,11,55,11,11]
> key = 11
> c = list1.count(key)
> 
> for _  in range(c - 1):
>  if key in list1:
>      list1.remove(key)
> print(list1)
> 
> #2.append
> list1 = [11,22,22,33,33,11,44,11,55,11,11]
> newList = []
> 
> for num in list1:
>  if num not in newList:
>      newList.append(num)
> print(newList)
> 
> 
> # 6.将属于列表l1 = ["Sun","Mon","Tue","Wed","Thu","Fri","Sat"]，但不属于列表l2 = ["Sun","Mon","Thu","Fri","Sat"]的所有元素定义为一个新列表l3
> l1 = ["Sun","Mon","Tue","Wed","Thu","Fri","Sat"]
> l2 = ["Sun","Mon","Thu","Fri","Sat"]
> l3 = []
> for ele in l1:
>  if ele not in l2:
>      l3.append(ele)
> 
> 
> # 7.已知列表namelist=['stu1','stu2','stu3','stu4','stu5','stu6','stu7']，删除列表removelist=['stu3', 'stu7', 'stu9']；请将属于removelist列表中的每个元素从namelist中移除(属于removelist，但不属于namelist的忽略即可)；
> namelist=['stu1','stu2','stu3','stu4','stu5','stu6','stu7']
> removelist=['stu3', 'stu7', 'stu9']
> # for ele in removelist:
> #     if ele in namelist:
> #         namelist.remove(ele)
> # print(namelist)
> 
> for nameele in namelist:
>  for removeele in removelist:
>      if removeele in namelist:
>          namelist.remove(removeele)
> print(namelist)
> 
> # 10.有如下值集合 [11,22,33,44,55,66,77,88,99,90]，对列表里的数据进行奇偶数分离，结果为[[所有偶数]，[所有奇数]]
> list1 = [11,22,33,44,55,66,77,88,99,90]
> 
> #1
> newList = []
> oddList = []
> evenList = []
> 
> for num in list1:
>  if num % 2 == 0:
>      evenList.append(num)
>  else:
>      oddList.append(num)
> newList.append(evenList)
> newList.append(oddList)
> 
> print(newList)
> 
> #2
> oddList = []
> evenList = []
> newList = [oddList,evenList]
> 
> for num in list1:
>  if num % 2 == 0:
>      evenList.append(num)
>  else:
>      oddList.append(num)
> 
> print(newList)
> ```

##### 1.2拷贝【重点掌握】

> 第一种情况：列表拷贝
>
> 第二种情况：copy中copy和deepcopy【深拷贝和浅拷贝】
>
> ```Python
> import  copy
> 
> #一、列表拷贝
> #1.=,变量的赋值
> list1 = [11,22,33]
> list2 = list1
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> list1[2] = 100
> #list1 = [11,22,100]
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> print("*" * 30)
> 
> #2.列表名.copy()
> #2.1一维列表
> list1 = [11,22,33]
> list2 = list1.copy()
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> list1[2] = 100
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> print("*" * 30)
> 
> #2.2二维列表
> list1 = [[11,22,33],[44,55]]
> list2 = list1.copy()
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> list1[1][1] = 100
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> print(id(list1),id(list2))
> 
> 
> """
> 1.引用赋值
>  不管是一维列表还是多维列表，只要一个列表发生改变，另外一个列表也会随着发生改变
> 2.列表中的copy
>  一维列表：一个列表发生改变，另外一个列表不会随着发生改变
>  二维列表：当修改二维列表中的元素，当一个列表发生改变，另外一个列表也会随着发生改变
> """
> 
> """
> [11, 22, 33]
> [11, 22, 33]
> True
> 2025481596680 2025481596680
> [11, 22, 100]
> [11, 22, 100]
> True
> 2025481596680 2025481596680
> ******************************
> [11, 22, 33]
> [11, 22, 33]
> False
> 2025481596616 2025481596872
> [11, 22, 100]
> [11, 22, 33]
> False
> 2025481596616 2025481596872
> ******************************
> [[11, 22, 33], [44, 55]]
> [[11, 22, 33], [44, 55]]
> False
> 2025481609288 2025481596616
> [[11, 22, 33], [44, 100]]
> [[11, 22, 33], [44, 100]]
> False
> 2025481609288 2025481596616
> """
> 
> print("*********深浅拷贝*********")
> 
> #二、深浅拷贝
> #第一步：导入模块import copy
> 
> #1.浅拷贝：copy.copy()
> #a.一维列表
> list1 = [11,22,33]
> list2 = copy.copy(list1)
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> 
> list1[2] = 100
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> 
> print("*" * 30)
> 
> #b。二维列表
> a = [1,2,3]
> b = [4,5,6]
> c = [a,b]
> d = copy.copy(c)
> print(c)
> print(d)
> 
> a.append(100)
> print(c)
> print(d)
> 
> print("~~~~" * 10)
> 
> #2.深拷贝：copy.deepcopy()
> #a.一维列表
> list1 = [11,22,33]
> list2 = copy.deepcopy(list1)
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> 
> list1[2] = 100
> print(list1)
> print(list2)
> print(id(list1) == id(list2))
> 
> print("*" * 30)
> 
> #b。二维列表
> a = [1,2,3]
> b = [4,5,6]
> c = [a,b]
> d = copy.deepcopy(c)
> print(c)
> print(d)
> 
> a.append(100)
> print(c)
> print(d)
> """
> *********深浅拷贝*********
> [11, 22, 33]
> [11, 22, 33]
> False
> [11, 22, 100]
> [11, 22, 33]
> False
> ******************************
> [[1, 2, 3], [4, 5, 6]]
> [[1, 2, 3], [4, 5, 6]]
> [[1, 2, 3, 100], [4, 5, 6]]
> [[1, 2, 3, 100], [4, 5, 6]]
> ​~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
> [11, 22, 33]
> [11, 22, 33]
> False
> [11, 22, 100]
> [11, 22, 33]
> False
> ******************************
> [[1, 2, 3], [4, 5, 6]]
> [[1, 2, 3], [4, 5, 6]]
> [[1, 2, 3, 100], [4, 5, 6]]
> [[1, 2, 3], [4, 5, 6]]
> """
> 
> 
> """
> 1.对于一维列表，copy和deepcopy之后的结果，一个列表发生改变，另外一个列表不受影响
> 2.对于二维列表
>  a.copy:只拷贝最外层，当一个列表的二维列表中的元素发生改变，则另外一个列表也会随着发生改变
>  b.deepcopy:拷贝里外层，当一个列表的二维列表中的元素发生改变，另外一个列表不受影响
> """
> 
> #面试题1：
> a = [1,2,["a","b"]]
> b = a
> c = a.copy()
> a.append(3)
> print(b)   #[1,2,["a","b"],3]
> print(c)   #1,2,["a","b"]]
> 
> a = [1,2,["a","b"]]
> b = a
> c = a.copy()
> a[-1].append(3)
> print(b)  #[1,2,["a","b",3]]
> print(c)  #[1,2,["a","b",3]]
> 
> 
> #面试题2：
> a = [1,2,3]
> b = [4,5,6]
> c = [a,b]
> d = copy.copy(c)
> e = copy.deepcopy(c)
> print(d)   #[[1,2,3],[4,5,6]]
> print(e)   #[[1,2,3],[4,5,6]]
> 
> a[0] = 7
> print(c)    #[[7,2,3],[4,5,6]]
> print(d)   #[[7,2,3],[4,5,6]]
> print(e)    #[[1,2,3],[4,5,6]]
> ```

#### 2.列表的简单算法【重点掌握】

> 需求：求任意一个数字列表中的最大元素
>
> ```Python
> #需求：求任意一个数字列表中的最大元素以及它的位置
> list1 = [23,4,23,100,55,4,23,24]
> 
> #方式一
> maxValue = max(list1)
> print(maxValue)
> 
> #方式二
> #假设法：假设列表中第0个下标对应的元素为最大值，只需要遍历列表，寻找更大的值，给maxValue重新赋值
> maxValue = list1[0]
> for num in list1:
>  if num > maxValue:
>      maxValue = num
> print(maxValue)
> 
> #方式三
> maxValue = list1[0]
> index1 = 0
> for i in range(1,len(list1)):
>  if list1[i] > maxValue:
>      maxValue = list1[i]
>      index1 = i
> print(index1,maxValue)
> 
> 
> #需求：交换两个变量的值
> #方式一:Python特有的语法
> num1 = 10
> num2 = 20
> print(num1,num2)
> num1,num2 = num2,num1
> print(num1,num2)
> 
> #方式二：定义第三者变量
> num1 = 10
> num2 = 20
> print(num1,num2)
> temp = 0
> temp = num1
> num1 = num2
> num2 = temp
> print(num1,num2)
> 
> #方式三：异或^
> num1 = 10
> num2 = 20
> print(num1,num2)
> num1 = num1 ^ num2  #10 ^ 20
> num2 = num1 ^ num2   #10 ^ 20  ^ 20  = 10
> num1 = num1 ^ num2   #10 ^ 20 ^ 10 = 20
> print(num1,num2)
> 
> #方式四：加减法
> num1 = 10
> num2 = 20
> print(num1,num2)
> num1 = num1 + num2   #10 + 20
> num2 = num1 - num2   #10 + 20 - 20 = 10
> num1 = num1 - num2   #10 + 20 - 10 = 20
> print(num1,num2)
> ```

##### 2.1冒泡排序

> 排序思路：比较两个相邻下标对应的元素，如果符合条件则交换位置
>
> ```Python
> #冒泡排序
> 
> #以升序为例
> 
> list1 = [3,5,1000,12,56,100,45,63,453]
> 
> #外层循环：控制比较的轮数
> for i in range(0,len(list1) - 1):
>  #内层循环：控制每一轮参与比较的下标以及比较的次数
>  for j in range(0,len(list1) - i - 1):
>      #如果下标小的元素  大于  下标大的元素，则交换位置
>      #j      j + 1
>      #list1[j]   list1[j + 1]
>      if list1[j] > list1[j + 1]:
>          list1[j],list1[j + 1]  = list1[j + 1], list1[j]
> print(list1)
> 
> """
> 问题：IndexError: list index out of range
> 原因：
>  当i= 0，通过for j in range(0,len(list1) - i)计算，j的取值范围0~4，当j取值为4的时候，j + 1的值为5
> 解决：
>  for j in range(0,len(list1) - i) -----》for j in range(0,len(list1) - i - 1)
> """
> ```

##### 2.2选择排序

> 排序思路：固定一个下标，然后用该下标对应的元素和列表中其他的元素依次比对，如果符合条件则交换位置
>
> ```Python
> #选择排序
> 
> #以升序为例
> 
> list1 = [3,5,1000,12,56,100,45,63,453]
> 
> #外层循环：控制的比较的轮数
> for i in range(0,len(list1) - 1):
>  #内层循环：控制每一轮比较的次数，兼顾参与比较的下标
>  for j in range(i + 1,len(list1)):
>      #如果下标小的元素  大于  下标大的元素，则交换位置
>      #i  j
>      #list1[i]  list1[j]
>      if list1[i] > list1[j]:
>          list1[i],list1[j] = list1[j],list1[i]
> print(list1)
> ```

##### 2.3顺序查找

> 查找思路：遍历指定的列表，把需要查找的元素和列表中的每个元素进行依次的比对，如果相等，则表示查找成功
>
> ```Python
> #顺序查找
> 
> list1 = [23,54,65,65,2,56,76,7]
> 
> key = 65
> 
> #方式一
> print(list1.index(key))  #第一次
> 
> #方式二
> for i in range(len(list1)):
>  if key == list1[i]:
>      print(i)
>      #break
> ```

##### 2.4二分法查找

> 前提【缺陷】：列表是有序的
>
> 查找思路：通过折半缩小查找范围，提高工作效率【将待查找的元素和有序列表中间下标对应的元素进行比较，以升序为例，如果带查找元素大于中间下标对应的元素，则确定该元素在后半段】
>
> ```Python
> list1 = [3,54,545,65,465,1,23,4324]
> 
> key = 23
> 
> #1.保证被查找的列表式有序的【升序】
> list1.sort()
> 
> #2.定义变量
> left = 0
> right = len(list1) - 1
> 
> #3.查找的条件；当left == right还未找到，则说明被查找元素不存在
> while left <= right:
>  #4.计算中间的下标
>  middle = (left + right) // 2
> 
>  #5.比较待查找元素和中间下标对应元素的大小
>  if key > list1[middle]:
>      #更改区间
>      left = middle + 1
>  elif key < list1[middle]:
>      right = middle - 1
>  else:
>      print("%s元素的位置为：%d" % (key,middle))
>      #退出循环
>      break
> 
> """
> 总结：
>  a.必须有序
>  b.列表升序和降序的代码有所区别
>  c.最后查找的是在排序后的列表中的位置
>  d.如果查找到，只能获取一个位置【考虑到重复元素】
> """
> ```

### 三、tuple元组

#### 1.概念

> 和列表类似，元组也是一个有序的集合
>
> 元组和列表的不同之处：
>
> ​	a.定义，列表：[],元组：()
>
> ​	b.列表是一种可变的数据类型【可以增加或者删除或者更改元素】，元组是一种不可变的数据类型【一旦定义好一个元组，该元组内部的元素将不能再发生任何的改变】

#### 2.创建元组

> ```Python
> #创建列表
> list1 = []
> list1 = [43,5,54]
> 
> #创建元组
> tuple1 = ()
> tuple2 = (43,5,54)
> print(tuple1,tuple2)
> print(type(tuple1))
> 
> #注意问题
> #a.和列表相同，元组中允许存储重复元素
> #b.和列表相同，元组的元素是有序的
> t1 = (11,11,22,33,22,22)
> print(t1)
> 
> #c.和列表相同，元组中也可以存储不同类型的数据
> t2 = (324,"fsg",True,10.33)
> print(t2)
> 
> #d，如果元组中只有一个元素，需要在袁术的后面添加一个逗号，消除歧义
> l1 = [10]
> print(type(l1))  #<class 'list'>
> #t1 = ("fag")  #等价于t1 = "fag"
> #print(type(t1))  #<class 'str'>
> 
> t1 = (10,)
> print(type(t1))  #<class 'tuple'>
> ```

#### 3.元素的访问

> 获取
>
> 修改
>
> ```Python
> #元素的访问
> 
> #1.获取
> #和列表相同，元组名[下标或者索引]
> tuple1 = (3,3,4,34,34,34,100)
> num1 = tuple1[4]
> print(num1)
> print(tuple1[-1])
> 
> 
> #2.修改
> tuple1 = (3,3,4,34,34,34,100)
> print(tuple1)
> # tuple1[1] = 18
> # print(tuple1)  #TypeError: 'tuple' object does not support item选项 assignment赋值
> 
> #特殊情况：如果一个元组中的元素为列表，可以任意更改列表中的元素
> tuple2 = (23,4,3,4,[4,4,4])
> print(tuple2)
> tuple2[-1][0] = 100
> print(tuple2)
> 
> #3.遍历元组
> #下标的取值范围：0~ len - 1  或者  -1 ~ - len
> 
> tuple1 = (3,3,4,34,34,34,100)
> #方式一
> i = 0
> while i < len(tuple1):
>  print(i,tuple1[i])
>  i += 1
> 
> #方式二
> for num in tuple1:
>  print(num)
> 
> #方式三
> for i in range(len(tuple1)):
>  print(i,tuple1[i])
> 
> #方式四
> for i,ele in enumerate(tuple1):
>  print(i,ele)
> 
> ```

#### 4.元组操作

> ```Python
> #元组操作
> #1.组合：+
> t1 = (1,2,3)
> t2 = (4,5,6)
> print(t1 + t2)
> print(t1)
> 
> #2.元素重复:*
> print(t1 * 3)
> 
> #3.判断元素是否存在
> print(2 in t1)  #True
> print(10 in t1)  #False
> 
> #4.切片
> list1 = ("a","b","c","d","e","f","g")
> print(list1[2])   #c
> 
> print(list1[2:])   #c","d","e","f","g"
> print(list1[:2])   #"a","b"
> print(list1[1:4])  #"b","c","d"
> 
> print(list1[1:4:2])   #bd
> print(list1[-1:-4:2])  #[]
> print(list1[-1:-4:-2])  #g e
> 
> print(list1[-4:-1:2])   #d  f
> print(list1[-4:-1:-2])   #[]
> print(list1[0:-1])   #["a","b","c","d","e","f"]
> 
> print(list1[10:])   #[]
> print(list1[1:10])  #"b","c","d","e","f","g"
> print(list1[0:-1:-2])   #[]
> print(list1[::-1])   #全部倒序
> 
> ```

#### 5.元组功能

> ```Python
> #元组的功能
> t1 = (23,4,3,45,4,5,4,100,54,5)
> #1.len
> print(len(t1))
> 
> #2.count
> print(t1.count(5))
> 
> #3.max、min
> print(max(t1))
> 
> #4.删除
> #del t1
> 
> #5.list(),tuple()
> #a。list将元组转化为列表
> print(type(t1))
> l1 = list(t1)
> print(type(l1))
> 
> #b.tuple将列表转化为元组
> t2 = tuple(l1)
> print(type(t2))
> 
> #注意：定义list或者tuple的时候，变量的命名不要使用list或者tuple
> # list = [23,43,4]
> # l1 = list(t1)
> # print(type(l1))
> 
> 
> 
> 
> ```

#### 6.二维元组

> ```Python
> #二维列表
> list1 = [[3,5,54,54],[54,54,5,4]]
> 
> for subList in list1:
>  for num in subList:
>      print(num)
> 
> #二维元组
> tuple1 = ((3,5,54,54),(54,54,5,4))
> 
> for subTuple in tuple1:
>  for num in subTuple:
>      print(num)
> 
> ```

> 1.元组中的元素是无法改变，涉及到多线程，如果使用可变数据，多个线程同时访问该数据，最后会导致该数据的结果发生混乱【不可变的数据比可变的数据更加易于维护】，如果需要对元素进行更改，则选用列表；如果希望数据永远不可变，则选用元组
>
> 2.元组在创建时间上和内存占用都优于列表

# Day6

### 一、上堂回顾

#### 1.默写题目

> 1.定义把一个非空数字列表，使用冒泡排序进行降序排序
>
> ```Python
> numList = []
> 
> #外层循环：控制比较的轮数
> for i in range(len(numList) - 1):
> #内层循环：控制每一轮比较的次数，同时兼顾参与比较的下标
> for j in range(len(numList) - i - 1):
>  #比较
>  if numList[j] < numList[j + 1]:
>    numList[j],numList[j + 1] = numList[j + 1],numList[j]
>    
> ```
>
> 2.定义一个非空元组，至少用两种方式遍历出其中的元素
>
> ```Python
> t1 = ()
> for ele in t1:
> print(ele)
> 
> for i in range(len(t1)):
> print(t1[i])
> 
> ```
>
> 3.使用至少两种方式交换两个变量的值
>
> ```Python
> num1 = 10
> num2 = 20
> num1,num2 = num2,num1
> 
> num3 = num1
> num1 = num2
> num2 = num3
> ```

#### 2.知识点回顾

> 1.list
>
> ​	a.append和extend之间的区别
>
> ​	b.拷贝
>
> ​		1》=和copy【实际开发】
>
> ​		2》copy模块中的copy和deepcopy【深浅拷贝，面试题】
>
> ​	c.简单算法
>
> ​		冒泡排序
>
> ​		选择排序
>
> ​		二分法查找【掌握思路】
>
> 2.tuple
>
> ​	注意：tuple的元组被定义完成之后将不能再修改

#### 3.作业讲解

> ```Python
> #需求：求一个数字列表中的第二大值以及它的位置
> 
> numList = [23,4,100,35,46,56,100,354,3,54,5,4,354,354]
> 
> #1.拷贝
> newList = numList.copy()
> 
> #2.对新列表进行升序排序
> # 外层循环：控制比较的轮数
> for i in range(len(numList) - 1):
>  # 内层循环：控制每一轮比较的次数，同时兼顾参与比较的下标
>  for j in range(len(numList) - i - 1):
>      # 比较
>      if numList[j] > numList[j + 1]:
>          numList[j], numList[j + 1] = numList[j + 1], numList[j]
> print(numList)
> 
> #3.获取最大值以及统计最大值的个数
> maxValue = numList[-1]
> maxCount = numList.count(maxValue)
> print(maxValue,maxCount)
> 
> #4.获取第二大值
> secondValue = numList[-(maxCount + 1)]
> print(secondValue)
> 
> #5.顺序查找
> for i in range(len(newList)):
>  if secondValue == newList[i]:
>      print(i)
> ```

### 二、布尔值和空值

> 布尔值：True和False相当于1和0，可以和数字类型的变量进行运算符
>
> ​	        主要用于if语句和while语句中
>
> 空值：None
>
> ```Python
> #1.bool类型
> b1 = True
> b2 = False
> print(b1,b2)
> 
> #2.可以运算
> print(10 + True)
> print(10 + False)
> 
> #3.结合逻辑运算符,根据真假判断
> print(3 and 5)  #5
> print(3 or 5)  #3
> 
> print(0 and 9)   #0
> print(0 or 9)   #9
> 
> print(4 and 0)  #0
> print(4 or  0)  #4
> 
> #4.
> #逻辑运算符
> print(True and False)
> #成员运算符
> print(10 in [3,4,343])
> #关系运算符
> print(10 > 36)
> #身份运算符
> print(10 is 20)
> 
> 
> #5.空值
> result = None
> print(type(result))   #<class 'NoneType'>
> #使用场景：当一个引用没有指向的之后，默认指向None
> 
> 
> #举例
> #1
> list1 = [34,5,45,65,4]
> r0 = list1.pop()
> print(r0)
> 
> r1 = list1.remove(5)
> print(r1)
> 
> 
> #2
> def test():
>  #pass
>  return
> print(test())
> ```

### 三、number数字型

#### 1.分类

> ```Python
> #整型
> num1 = 10
> print(type(num1))  #<class 'int'>
> 
> #浮点型
> num2 = 10.345
> print(type(num2)) #<class 'float'>
> 
> #复数
> #a。a + bj
> num3 = 3 + 5j
> print(type(num3))  #<class 'complex'>
> #b。complex(a,b)
> num4 = complex(4,5)
> print(type(num4))
> ```

#### 2.类型转换

> ```Python
> #int(x,base=10)
> 
> #int("110afag")   #ValueError: invalid literal for int() with base 10: '110afag'
> 
> #1
> r0 = int("110")
> print(r0,type(r0))   #110
> 
> r0 = int("110",base=10)
> print(r0,type(r0))
> 
> r0 = int("110",10)
> print(r0,type(r0))
> 
> #2
> #base是为了标记当前的数据是几进制，int(xx)将数据转化为十进制
> r0 = int("110",base=2)
> print(r0,type(r0))
> r0 = int("110",2)
> print(r0,type(r0))
> 
> r0 = int("110",base=8)
> print(r0,type(r0))
> ```

#### 3.系统功能

##### 3.1数学功能

> ```Python
> import  math
> 
> #一、系统功能【内置功能】
> #1.绝对值
> a1 = -19
> print(abs(a1))
> 
> #2.求最值
> print(max([23,5,45,454]))
> print(min([23,5,45,454]))
> 
> print(max(23,5,45,454))
> print(min(23,5,45,454))
> 
> print(max((23,5,45,454)))
> print(min((23,5,45,454)))
> 
> print(max("fhf","zy","abc"))
> 
> #3.求幂
> print(pow(4,2))
> 
> #4.求一个浮点数的四舍五入值
> #注意1：默认返回一个整数
> print(round(10.2343))
> print(round(10.6343))
> #注意2：如果指明第二个参数，则表示保留浮点数小数点后几位
> print(round(10.2343,2))
> print(round(10.6353,2))
> 
> #5.求和
> #注意：sum可以对序列【可迭代对象】中的元素求和
> print(sum([1,2,3]))
> #print(sum(["a","b","c"]))  #TypeError: unsupported operand type(s) for +: 'int' and 'str'
> 
> print(sum((1,2,3)))
> print(sum((1,2,3),1))  #元组的元素和加1
> 
> print(sum([1,2,3]))
> print(sum([1,2,3],4))  #列表的元素和加4
> 
> #需求：求1~100之间整数的和
> print(sum(range(1,101)))
> 
> #6，比较
> num1 = 6
> num2 = 9
> print((num1 - num2) > 0)
> #if语句
> 
> #二、math模块
> #1.向上取整
> #注意：向上或者向下取整和四舍五入的区别
> print(math.ceil(18.39))
> print(math.ceil(18.99))
> 
> #2.向下取整
> print(math.floor(18.39))
> print(math.floor(18.99))
> 
> #3.求算术平方根，结果为浮点数
> print(math.sqrt(9))
> 
> #4.获取一个浮点数的小数部分和整数部分，结果为一个元组（小数部分，整数部分）
> print(math.modf(10.45))   #(0.23000000000000043, 10.0)
> 
> #5.数学常量
> #圆周率
> print(math.pi)
> #自然常数
> print(math.e)
> ```

##### 3.2随机数功能

> ```Python
> #import  random
> #从random模块中导入所有内容
> from random import  *
> 
> #1.choice(xx)
> #注意：xx只能是可迭代对象
> #a.列表
> num1 = choice([23,43,43,4343])
> print(num1)
> 
> #b.range(start,end,step)
> num2 = choice(range(5))
> print(num2)
> 
> #c.元组
> num3 = choice((23,43,43,4343))
> print(num3)
> 
> #d.字符串
> num4 = choice("hfjakef")   #"hfjakef" ----->("h",'f','j'.....)
> print(num4)
> 
> #需求：产生一个4~10之间的任意整数随机数
> print(choice(range(4,11)))
> 
> #2.randint()
> """
> choice(range(start,end,step)),end不包含,step可以是任意的整数，表示步长
> randint(start,end),end包含，没有step参数
> """
> 
> #3.randrange()
> """
> choice(range(start,end,step))
> randint(start,end)
> randrange(start,end,step)
> """
> 
> #需求：求1~100之间的整数随机数
> print(choice(range(1,101)))
> print(randint(1,100))
> print(randrange(1,101))
> 
> #注意：在Python中，一旦涉及到step，都只能是整型
> #print(randrange(1,101,0.5))  #ValueError: non-integer step for randrange()
> 
> 
> #4.random()
> #获取0~1之间的浮点数随机数
> print(random())
> print(round(random(),2))
> 
> #需求：求4~10之间的任意的随机数
> """
> 0~1 * 6 ---->0~6
> 0~4 + 4 ----->4~10
> """
> print(random() * 6 + 4)
> 
> #需求：求20~100之间的任意的随机数
> print(random() * 80 + 20)
> 
> #5.uniform()
> #uniform(start,end),获取start到end之间的任意的随机数【包含整数和浮点数】
> print(uniform(20,101))
> 
> #6.shuffle(),对序列中 元素进行随机排序
> list1 = [11,22,33,44]
> print(list1)
> shuffle(list1)
> print(list1)
> 
> 
> #练习：编写程序，生成一个长度为10的列表，列表中的元素为1~100之间的随机数
> list1 = []
> for _ in range(10):
>  #list1.append(randint(1,100))
>  list1.append(round(uniform(1,100),3))
> print(list1)
> 
> ```

##### 3.3三角函数

> ```Python
> import  math
> 
> #将角度转化为弧度
> print(math.radians(90))
> #将弧度转化为角度
> print(math.degrees(math.pi / 2))
> 
> 
> print(math.sin(math.radians(90)))
> print(math.cos(math.radians(90)))
> 
> print(math.asin(math.radians(90)))
> 
> ```

### 四、dict字典

#### 1.概念

> 思考问题：保存5个人的年龄，方便后期的查找，单纯使用列表和元组存储，数据容易发生混乱
>
> 解决方案：使用字典【将人的姓名作为key，将人的年龄作为value】
>
> 也是一种存储数据的方式，但是字典是无序的，其中存储的数据是键-值对
>
> 作用：具有极快的查找速度
>
> key的特点：
>
> ​	a.字典中的key必须是唯一的
>
> ​	b.key必须是不可变的数据类型
>
> ​		list是可变的，不可以充当key
>
> ​		tuple，整型，字符串，对象等都可以充当key

#### 2.创建

> ```Python
> #语法：字典名  = {键1：值1，键2：值2.。。。。。}
> 
> #一个字典中键值对的个数就是该字典的长度
> 
> #1.创建空字典
> dict1 = {}
> print(dict1)
> 
> 
> #2.创建非空字典
> #注意：字典是一种无序的集合
> dict2 = {"zhangsan":19,"jack":10}
> print(dict2)
> 
> 
> #3.key不能是list
> #dict3 = {[1,2]:10,[34,5]:20}
> #print(dict3)   #TypeError: unhashable type: 'list'  哈希
> 
> #4.比较下来，字典更加占用内存空间
> list1 = ["zhangsan","jack"]
> list2 = [19,10
> 
> ```

#### 3.键值对的访问

> 获取
>
> 添加
>
> 删除
>
> ```Python
> #在字典中，通过key操作value，key相当于list或者tuple的索引
> 
> dict1 = {"zhangsan":19,"jack":10,"bob":13}
> 
> #1.获取
> #a.字典名[key]
> age1 = dict1["jack"]
> print(age1)
> 
> #如果一个key不存在，会报错
> #print(dict1["lisi"])  #KeyError: 'lisi'
> 
> #b.get()
> age2 = dict1.get("jack")
> print(age2)
> 
> result = dict1.get("lisi")
> print(result)
> if result == None:
>  print("key不存在")
> else:
>  print("key存在的")
> 
> #2.添加
> dict1 = {"zhangsan":19,"jack":10,"bob":13}
> print(dict1)
> #a。如果key存在，字典名[key] = 值 则表示修改指定key的value
> dict1["bob"] = 20
> print(dict1)
> 
> #b.如果key不存在，字典名[key] = 值 则表示向字典中添加键值对
> dict1["rose"] = 18
> print(dict1)
> 
> #3.删除
> #a.pop
> dict1.pop("jack")
> print(dict1)
> 
> #b。del
> del dict1["zhangsan"]
> print(dict1)
> 
> #c。clear
> dict1.clear()
> print(dict1)
> 
> #结论：dict和list相同，都是可变的数据类型
> 
> ```

#### 4.遍历

> ```Python
> #字典的功能
> dict1 = {1:10,2:20,3:30}
> 
> #获取字典中的键值对的总数
> print(len(dict1))
> 
> #获取字典中的所有的key
> r0 = dict1.keys()
> print(r0,type(r0))
> print(list(r0))
> 
> #获取字典中所有的value
> r0 = dict1.values()
> print(r0,type(r0))
> print(list(r0))
> 
> #获取字典中的所有的key和value的映射关系，
> r0 = dict1.items()
> print(r0,type(r0))  #dict_items([(1, 10), (2, 20), (3, 30)]) <class 'dict_items'>
> print(list(r0))  #[(1, 10), (2, 20), (3, 30)]
> 
> 
> #字典的遍历
> dict1 = {"zhangsan":19,"jack":10,"bob":13}
> #1.获取key[******]
> for key in dict1:
>  print(key,dict1[key])
> 
> #2.获取key
> for key in dict1.keys():
>  print(key,dict1[key])
> 
> #3.获取value[****]
> for value in dict1.values():
>  print(value)
> 
> #4.获取key
> for i,key in enumerate(dict1):
>  print(i,key,dict1[key])
> 
> #5.获取key和value的映射关系[******]
> for key,value in dict1.items():
>  print(key,value)
> 
> ```

#### 5.练习

> ```Python
> """
> 1.已知字典dict1 = {"k1":"v1","k2":"v2","k3":"v3"},完成下面操作
>  a.循环遍历出所有key
>  b.循环遍历出所有的value
>  c.在字典中添加一对新的键值对"k4":"v4"
>  d.删除字典中的键值对"k1":"v1"
>  e.获取"k2"对应的值
>  f.生成一个新的字典，{"v1":"k1","v2":"k2","v3":"k3"}
> """
> dict1 = {"k1":"v1","k2":"v2","k3":"v3"}
> for key in dict1:
>  print(key)
> for value in dict1.values():
>  print(value)
> if  "k3" not in dict1:
>  dict1["k4"] = "v4"
> 
> if "k1" in dict1:
>  dict1.pop("k1")
> 
> #e
> if "k2" in dict1:
>  v2 = dict1["k2"]
> v2 = dict1.get("k2")
> if v2 == None:
>  print("不存在")
> else:
>  print(v2)
> 
> #f
> dict2 = {}
> for key,value in dict1.items():
>  dict2[value] = key
> print(dict2)
> 
> #2.已知列表list1 = [11,22,33,44,55,66],将其进行奇偶数分离，结果为一个字典{"偶数":[],"奇数":[]}
> list1 = [11,22,33,44,55,66]
> evenList = []
> oddList = []
> 
> for num in list1:
>  if num % 2 == 0:
>      evenList.append(num)
>  else:
>      oddList.append(num)
> 
> newDict = {"偶数":evenList,"奇数":oddList}
> print(newDict)
> 
> #3.已知列表list1 = [0,1,2,3,4],list2 = ['a','b','c','d','e'],生成字典{0:'a',1:"b".....}
> list1 = [0,1,2,3,4]
> list2 = ['a','b','c','d','e']
> newDict = {}
> 
> for i in range(len(list1)):
>  #list1[i]:key   list2[i] :value
>  newDict[list1[i]] = list2[i]
> print(newDict)
> 
> #优化：一般化，如果列表的长度不一致
> if len(list1) <= len(list2):
>  for i in range(len(list1)):
>      newDict[list1[i]] = list2[i]
> else:
>  for i in range(len(list2)):
>      newDict[list1[i]] = list2[i]
> 
> #4.从控制台输入一个字符串，统计其中每个字符出现的次数
> #hello---->{"h":1,"e":1,"l":2,"o":1}
> str1 = input("请输入任意的文本：")
> dict1 = {}
> 
> #思路：将字符作为key，次数作为value生成一个字典，首先判断字符在字典中是否存在，如果不存在，则添加键值对，如果存在，则给value递增1
> for ch in str1:
>  if ch not in dict1:
>      dict1[ch] = 1
>  else:
>      dict1[ch] += 1
> print(dict1)
> ```

### 五、set集合

#### 1.概念

> list:[]
>
> tuple:()
>
> dict:{}
>
> set:{}
>
> set和dict比较，相当于在集合中存储了字典中的所有的key
>
> 本质：一个无序且没有重复元素的集合

#### 2.创建set

> ```Python
> #创建set
> #1.注意：如果书写一个空的{}，默认表示字典
> dict1 = {}
> print(type(dict1))
> 
> #2
> s1 = {12,34,5435}
> print(s1,type(s1))
> 
> #3.list(),tuple(),dict(),set()
> s1 = set()  #创建空集合
> print(s1,type(s1))
> 
> #无序，不允许重复元素出现
> s1 = set([3,43,43])
> print(s1,type(s1))
> 
> s1 = set((3,43,43))
> print(s1,type(s1))
> 
> #注意：如果通过字典创建集合，只获取字典中所有的key
> s1 = set({12:1,2:4})
> print(s1,type(s1))
> ```

#### 3.使用

> 添加，删除，遍历，交集和并集
>
> ```Python
> #1.添加
> #add(),添加，
> s1 = {11,22,33,44}
> print(s1)
> #a.添加单个元素
> # s1.add(55)
> # print(s1)
> 
> #b.添加多个元素
> # s1.add([66,77])
> # print(s1)
> 
> # s1.add((66,77))
> # print(s1)
> 
> # s1.add({66:1,77:2})
> # print(s1)
> 
> #结论：add只能支持不可变的数据类型，list和dict都是可变的，add不能识别
> 
> #向集合中添加一个已经存在的元素【排重的】，不会报错
> s1.add(22)
> print(s1)
> 
> print("*" * 30)
> 
> #update()，更新
> s1 = {11,22,33,44}
> print(s1)
> 
> #a。添加单个元素
> #s1.update(55)   #TypeError: 'int' object is not iterable可迭代对象
> #print(s1)
> 
> s1.update("fahjg")
> print(s1)
> 
> s1.update([23,4,43])
> print(s1)
> 
> s1.update((100,200))
> print(s1)
> 
> s1.update({88:99})
> print(s1)
> 
> #结论：update只能识别可迭代对象【str，list,tuple,dict】
> 
> #2.删除：remove
> s1 = {11,22,33,44}
> print(s1)
> s1.remove(22)
> print(s1)
> 
> # list1 = [3,5,45,4]
> # del list1[1]
> 
> #3.遍历
> for i in s1:
>  print(i)
> 
> for i,num in enumerate(s1):
>  print(i,num)
> 
> #4.交集和并集
> s1 = {1,2,3,4}
> s2 = {3,4,5,6}
> 
> #交集：&【按位与】
> print(s1 & s2)    #{3,4}
> 
> #并集：|【按位或】
> print(s1 | s2) #{1,2,3,4,5,6}
> ```

# Day7

### 一、上堂回顾

#### 1.默写题目

> 1.使用不同方式实现去除一个非空列表中的重复元素
>
> ```Python
> list1 = [13,3,3,43,43]
> 
> #方式一
> set1 = set(list1)
> list2 = list(set1)
> 
> #方式二
> list2 = []
> for ele in list1:
> if ele not in list2:
>  list2.append(ele)
> ```
>
> 2.简述dict和set之间的区别和联系
>
> ```Python
> """
> 相同点：
> 	a.都是用来存储不同类型数据的容器
> 	b.都是无序的
> 	c.dict中的key是唯一的，set中的元素也是唯一的
> 	d.dict和set都是可变的数据类型，都可以增加，删除或者修改元素
> 不同点：
> 	a.dict中相当存储了一个集合【key】和一个列表【value】，从内存角度上分析，dict相当于占用了两份内存
> 	b.set中存储单个数据，dict中存储键值对
> 联系：
> 	a.set中的元素相当于存储了dict中的key
> 	b.二者之间可以通过dict（），set()实现转化
> """
> ```
>
> 3.自定义一个非空数字列表，使用选择排序实现降序排序
>
> ```Python
> list1 = []
> 
> for i in range(len(list1) - 1):
> for j in range(i + 1,len(list1)):
>  if list1[i] < list1[j]:
>    list1[i],list1[j]  = list1[j],list1[i]
> ```

2.知识点回顾

> 1.列表和字典
>
> ​	列表：常用功能
>
> ​	字典：遍历【键值对的添加】
>
> 2.总结
>
> ​	可变的数据类型：list,dict,set
>
> ​	不可变的数据类型：number,string,bool,tuple
>
> ​	可以使用for循环遍历的数据类型【可迭代对象】：list,dict,set，string,tuple

### 二、string字符串

#### 1.创建

> ```Python
> #字符串的定义
> 
> #1.单引号
> str1 = 'hello'
> print(str1)
> 
> #2.双引号
> str2 = "hello"
> print(str2)
> 
> #3.三引号
> str3 = """hello"""
> print(str3)
> 
> #检测他们的内存地址
> #注意1：不管使用哪种形式表示字符串，只要数据相同，则他们的地址也相同
> print(str1 == str2)
> print(str1 is str2)
> print(id(str1) == id(str2))
> 
> print(str1 == str3)
> print(str1 is str3)
> print(id(str1) == id(str3))
> 
> #4.三引号的特点
> #需求：在字符串的内部进行换行
> str1 = 'hello\nworld\naaa\nbbb'
> print(str1)
> 
> str2 = "hello\nworld\naaa\nbbb"
> print(str2)
> 
> #注意2：三引号不需要使用\n进行换行，按下回车键就可以实现换行，也可以将其中的内容原样输出
> str3 = """hello
>  world
>  aaa
>  bbb
>  ccc
> """
> print(str3)
> 
> 
> #5.字符串的组成
> #可以由数字，字母，特殊符号以及中文
> str1 = "23ab&%测试_"
> print(str1)
> 
> 
> #6.一旦字符串中出现特殊字符，可能需要转义
> #转义：使用\修改后面的字母或者符号的含义【特殊字符----》普通字符   普通字符-----》特殊字符】
> #普通字符-----》特殊字符
> str1 = "\n"
> print(str1)
> 
> #需求：打印"hello"
> #特殊字符----》普通字符
> print("hello")
> print("\"hello\"")
> 
> 
> #7.如果一个字符串中有多个字符需要被转义，则可以使用r"xxxxx"
> #r"xxxxx"一般使用在路径和正则表达式
> path1 = "C:\\Users\\Administrator\\Desktop\\XA-Python1904\\Day7"
> print(path1)
> 
> path2 = r"C:\Users\Administrator\Desktop\XA-Python1904\Day7"
> print(path2)
> 
> """
> 常用的转义字符
> \n：换行
> \t:tab键
> \r:回车键
> """#字符串的定义
> 
> #1.单引号
> str1 = 'hello'
> print(str1)
> 
> #2.双引号
> str2 = "hello"
> print(str2)
> 
> #3.三引号
> str3 = """hello"""
> print(str3)
> 
> #检测他们的内存地址
> #注意1：不管使用哪种形式表示字符串，只要数据相同，则他们的地址也相同
> print(str1 == str2)
> print(str1 is str2)
> print(id(str1) == id(str2))
> 
> print(str1 == str3)
> print(str1 is str3)
> print(id(str1) == id(str3))
> 
> #4.三引号的特点
> #需求：在字符串的内部进行换行
> str1 = 'hello\nworld\naaa\nbbb'
> print(str1)
> 
> str2 = "hello\nworld\naaa\nbbb"
> print(str2)
> 
> #注意2：三引号不需要使用\n进行换行，按下回车键就可以实现换行，也可以将其中的内容原样输出
> str3 = """hello
>  world
>  aaa
>  bbb
>  ccc
> """
> print(str3)
> 
> 
> #5.字符串的组成
> #可以由数字，字母，特殊符号以及中文
> str1 = "23ab&%测试_"
> print(str1)
> 
> 
> #6.一旦字符串中出现特殊字符，可能需要转义
> #转义：使用\修改后面的字母或者符号的含义【特殊字符----》普通字符   普通字符-----》特殊字符】
> #普通字符-----》特殊字符
> str1 = "\n"
> print(str1)
> 
> #需求：打印"hello"
> #特殊字符----》普通字符
> print("hello")
> print("\"hello\"")
> 
> 
> #7.如果一个字符串中有多个字符需要被转义，则可以使用r"xxxxx"
> #r"xxxxx"一般使用在路径和正则表达式
> path1 = "C:\\Users\\Administrator\\Desktop\\XA-Python1904\\Day7"
> print(path1)
> 
> path2 = r"C:\Users\Administrator\Desktop\XA-Python1904\Day7"
> print(path2)
> 
> """
> 常用的转义字符
> \n：换行
> \t:tab键
> \r:回车键
> """
> ```

#### 2.操作

> ```Python
> #1.连接【拼接】：+
> str1 = "hello"
> str2 = "Python"
> print(str1 + str2)
> print(str1)
> 
> #结论：字符串的底层其实维护了一个字符元组，所以字符串也是不可变的数据类型
> # 【以后但凡涉及到字符串的更改，都是生成了一个新的字符串】
> 
> #2.重复字符串：*
> print("*" * 30)
> print("abc" * 3)
> 
> #3.获取字符串中的字符
> #和列表以及 元组相同，字符串也是有索引的，通过索引获取字符
> str3 = "1234abcd"
> print(str3[2])
> 
> #4.判断子字符串在原字符串中是否存在
> #注意：子字符串在原字符串中是连续存在的，则返回True
> print("12" in str3)
> print("ad" in str3)
> 
> #5.切片
> s1 = "123456abcdef"   #0~11
> print(s1[2])
> print(s1[2:])
> print(s1[:2])
> print(s1[2:7:2])
> print(s1[-2:-7])   #""
> print(s1[-2:-7:-1])
> print(s1[0:-1])
> print(s1[12:])
> print(s1[:12])
> ```

#### 3.功能

##### 3.1转换

> ​	eval()：将str转换为有效的表达式
>
> ​	upper():将小写字母转换为大写
>
> ​	lower():大---》小
>
> ​	swapcase():大---》小  小----》大
>
> ​	capitalize():首单词的首字母大写，其他全部小写
>
> ​	title():每个单词的首字母大写，其他全部小写
>
> ​	ord(),chr()

##### 3.2查找

> ​	find():从左往右进行检索，返回被查找的子字符串在原字符串中第一次出现的位置，如果查找不到返回-1
>
> ​	rfind():从右往左进行检索
>
> ​	index()：从左往右进行检索，返回被查找的子字符串在原字符串中第一次出现的位置，如果查找不到则直接报错
>
> ​	rindex():从右往左进行检索

##### 3.3填充和提取

> ​	center(width[,fillchar]):用fillchar填充指定的字符串，填充之后的长度为width,原字符串居中显示，举例：
>
> ```Python
> str1 = "hello"
> str2 = str1.center(20)
> print(str2)  #          hello          
> str2 = str1.center(20,"*")
> print(str2)  #*******hello*******
> ```
>
> ​	ljust(width[,fillchar]):用fillchar填充指定的字符串，填充之后的长度为width,原字符串居左显示，
>
> ​	rjust(width[,fillchar]):用fillchar填充指定的字符串，填充之后的长度为width,原字符串居右显示，
>
> ​	zfill(width)：原字符串居右显示，剩余的字符默认用0填充
>
> ​	strip():去除一个指定字符串中两端指定的子字符
>
> ​	lstrip():去除一个指定字符串中左边指定的子字符
>
> ​	rstrip():去除一个指定字符串中右边指定的子字符

##### 3.4合并和分割

> ​	join()：使用指定的子字符串将列表中的元素连接【列表-----》字符串】
>
> ​	split():使用指定的子字符串将原字符串进行分割，得到一个列表  【字符串-----》列表】

##### 3.5替换

> ​	replace(old,new):将原字符串中的old替换为new
>
> ​	映射替换：
>
> ​		maketrans():生成映射表
>
> ​		translate():根据映射表将指定字符串中的指定字符替换为映射表中对应的字符

##### 3.6判断

> ​	isalpha():一个字符串非空并字符全部是字母才返回True    
>
> ​	isalnum():一个字符串非空并字符是字母或者数字才返回True   ***
>
> ​	isupper()/islower()/istitle():和upper，lower,title有关
>
> ​	isdigit()/isdecimal():一个字符串非空并字符全部是数字才返回True   ***
>
> ​	startswith()；判断一个字符串是否是以指定自字符串开头【前缀】
>
> ​	endswith():判断一个字符串是否是以指定自字符串结尾【后缀】

##### 3.7编码和解码

> ​	encode():编码
>
> ​	decode()；解码
>
> ```Python
> """
> 字符串类型str和字节类型bytes
> 
> 编码：将字符串类型转换为字节类型的过程
> 解码：将字节类型转换为字符串的过程
> 
> 常用编码格式：
>  utf-8/UTF-8/utf8/UTF8
>  gbk/GBK
> """
> 
> #1.编码：将字符串类型转换为字节类型的过程
> #方式一：encode
> str1 = "hello1224%%###中文测试"
> r0 = str1.encode("utf-8")
> r1 = str1.encode("gbk")
> print(r0,type(r0))
> print(r1,type(r1))
> 
> #方式二：bytes()
> str1 = "hello1224%%###中文测试"
> r0 = bytes(str1,encoding="utf-8")
> r1 = bytes(str1,encoding="gbk")
> print(r0,type(r0))
> print(r1,type(r1))
> 
> 
> #2.解码：将字节类型转换为字符串的过程
> #方式一：decode()
> r2 = r0.decode("utf-8")
> r3 = r1.decode("gbk")
> print(r2,type(r2))
> print(r3,type(r3))
> 
> #方式二：str()
> r2 = str(r0,encoding="utf-8")
> r3 = str(r1,encoding="gbk")
> print(r2,type(r2))
> print(r3,type(r3))
> 
> #注意：一般情况下，编解码的格式必须一致，否则乱码
> ```

#### 4.练习

> ```Python
> """
> 1.已知字符串：“this is a test of Python”
> 	a.统计该字符串中字母s出现的次数
> 	b.取出子字符串“test”
> 	c.采用不同的方式将字符串倒序输出【面试题】
> 	d.将其中的"test"替换为"exam"
> """
> str1 = "this is a test of Python"
> #a
> c = str1.count("s")
> 
> #b
> s1 = str1[10:14]
> 
> #c
> #方式一
> s1 = str1[::-1]
> print(s1)
> 
> #方式二
> s2 = ""
> i = len(str1) - 1
> while i >= 0:
>  s2 += str1[i]
>  i -= 1
> print(s2)
> 
> #方式三
> #reverse（）是列表的功能
> list1 = list(str1)
> list1.reverse()
> 
> s3 = ""
> for ch in list1:
>  s3 += ch
> print(s3)
> 
> #d
> str2 = str1.replace("test","exam")
> print(str1)
> print(str2)
> 
> 
> #面试题
> str1 = "this is a test of Python"
> str1.replace("test","exam")
> print(str1)
> 
> """
> 2.已知字符串 a = "aAsmr3idd4bgs7Dlsf9eAF",要求如下
> 	a.请将a字符串的大写改为小写，小写改为大写
> 	b.请将a字符串的数字取出，并输出成一个新的字符串
> 	c.请统计a字符串出现的每个字母的出现次数（忽略大小写，a与A是同一个字母），并输出成一个字典。 例 {'a':4,'b':2}
> 	d.输出a字符串出现频率最高的字母
> 	e.请判断 'boy'里出现的每一个字母，是否都出现在a字符串里。如果出现，则输出True，否则，则输 出False
> """
> a = "aAsmr3idd4bgs7Dlsf9eAF"
> #a
> a1 = a.swapcase()
> print(a)
> print(a1)
> 
> #b
> #方式一
> newStr1 = ""
> for ch in a:
>  if ch.isdigit():
>      newStr1 += ch
> print(newStr1)
> 
> #方式二
> newStr2 = ""
> for ch in a:
>  if ch.isdecimal():
>      newStr2 += ch
> print(newStr2)
> 
> #c
> #忽略大小写
> b = a.lower()
> dict1 = {}
> for ch in b:
>  if ch not in dict1:
>      dict1[ch] = 1
>  else:
>      dict1[ch] += 1
> print(dict1)
> 
> #d
> #获取每个字符的出现次数
> dict1 = {}
> for ch in a:
>  if ch not in dict1:
>      dict1[ch] = 1
>  else:
>      dict1[ch] += 1
> print(dict1)
> 
> #获取次数的最大值
> maxValue = max(dict1.values())
> 
> #在字典中进行比对，找出value对应的key
> for key,value in dict1.items():
>  if value == maxValue:
>      print(key)
> 
> #e
> """
> list1 = [1,2,3,4]
> set1 = set(list1)
> print(set1)
> set1.update([4])
> print(set1)
> """
> 
> #将字符串转化内集合
> strSet = set(a)
> print(strSet)
> search = "boy"
> #将boy更新到集合中
> strSet.update(search)
> print(strSet)
> 
> if len(strSet) == len(set(a)):
>  print(True)
> else:
>  print(False)
> ```
>
> ```Python
> #1.去除字符串两端的指定字符
> str1 = "****abfahe****125323***************"
> #注意：strip(xx),xx可以是任意字符任意长度的字符串，xx尽量只书写一个字符
> str2 = str1.strip("*")
> print(str1)
> print(str2)
> 
> str3 = str1.lstrip("*")
> print(str3)
> 
> str4 = str1.rstrip("*")
> print(str4)
> 
> """
> 2.键盘输入一句英文 将每个单词的首字母大写
> 	例如:
> 		输入: hello nice to meet you
> 		转化之后:Hello Nice To Meet You
> """
> str1 =input("xxx")
> str2 = str1.title()
> print(str2)
> 
> #3.输入一个字符串，压缩字符串如下aabbbccccd变成a2b3c4d1
> newStr = ""
> dict1 = {}
> for ch in "aabbbccccd":
>  if ch not in dict1:
>      dict1[ch] = 1
>  else:
>      dict1[ch] += 1
> 
> for key,value in dict1.items():
>  newStr += key + str(value)
> print(newStr)
> 
> ```

> ```Python
> """
> 1.写代码，有如下变量，请按照要求实现每个功能
> 
> """
> name = "gouguoQ "
> # a.移除name变量对应值的两边的空格，并输出移除后的内容
> str1 = name.strip(" ")
> print(str1)
> 
> # b.判断name变量对应的值是否以"go"开头，并输出结果
> rb = name.startswith("go")
> print(rb)
> 
> # c.判断name变量对应的值是否以"Q"结尾，并输出结果
> rc = name.endswith("Q")
> print(rc)
> 
> # d.将name变量对应的值中的"o"，替换为"p"，并输出结果
> rd = name.replace("o","p")
> print(rd)
> 
> # e.将name变量对应的值根据"o"分割，并输出结果
> name = "gouguoQo"
> #split(subStr,max),默认分割整个字符串，如果指定max，则分割的次数由max决定
> re = name.split("o")
> print(re)
> 
> re = name.split("o",2)
> print(re)
> 
> #splitlines(),默认以换行符进行分割
> str1 = "aaa\nbbb\ncccc\nggfg"
> re = str1.splitlines()
> print(re)
> 
> str2 = """aaa
> bbb
> ccc
> yreytr
> zzzz
> """
> re = str2.splitlines()
> print(re)
> 
> # g.将name变量对应的值变大写，并输出结果
> rg = name.upper()
> print(rg)
> 
> # h.将name变量对应的值变成小写，并输出结果
> rh = name.lower()
> print(rh)
> 
> # i.请输出name变量对应的值的第二个字符
> ri = name[1]
> 
> # j.请输出name变量对应的值的前三个字符
> rj = name[0:3]
> 
> # k.请输出name变量对应值的后2个字符
> rk = name[-2:]
> 
> # l.请输出name变量中的值"Q的索引的位置
> #index()
> rl1 = name.index("Q")
> print(rl1)
> 
> # rl3 = name.index("a")
> # print(rl3)  #ValueError: substring not found
> 
> 
> #find()
> rl2 = name.find("Q")
> print(rl2)
> 
> #注意：如果子字符串不存在，则index直接报错，find返回-1
> rl3 = name.find("a")
> print(rl3)
> 
> 
> #演示
> #index和find，如果查找的是一个长度大于1的字符串，如果存在，则返回子字符串的第0个字符在原字符串中的下标
> str2 = "aahello abchello"
> 
> #从左到右
> r = str2.index("hello")
> print(r)
> r = str2.find("hello")
> print(r)
> #从右到左
> r = str2.rindex("hello")
> print(r)
> r = str2.rfind("hello")
> print(r)
> 
> # m.获取子序列，仅不包含最后一个字符，如：woaini则获取woain  root则获取roo
> rm = name[0:-1]
> 
> # n.利用下划线将列表li = ['gou', 'guo', 'qi']的每一个元素拼接成字符串gou_guo_qi
> name = "gou_guo_qi"
> 
> #分割
> rn1 = name.split("_")
> print(rn1)
> 
> #合并
> #连接字符串.join(列表)
> li = ['gou', 'guo', 'qi']
> newName = "_".join(li)
> print(newName)
> 
> #练习
> s = "hello world"
> print(list(s))
> print(list(s)[:3])   #['h','e','l']
> print("*".join(list(s)[:3]) )#h*e*l
> ```

> ```Python
> #2.概念
> #a.字符串是可迭代对象【可以使用for循环遍历的数据】
> 
> name = "fahjahw"
> #b.遍历字符串
> #方式一
> for ch in name:
>  print(ch)
> 
> #方式二：
> for i in range(len(name)):
>  print(name[i])
> 
> #c.字符串的底层维护了一个元组，和元组一样，字符串属于不可变的数据类型
> 
> 
> #3.实现一个整数加法计算器,例如：从控制台输入 3 + 4，最后输出7
> """
> #方式一:split
> r3 = input("请输入数据：")
> print(type(r3))
> print(r3)
> numList = r3.split("+")   #3+4--->['3','4']    3 + 4----->['3 ',' 4']
> n1 = int(numList[0][0])
> n2 = int(numList[1][-1])
> n3 = n1 + n2
> print(n3)
> """
> 
> #方式二：eval
> """
> r3 = input("请输入数据：")
> r33 = eval(r3)
> print(r33)
> """
> 
> #演示
> print(int("123"))
> print(int("+123"))
> print(int("-123"))
> 
> #print(int("12+3"))  #ValueError: invalid literal for int() with base 10: '12+3'
> print(eval("12+3"))
> print(eval("    12 +3   "))
> print(eval("12 +3   "))
> print(eval("    12 +   3"))
> 
> print(eval("12 * 3"))
> print(eval("12 / 3"))
> 
> ##print(eval("a12 * 3"))  #NameError: name 'a12' is not defined
> 
> #4.统计用户输入的内容中有几个数字，几个字母？
> str4 = "23524$%huhg346"
> 
> #统计数字
> n1 = 0
> #统计字母
> n2 = 0
> for ch in str4:
>  if ch.isdigit():
>      n1 += 1
>  if ch.isalpha():
>      n2 += 1
> 
> #5.编写敏感词语过滤程序，提示用户输入内容，如果用户输入的内容中包含特殊的字符，如山寨 水货，则将内容替换为*****
> 
> """
> #方式一
> data = input("请输入内容：")
> key1 = "山寨"
> key2 = "水货"
> r1 = data.find(key1)
> r2 = data.find(key2)
> if r1 == -1 and r2 == -1:
>  print(data)
> elif r1 != -1 or r2 != -1:
>  #替换
>  data1 = data.replace(key1,"****")
>  data2 = data1.replace(key2,"****")
> 
> #方式二
> while True:
>  data = input("请输入内容【输入q退出】：")
> 
>  if data == "q":
>      break
>  elif "山寨" in data or "水货" in data:
>      data1 = data.replace("山寨","****")
>      data2 = data1.replace("水货","****")
>      print(data2)
>  else:
>      print(data)
> """
> 
> #6.制作表格
> #循环提示用户输入：用户名、密码、邮箱（要求用户输入的长度不能超过20个字符，如果超过则只有前20个字符有效），如果用户输入q或者Q表示不再继续输入，将用户的内容一表格形式打印
> #方式一：%占位符
> """
> while True:
>  name = input("请输入姓名：")
>  pwd = input("请输入密码：")
>  mail = input("请输入邮箱：")
> 
>  name = name[:20]
>  pwd = pwd[:20]
>  mail = mail[:20]
> 
>  print("%s\t%s\t%s" % (name,pwd,mail))
> """
> 
> #方式二
> #format格式化，expandtabs扩展tab【一个tab相当于8个空格】
> """
> newStr = ""
> while True:
>  name = input("请输入姓名：")
>  pwd = input("请输入密码：")
>  mail = input("请输入邮箱：")
> 
>  name = name[:20]
>  pwd = pwd[:20]
>  mail = mail[:20]
> 
>  result = "{0}\t{1}\t{2}\n"
>  result1 = result.format(name,pwd,mail)
>  tab = result1.expandtabs(20)
>  newStr += tab
> 
>  if name == "q" or pwd == "q" or mail == "q" or name == "Q" or pwd == "Q" or mail == "Q":
>      break
> 
> print(newStr)
> """
> 
> #演示：
> print("%s-%s-%s" % ("111","222","333"))
> print("{}-{}-{}".format("111","222","333"))
> 
> #注意1：如果{}中没有任何标记，则{}的个数必须和后面的数据的个数匹配
> #print("{}-{}-{}-{}".format("111","222","333"))
> 
> print("{0}-{1}-{2}-{0}".format("111","222","333"))
> 
> print("{0}-{1}-{1}-{0}".format("111","222","333"))
> 
> #7.从控制台输入一个表示时分秒时间的字符串，格式为：xx：xx:xx,获取该时间的下一秒
> #16:37：23----》16:37：24
> #16:37：59----》16:38：00
> #16:59：59---》17:00:00
> #23:59:59
> 
> timeStr = input("请输入一个时间：")
> 
> timeList = timeStr.split(":")
> h = int(timeList[0])
> m = int(timeList[1])
> s = int(timeList[2])
> 
> s += 1
> 
> if s == 60:
>  s = 0
>  m += 1
>  if m == 60:
>      m = 0
>      h += 1
>      if h == 24:
>          h = 0
> 
> print("%.2d:%.2d:%.2d" % (h,m,s))
> 
> print("{}:{}:{}".format(h,m,s))
> 
> 
> #8.从控制台输入一个单词，判断在一个字符串中出现的次数
> str1 = "this is a test this is a exam this is a test"
> key = "is"
> 
> wordList = str1.split(" ")
> 
> dict1 = {}
> 
> for word in wordList:
>  if word not in dict1:
>      dict1[word] = 1
>  else:
>      dict1[word] += 1
> 
> value = dict1.get(key)
> print(value)
> ```

# Day8

### 一、上堂回顾

#### 1.默写题目

> 已知一个字符串s = "aBcdef",使用系统功能完成下面操作
>
> ​	a.获取字符串的长度
>
> ​	b.统计字符“a”在s中出现的次数
>
> ​	c.判断s是否是以“abc”开头的
>
> ​	d.将s中的字母全部转为大写
>
> ​	e.将其中的“def”替换为"hello"
>
> ​	f.获取“c”在s中第一次出现的位置，如果不存在，返回-1
>
> ```Python
> s = "aBcdef"
> l = len(s)
> print(l)
> c = s.count("a")
> print(s.startswith("abc"))
> s1 = s.upper()
> s2 = s.replace("def","hello")
> index1 = s.find("c")
> ```

### 二、函数

#### 1.函数概述

> 案例：
>
> ```Python
> #需求：求圆的面积
> 
> # r1 = 2
> # s1 = 3.14 * r1 ** 2
> #
> # r2 = 4
> # s1 = 3.14 * r2 ** 2
> #
> # r3 = 7
> # s1 = 3.14 * r3 ** 2
> #
> # r4 = 10
> # s1 = 3.14 * r4 ** 2
> 
> #问题：一旦遇到重复出现的代码，优化代码，可以使用循环【完全相同的代码，代码之间存在某种规律】
> #如果重复出现的代码之间没有规律，优化代码，可以采用函数
> 
> def circleArea(raidus):
>  s1 = 3.14 * raidus ** 2
> 
> circleArea(2)
> circleArea(4)
> circleArea(7)
> circleArea(10)
> ```
>
> 在一个完整的项目中，某些功能会被反复使用，会将反复出现的代码封装成函数，以后如果要继续使用该功能则直接使用函数即可
>
> 本质：对某些特殊功能的封装
>
> 优点：
>
> ​	a.简化代码结构，提高应用的模块性
>
> ​	b.提高了代码的复用性
>
> ​	c.提高了代码维护性

#### 2.函数使用【重点掌握】

##### 2.1定义函数

> 语法：
>
> ​	def  函数名(变量1，变量2....):
>
> ​		函数体
>
> ​		return   返回值
>
> 说明：
>
> ​	a.def是一个关键字，是definition的缩写，专门定义函数
>
> ​	b.函数名：遵循合法标识符的规则和规范即可，尽量做到见名知意
>
> ​	c.(变量1，变量2....):被称为形式参数，是一个参数列表，都只是没有赋值的变量
>
> ​	d.函数体：封装某些特殊的功能
>
> ​	e.return是一个关键字，表示返回，只能用在函数中，表示结束函数，可以单独使用，也可以携带数据，当携带数据，则表示该函数的返回值
>
> ​	f.返回值:常量，变量，表达式
>
> ​	g.函数的定义分为两部分：函数的声明和函数的实现
>
> ​	h.变量1，变量2.... 和 return   返回值 可以根据具体的需求选择性的省略

##### 2.2函数的调用

> ```Python
> def func1():
>  print("func~~~1111")
>  func2()
>  print("exit~~~1111")
> 
> def func2():
>  print("func~~~2222")
>  func3()
>  print("exit~~~2222")
> 
> def func3():
>  print("func~~~3333")
>  func4()
>  print("exit~~~3333")
> 
> def func4():
>  print("func~~~44444")
>  print("exit~~~44444")
> 
> func1()
> 
> #函数的入栈和出栈
> #栈：先进后出，后进先出
> 
> #入栈：函数被调用   出栈：函数被调用完成
> ```

##### 2.3函数的参数

> 形式参数：简称形参，定义在函数的声明部分，本质是一个没有值的变量，用于接收实参的值
>
> 实际参数：简称实参，出现在函数的调用过程中，本质是一个有值的变量或者常量，用于给形参赋值
>
> 传参：实参给形参赋值的过程

##### 2.4形参的分类

> 1》必需参数
>
> 2》默认参数
>
> 3》关键字参数
>
> 4》不定长参数【可变参数】
>
> ```Python
> #1.必需参数
> #a。
> def myPrint(name,age):
>  print(name,age)
> 
> #传参:在函数调用的时候进行
> #实参是常量
> myPrint("jack",18)  #name = "jack"  age = 18
> 
> #实参是变量
> n = "zhangsan"
> a = 10
> myPrint(n,a)   #name = n   age = a
> 
> myPrint(10,37)
> 
> #b
> def myPrint(name,age):
>  print("姓名：%s,年龄：%d" % (name,age))
> 
> myPrint(10,20)
> myPrint("aaa",20)
> #myPrint("bbbb","cccc")  #TypeError: %d format: a number is required, not str
> 
> """
> 总结：
>  a.实参和形参的数量必须一致
>  b.实参的类型和形参的类型必须匹配【主要由函数体和需求决定】
>  c.实参的顺序和形参的顺序尽量保持一致
> """
> 
> #练习：封装函数，求两个数的和
> def mySum(num1,num2):
>  total = num1 + num2
> mySum(23,43)
> 
> #2.默认参数
> #2.1.形参全部设置为默认参数
> def func1(num1 = 10,num2 = 20):
>  print(num1 + num2)
> #a.可以不传参，使用默认值
> func1()
> #b，可以传递一部分参数，按照顺序从前往后进行赋值
> func1(3)    #num1 = 3
> #c
> func1(3,4)  #num1 = 3 num2 = 4
> 
> #2.2将形参的一部分设置默认参数，默认参数处于形参列表的最后
> def func1(num1,num2 = 20):
>  print(num1 + num2)
> #a.
> func1(45)
> #b
> func1(5,7)
> 
> def func1(num1,num2 = 20,num3 = 8):
>  print(num1 + num2)
> func1(4,6)
> 
> #默认参数的好处：可以简化函数的调用
> n1 = int("123")
> n2 = int("110",2)
> 
> print("fahf")
> 
> 
> #3.关键字参数
> #默认参数：针对的是形参列表
> #关键字参数：针对的是实参列表
> #a.
> def show(a,b):
>  print("%s-%d" % (a,b))
> 
> show("fhakfh",18)
> #show(18,"fhakfh")
> 
> #注意1：关键字来源于形参
> show(b = 18,a = "hello")
> show(a = "hello",b = 18)
> 
> #b.
> def show(a,b = 10):
>  print("%s-%d" % (a,b))
> 
> show("aaa")
> show("bbbb",20)
> show(a = "ccc",b = 9)
> #注意：如果实参列表的一部分为关键字参数，最好让关键字参数出现在列表的最后，类似于默认参数的用法
> show("ddd",b = 6)
> #show(a = "ddd",6)
> 
> 
> #关键字参数的好处：传参的时候可以不按照顺序传参
> print("aaa","bbb","cccc",sep="*")
> n2 = int("110",base=2)
> 
> 
> #4.不定长参数【可变参数】:函数在实现的时候可以处理比声明时候更多的参数
> a,b,*c = (1,2,3,4,4,5,5,55)
> print(a,b,c)
> a,*b,c = [1,2,3,4]
> print(a,b,c)
> *a,b,c = [1,2,3,4]
> print(a,b,c)
> 
> #4.1 *
> #注意1：*xxx相当于是一个元组，xx相当于元组的变量名，在函数体可以将xx当做元组处理
> #a.
> def text1(*num):
>  print(num)
>  print(type(num))
> 
>  for n in num:
>      print(n)
> text1()
> text1(10)
> text1(10,20,30)
> text1(10,"aaa",True,10.3)
> text1(10,"aaa",True,10.3,[3,4,34],(5,4,4),{4:5})
> 
> #b
> def text1(num1,*num):
>  print(num1,num)
> text1(3,54,5,45,45)
> 
> #问题：如果在形参列表中设置了必须参数和不定长参数，如果将不定长参数设置在列表的前面或者中间，则会报错
> # def text1(*num1,num):
> #     print(num1,num)
> # text1(3,54,5,45,45)  #TypeError: text1() missing 1 required keyword-only argument: 'num'
> 
> #解决
> #方式一：尽量将不定长参数设置在列表的最后
> def text1(num,*num1):
>  print(num,num1)
> text1(3,54,5,45,45)
> 
> #方式二：结合关键字参数传参
> def text1(*num1,num):
>  print(num1,num)
> text1(3,54,5,45,num = 45)
> 
> #注意：结合上面的演示，在形参列表中，*的不定长参数最多只出现一个
> # def text1(*num1,*num):
> #     print(num1,num)
> # text1(3,54,5,45,45)
> 
> 
> #4.2 **
> #注意1：**xx.则xx代表的是一个字典
> def text2(**num):
>  print(num)
>  print(type(num))
> 
>  for key,value in num.items():
>      print(key,value)
> 
> #注意2：传参的时候，必须以key=value的方式传参，注意和关键字参数的区别
> text2(x=10)
> text2(x=10,y=20,z=30)
> 
> 
> """
> 总结：
>  a.在实际开发中，常用必需参数
>  b.关键字参数和默认参数在系统函数中使用较多
>  c.不定长参数常用的形式：*args,**kwargs
>      args和 kwargs 只是一个标识符，可以是任意的
> """
> ```

##### 2.5参数的传递：值传递和引用传递

> ```Python
> #1.值传递:实参是不可变的数据类型，如number，string，tuple，bool
> def func1(num1):
>  print("修改前num1:%d" % (id(num1)))
>  num1 = 20
>  print("修改后num1:%d" % (id(num1)))
> 
> temp = 10
> print("temp:%d" % (id(temp)))
> func1(temp) #num1 = temp
> print(temp)
> 
> #2.引用传递：实参是可变的数据类型，如：list，dict,set
> def func1(list1):
>  print("修改前num1:%d" % (id(list1)))
>  list1[0] = 20
>  print("修改后num1:%d" % (id(list1)))
> 
> temp = [1,2,3]
> print("temp:%d" % (id(temp)))
> func1(temp)
> print(temp)
> 
> """
> 值传递，如果形参发生改变，实参不受影响
> 引用传递,如果形参发生改变，实参也会随着被修改
> """
> ```

##### 2.6返回值

> return关键字的使用
>
> ```Python
> #1.如果一个函数没有返回值，则默认返回None
> def show1():
>  print("show")
> print(show1())
> 
> #2.如果一个函数中使用return语句，但是没有任何数据，则默认返回None
> #return的作用：用于结束函数，一旦遇到returan语句，后面的语句将没有执行的机会
> def show2():
>  print("show")
>  return
>  #print("hello")
> 
> print(show2())
> 
> #3.如果一个函数中使用return语句，并且后面添加了返回值，则结束函数的同时将指定的数据返回【在哪里调用该函数，则返回到哪里】
> def show3():
>  print("show")
>  return "hello"
> s3 = show3()   #s3 = "hello"
> print(s3)
> 
> #4.return 返回值的意义:在函数内部运算的结果，如果想要在函数外部访问，则只能通过返回值的形式进行间接的访问
> def show4():
>  #局部变量：仅仅能在当前函数中被访问
>  num1 = 10
>  print("函数内部：",num1)
> 
>  return num1
> 
> num2 = show4()   #num2 = num1 = 10
> #print(num1)  #NameError: name 'num1' is not defined
> 
> 
> """
> 封装函数的必要条件：
>  a.形式参数【如果有未知项参与运算，将未知项设置为参数】
>  b.返回值【如果在函数的外部需要访问函数内部的数据，设置返回值】
> """
> 
> #5.特殊情况一：return后面可以跟多个值,在函数外面获取得到的结果为一个元组
> def show5():
>  print("show")
>  return 10,"abc",True
> 
> s5 = show5()
> print(s5)   #(10, 'abc', True)
> 
> #6.特殊情况二：函数的多分支中也可以使用return，可以返回不同类型的数据
> def show6(num):
>  if num > 0:
>      return "正数"
>  elif num < 0:
>      return  -1
>  else:
>      print("等于0")
> 
> print(show6(7))
> print(show6(-7))
> print(show6(0))
> 
> #7.特殊情况三：break和return的作用
> #break只是跳出当前的循环，return只能使用在函数中，结束函数，不管return处于多少层循环之中
> #注意：在某些情况下，在函数中，可以使用return代替break
> def show71():
>  for i in range(5):
>      for j in range(3):
>          print("%d=%d" % (i,j))
>          if j == 1:
>              break
>  print("over~~~71")
> 
> show71()
> 
> print("*" * 20)
> 
> def show72():
>  for i in range(5):
>      for j in range(3):
>          print("%d=%d" % (i,j))
>          if j == 1:
>              return
> 
>  print("over~~~72")
> show72()
> ```

##### 2.7练习一

> ```Python
> #1.封装函数， 比较两个数的大小
> def compare(num1,num2):
>  """
>  比较两个数的大小
>  :param num1: 第一个数
>  :param num2: 第二个数
>  :return: 结果，1则表示第一个数大于第二个数
>                  -1表示第二个数大于第一个数
>                  0则表示相等
>  """
>  if num1 > num2:
>      return 1
>  elif num1 < num2:
>      return -1
>  else:
>      return 0
> 
> 
> #2.封装函数，判断年的平润性
> def isleapyear(year):
>  if (year % 4 == 0 and year % 100 != 0) or year % 400 == 0:
>      return True
>  else:
>      return False
> 
> #4.封装函数，求1~某个数之间整数的和
> def getTotal(num):
>  total = 0
>  for i in range(1,num + 1):
>      total += i
>  return total
> 
> 
> #3.封装函数，统计1~某个数的范围内质数的个数
> #3.1判断一个数是否是质数
> def isprime(num):
>  if num < 2:
>      return False
>  else:
>      result = True
> 
>      for i in range(2,num):
>          if num % i == 0:
>              result = False
>              break
>      return  result
> 
> #3.2统计个数
> def getCount(n):
>  count1 = 0
>  for m in range(1,n + 1):
>      if isprime(m):
>          count1 += 1
>  return count1
> 
> print(getCount(15))
> ```
>
> ```Python
> #1.封装函数，求两个数的和返回结果
> def mySum(num1,num2):
>  return num1 + num2
> 
> 
> #2.封装函数，对一个列表进行冒泡排序，返回排序之后的列表【模拟sort使用】
> def mySort(newList,reverse=False):
>  #reverse为False，升序，  reverse为True，降序
>  if reverse:
>      for i in range(len(newList) - 1):
>          for j in range(len(newList) - i - 1):
>              if newList[j] < newList[j + 1]:
>                  newList[j], newList[j + 1] = newList[j + 1], newList[j]
>  else:
>      for i in range(len(newList) - 1):
>          for j in range(len(newList) - i - 1):
>              if newList[j] > newList[j + 1]:
>                  newList[j], newList[j + 1] = newList[j + 1], newList[j]
> 
>  return newList
> 
> 
> list1 = [23,43,2,43,545,4,100]
> # r = mySort(list1)
> # print(r)
> 
> r = mySort(list1,reverse=True)
> print(r)
> ```

##### 2.8空函数和主函数

> ```Python
> #空函数
> # def test():
> #     pass
> 
> 
> 
> #主函数:只有当前文件被run，则if判断中的代码才会被执行
> if __name__  == "__main__":
>  print("fhafhahfka")
> 
> ```

##### 2.9练习二

> ```Python
> #后台管理会员
> """
> 删除会员
> 删除会员
> 查看会员信息
> 退出系统
> """
> 
> #存储会员信息
> users = {}
> 
> admin = pwd = "root"
> 
> #只有登录当前系统成功之后才能会员操作
> username = input("请输入用户名：")
> password = input("请输入密码;")
> 
> 
> #一、封装函数
> def addUser():
>  adduseraname = input("请输入要添加的用户名：")
>  if adduseraname not in users:
>      addpassword = input("请输入要添加的用户的密码：")
>      users[adduseraname] = addpassword
>      print("添加成功")
>  else:
>      print("该用户已经存在")
> 
> def delUser():
>  deluseraname = input("请输入要删除的用户名：")
>  if deluseraname in users:
>      users.pop(deluseraname)
>      print("删除成功")
>  else:
>      print("该用户不存在")
> 
> def showUser():
>  for name,pwd in users.items():
>      print("用户名称：{0}，用户密码：{1}".format(name,pwd))
> 
> 
> #二、调用函数
> if __name__ == "__main__":
>  if username == admin and password == pwd:
>      print("登录成功")
> 
>      while True:
>          print("菜单".center(30, "*"))
>          print("""1.添加会员
>         2.删除会员
>         3.查看会员信息
>         4.退出系统""")
>          choice = input("请输入你要进行的操作：")
>          if choice.isdigit():
>              choice = int(choice)
>              if choice in range(1, 5):
>                  if choice == 1:
>                      addUser()
>                  elif choice == 2:
>                      delUser()
>                  elif choice == 3:
>                      showUser()
>                  else:
>                      break
>              else:
>                  print("没有该项操作")
>          else:
>              print("输入错误")
> 
> ```

#### 3.匿名函数

> 概念：不再使用def这种标准形式定义函数，而是使用lambda表达式来创建函数，该函数没有函数名，被称为匿名函数
>
> 语法：lambda  形参列表:函数体 
>
> 说明：
>
> ​	a.lambda只是一个表达式，用一行代码实现一个简单的逻辑，可以达到对函数的简化【优点】
>
> ​	b.lambda主体是一个表达式，而不是一个代码块，只能封装有限的逻辑【缺点】
>
> ​	c.lambda拥有自己的命名空间，不能访问自有列表之外或者全局命名空间里的参数
>
> ```Python
> #1.求两个数的和
> def mySum(num1,num2):
>  return  num1 + num2
> 
> r1 = mySum(23,3)
> print(r1)
> #print(mySum)
> 
> mySum1 = lambda num1,num2:num1 + num2
> print(mySum1)
> r2 = mySum1(3,4)
> print(r2)
> 
> #2.
> def test(x,y):
>  print(x,y)
> t1 = test(11,22)
> print(t1)
> 
> test1 = lambda x,y:print(x,y)
> t = test1(11,22)
> print(t)
> 
> #3.练习：封装函数，求两个数的平方和
> def add1(x,y):
>  return x ** 2 + y ** 2
> 
> add2 = lambda x,y:x ** 2 + y ** 2
> 
> 
> #4.匿名函数可以使用默认参数，关键字参数和不定长参数
> t1 = lambda a,b=0:a + b
> print(t1(6))
> print(t1(6,4))
> print(t1(a=7,b=8))
> 
> 
> #5.面试题
> def func():
>  a = []
>  for i in range(5):
>      a.append(lambda x:i * x)
>  return a
> 
> result = func()   #result = a
> print(result)
> print(result[0])  #<function func.<locals>.<lambda> at 0x00000286501A68C8>
> print(result[0](2))
> 
> print(result[0](2))
> print(result[1](2))
> print(result[2](2))
> 
> ```

#### 4.偏函数

> ```Python
> import  functools
> 
> #int(xx)
> 
> #int函数可以把字符串转换为整型，默认情况下，其中的xx被识别为十进制，最终以十进制输出
> print(int("123"))
> 
> #如果是二进制爱，八进制或者十六进制，每次都需要指明
> print(int("110",base=2))
> print(int("110",2))
> 
> print(int("1101",2))
> print(int("1001",2))
> print(int("1000",2))
> print(int("1100",2))
> print(int("1111",2))
> 
> #需求：自定义一个函数，借助于int（），其中的数据被识别为二进制
> #方式一：默认参数
> """
> def int2(x,base=2):
>  return int(x,base)
> 
> print(int2("1101"))
> print(int2("1001"))
> print(int2("1000"))
> print(int2("1100"))
> print(int2("1111"))
> 
> print(int2("110",10))
> """
> 
> #方式二：偏函数
> #对函数的参数做一些控制，把该类函数称为偏函数，一般情况下，偏函数不需要自定义，由系统生成，直接使用
> #第一步：导入模块   import functools
> #第二步：functools.partial(已有的函数名，默认参数)
> int2 = functools.partial(int,base=2)
> print(int2)
> 
> print(int2("1101"))
> print(int2("1001"))
> print(int2("1000"))
> print(int2("1100"))
> print(int2("1111"))
> 
> print(int2("110",base=10))
> 
> #总结：根据一个已知的函数，通过控制该函数的参数生成一个新的函数，新的函数被称为偏函数
> #当一个函数的参数过多的情况下，需要简化函数的调用，使用functools.partial创建一个新的函数，把原函数中的某些参数固定
> #根据不同的需求调用不同的函数
> 
> 
> #预习：列表生成式，生成器，可迭代对象和迭代器，变量的作用域，闭包
> 
> ```

# Day9

### 一、上堂回顾

#### 1.默写题目

> 封装函数，分别实现下面的功能
>
> 1.将某个字符串中的大写字母转化为小写，并将新的字符串返回
>
> ```Python
> #注意1：明确是否需要设置参数和返回值
> def customlower(s):
> #注意2：在字符串操作中，但凡涉及到字符串的修改，则生成了一个新的字符串
> return s.lower()
> ```
>
> 2.计算从1到某个数以内所有奇数的和并返回结果
>
> ```Python
> def getSum(num):
> total = 0
> for n in range(1,num + 1):
>  if n % 2 == 1:
>    total += n
>    
> return total  
> ```
>
> 3.使用二分法查找在某个列表中查找指定元素，将查找到的索引返回
>
> ```Python
> #find---->-1
> 
> #注意1：二分法查找的前提条件：列表必须是有序的
> def customsearch(newList,key):
>  newList.sort()
>  
>  #注意2：查找的思路：通过折半缩小查找范围【和中间下标对应的元素比较大小】
>  
>  left = 0
>  right = len(newList) - 1
>  
>  
>  while left <= right:
>      middle = (left + right) // 2
>      
>      if key > newList[middle]:
>          left = middle + 1
>      elif key < newList[middle]:
>          right = middle - 1
>      else:
>          #处理的是能查找的情况
>          return middle
>      
>  #处理的是查找不到的情况    
>  return -1       
> ```

#### 2.知识点回顾

> 1.函数的定义以及函数的优点
>
> 2.参数
>
> ​	必需参数，默认参数，关键字参数，不定长参数
>
> 3.返回值
>
> ​	return的使用

### 二、列表生成式和生成器【重点掌握】

#### 1.列表生成式

> 列表生成式：List  Comprehensions,是Python内置的专门用来生成列表的一种工具
>
> list(range())
>
> ```Python
> #1.range
> r0 = range(10)
> print(r0)
> print(type(r0))
> 
> #list()
> l0 = list(r0)
> print(l0)
> 
> l1 = list(range(1,10,2))
> print(l1)
> 
> #range()的缺点：生成的列表相当于数学上的等差数列
> 
> #列表生成式的语法：[新列表中元素的规律  for循环  if语句]
> """
> 注意：if语句可以省略的
> """
> 
> #2.需求：生成一个列表，[1,4,9,16,25,36]
> #方式一
> newList1 = []
> for i in range(1,7):
>  newList1.append(i ** 2)
> print(newList1)
> 
> #方式二
> newList2 = [i ** 2 for i in range(1,7)]
> print(newList2)
> 
> #3.需求：生成一个列表，[1,9,25,49,81]
> #方式一
> newList1 = []
> for i in range(1,10):
>  if i % 2 == 1:
>      newList1.append(i ** 2)
> print(newList1)
> 
> #方式二
> newList2 = [i ** 2 for i in range(1,10) if i % 2 == 1]
> print(newList2)
> 
> #4.需求：已知列表[2,4,3,3,6,1],生成一个新的列表，新列表中的元素是已知列表中元素的3倍
> #方式一
> newList1 = []
> for n in [2,4,3,3,6,1]:
>  newList1.append(n * 3)
> print(newList1)
> 
> #方式二
> newList2 = [n * 3 for n in [2,4,3,3,6,1]]
> print(newList2)
> 
> 
> #5.在列表生成式中，可以使用嵌套for循环
> newList1 = [x + y for x in "ABC" for y in "XYZ"]
> print(newList1)
> 
> #6.在列表生成式中，for循环中也可以使用多个变量
> dict1 = {"a":1,"b":2,"c":3}
> newList = [key + "=" + str(value) for key,value in dict1.items()]
> print(newList)
> 
> #练习：将已知列表中所有的元素全部小写，生成一个新的列表
> list1 = ["Aaa","vsf","HELLo"]
> #方式一
> newList1 = []
> for ch in list1:
>  newList1.append(ch.lower())
> print(newList1)
> 
> #方式二
> newList2 = [ch.lower() for ch in list1]
> print(newList2)
> 
> 
> #问题：如果列表中存在各种不同类型的数据，则上面的代码会报错，'int' object has no attribute 'lower'
> list1 = ["Aaa",True,"vsf","HELLo",10]
> 
> #isinstance(变量，类型)，判断一个变量是否是指定的数据类型，是则返回true
> #方式一
> newList1 = []
> for ch in list1:
>  if isinstance(ch,str):
>      newList1.append(ch.lower())
> print(newList1)
> 
> #方式二
> newList2 = [ch.lower() for ch in list1 if isinstance(ch,str)]
> print(newList2)
> ```

#### 2.生成器

> ​	通过列表生成式，可以直接创建一个列表，但是，受到内存限制，列表的容量是有限的，而且如果创建一个包含了100万个元素的列表，不仅会占用很大的内存空间，如果在使用的时候仅仅访问前几个元素，则大量的内存空间会被浪费掉
>
> ​	所以，如果列表中的元素可以通过某种算法计算，在循环中的过程中不断推算出后续的元素，这样就不必创建完整的列表，从而节省大量的内存空间，在Python，这种一边循环一边计算的机制，被称为生成器【generator】
>
> 定义生成器的方式：
>
> ​	a.将列表生成式中的[]改为(),就是一个生成器
>
> ​	b.通过函数和关键字yield生成
>
> ```Python
> #1,列表生成式和生成器之间的区别
> list1 = [i ** 2 for i in range(5)]
> print(list1)
> print(type(list1))
> 
> gene1 = (i ** 2 for i in range(5))
> print(gene1)
> print(type(gene1))
> 
> #2.获取生成器中的元素
> #生成器也是一个可迭代对象，可以采用for循环或者next（）获取其中的元素
> #next():每调用一次，则会获取生成器中的一个元素
> 
> #方式一
> print(next(gene1))
> print(next(gene1))
> print(next(gene1))
> print(next(gene1))
> print(next(gene1))
> 
> print("*" * 20)
> 
> #注意：如果一个生成器中的元素通过next获取完毕，再次调用next，则会报错StopIteration【停止迭代】
> #print(next(gene1))
> 
> #方式二
> for num in gene1:
>  print(num)
> 
> 
> #3.通过函数和yield关键字生成
> #3.1普通函数
> def test(n):
>  for x in range(1,n + 1):
>      print(x)
> 
> t = test(10)
> print(t)   #None
> 
> print("*" * 20)
> 
> #3.2
> #yield：暂停
> def test(n):
>  for x in range(1,n + 1):
>      print("hello",x)
>      yield x
>      print("x=%d" % (x))
> 
> t = test(10)
> print(t)
> 
> # print(next(t))
> # print(next(t))
> # print(next(t))
> # print(next(t))
> # print(next(t))
> # print(next(t))
> 
> #使用循环获取生成器中的所有的元素
> while True:
>  try:
>      print(next(t))
>  except:
>      break
> 
> 
> """
> 总结：
>  工作原理：每次调用next的时候，函数会执行到yield停止，将yield后面的值返回，代码停止，下次再调用next
> 函数生成器会接着从yield后面的代码继续执行。。。。
>  生成器类似于返回值为一个列表的函数，这个函数可以接收参数，可以被调用，但是，不同于一般列表的地方在于：
> 一般的函数一次性返回一个非空的列表 ，生成器只能生成一个值，这样消耗的内存会减少
> """
> #一般函数
> def func(n):
>  list1 = []
>  for i in range(1,n + 1):
>      list1.append(i)
>  return list1
> 
> #生成器函数
> def test(n):
>  for x in range(1, n + 1):
>      yield x
> ```

### 三、可迭代对象和迭代器【面试题】

#### 1.可迭代对象

> 只能用for循环遍历的数据被称为可迭代对象【Iterable类】
>
> 可迭代对象的数据类型：
>
> ​	a.集合数据类型：list,tuple,dict,set,str
>
> ​	b.generator:包括()生成器和带yield关键字的函数
>
> ```Python
> from collections import  Iterable
> 
> print(isinstance([],Iterable))
> print(isinstance((),Iterable))
> print(isinstance({},Iterable))
> print(isinstance((x for x in range(4)),Iterable))
> print(isinstance("abc",Iterable))
> 
> print(isinstance(10,Iterable))
> print(isinstance(True,Iterable))
> ```

#### 2.迭代器

> 不但可以使用for循环遍历，还可以被next函数调用的数据被称为迭代器【Iterator类】
>
> 迭代器的数据类型：生成器
>
> ```Python
> from collections import  Iterator
> 
> print(isinstance([],Iterator))
> print(isinstance((),Iterator))
> print(isinstance({},Iterator))
> print(isinstance("abc",Iterator))
> 
> print(isinstance(10,Iterator))
> print(isinstance(True,Iterator))
> 
> print(isinstance((x for x in range(4)),Iterator))
> 
> 
> #iter(),将一个不是迭代器的可迭代对象转换为迭代器
> print(isinstance(iter([]),Iterator))
> print(isinstance(iter(()),Iterator))
> print(isinstance(iter({}),Iterator))
> print(isinstance(iter("abc"),Iterator))
> ```

> 联系：
>
> ​	a.迭代器一定是可迭代对象，但是可迭代对象不一定是迭代器
>
> ​	b.通过iter()可以将一个不是迭代器的可迭代对象转换为迭代器【list,tuple,dict,set,str】

### 四、函数的本质【重点掌握】

#### 1.变量可以指向函数

> ```Python
> #1.变量可以指向函数
> 
> #获取函数调用的结果
> print(abs(-10))  #10
> #获取求绝对值的函数
> print(abs)  #<built-in内置/內建 function abs>
> 
> x = abs(-18)
> print(x)
> 
> f = abs
> print(f)
> 
> #结论：函数本身可以赋值给变量，如果一个变量指向一个函数，则可以通过该变量调用指定的函数
> print(f(-20))
> 
> ```

#### 2.函数名是一个变量名

> ```Python
> #2.函数名是一个变量名
> print(abs(-36))  #36
> 
> #给函数名重新赋值
> #abs = 10
> 
> #print(abs(-36))  #TypeError: 'int' object is not callable
> 
> #list,tuple,dict,set不要被使用为变量名
> 
> #结论：函数名就是一个变量名，只不过该变量指向一个可以实现某种功能的函数，同时也可以给该变量进行重新赋值
> #但是，如果给函数名重新赋值，则再次调用函数无法使用，注意：定义变量的时候，尽量避开系统函数或者模块的命名
> 
> 
> ```

#### 3.函数可以作为参数

> ```Python
> #3.函数可以作为参数
> #3.1
> def add(x,y,f):
>  return f(x) + f(y)
> 
> num1 = 2
> num2 = -3
> r0 = add(num1,num2,abs)
> print(r0)
> 
> #3.2
> def add(x,y,f):
>  return f(x,y) + f(x,y)    #test(3,4) + test(3,4)
> 
> def test(a,b):
>  return  a + b
> 
> print(add(3,4,test))  #f = test
> 
> #结论：一个函数可以作为另外一个函数的参数使用，传参的时候，只需要传递函数名即可
> 
> 
> ```

### 五、闭包【重点掌握】

> 如果在一个函数的内部定义了另外一个函数，外部的函数被称为外部函数【outter】,里面的函数被称为内部很熟【inner】
>
> 在一个外部函数中定义一个内部函数，并且外部函数的返回值为内部函数的引用，这样就构成了闭包【Closure】
>
> ```Python
> #1.简单的闭包【没有参数】
> def outter1():
>  def inner1():
>      print("闭包被调用了")
>      return 10
> 
>  return inner1
> 
> f1 = outter1()
> print(f1)
> print(f1())
> 
> #注:1：闭包除了外部函数必须返回内部函数的引用之外，其他用法和普通用法完全相同
> 
> #2。有参数的闭包【外部函数】
> #a和num被称为自由变量或者临时变量：在内部函数中可以直接任意访问
> def outter2(a):
>  num = 19
>  def inner2():
>      print(a,num)
>  return inner2
> 
> f2 = outter2(36)
> f2()
> 
> #注意2：一个函数访问另外一个函数中的变量，使用了闭包之后，将不再需要设置返回即可访问
> 
> #3.有参数的闭包【内部函数】
> def outter3(a):
>  num = 19
>  def inner3(b):
>      print(a + b,num)
>  return inner3
> 
> f3 = outter3(3)  #f3 = inner3
> f3(4)
> 
> #注意3：注意变量的作用域，闭包常用的场景是装饰器
> 
> ```

### 六、变量的作用域【重点掌握】

#### 1.概念

> 出现的原因：变量的作用域指的是变量可以被访问的范围
>
> 程序中的变量并不是在任意的位置都可以访问，访问权限取决于该变量被定义的位置
>
> 变量的生命周期也决定了变量被访问的范围
>
> 分类：
>
> ​	L:local,局部作用域
>
> ​	E:Enclosing,函数作用域【定义在外部函数和内部函数之间】
>
> ​	G:Global,全局作用域
>
> ​	B:Built-in,內建作用域【内置作用域】 a = abs

#### 2.查找规则

> ```Python
> #1.变量不重名
> #全局作用域:在当前py文件都能被访问
> num1 = 10
> print(num1)
> 
> def outter1():
>  #函数作用域：只能在当前外部函数中
>  num2 = 20
> 
>  print(num1,num2)
> 
>  def inner1():
>      #局部作用域：只能在当前内部函数中
>      num3 = 30
> 
>      print(num1,num2,num3)
> 
>  return inner1
> 
> f1 = outter1()
> f1()
> 
> print("*" * 20)
> 
> #2.变量重名
> num = 10
> print(id(num))
> def outter2():
>  num = 20
>  print(id(num))
>  def inner2():
>      num = 30
>      print(id(num))
>      print(num)
> 
>  return inner2
> 
> f2 = outter2()
> f2()
> 
> print(num)  #30
> 
> #结论：当不同作用域下的变量重名的时候，访问变量采用的是就近原则，查找的规则：L---->E----->G
> #建议：在实际开发中，如果涉及到多个不同的作用域，尽量避免变量的重名，
> 
> 
> #3.哪些语句能够引入新的作用域
> if True:
>  n1 = 37
> print(n1)
> 
> n = 0
> while n < 2:
>  n2 = 20
>  n += 1
> print(n2)
> 
> """
> 总结：
>  1.能够引入新的作用域：函数【def,lambda】、模块【module】、类【class】
>  2.不能引入新的作用域：if语句，while语句，for语句，try-except语句
> """
> 
> ```

#### 3.全局变量和局部变量

> 说明：全局和局部只是一个相对的概念
>
> ```Python
> #形式一
> #全局变量
> num1 = 10
> def test():
> #局部变量
> num2 = 20
> 
> 
> #形式二
> #全局变量
> num1 = 10
> def outter():
> #函数作用域的变量
> num2 = 20
> def inner1():
>  #局部变量
>  num3 = 30
> 
> return inner1
> 
> ```
>
> 全局变量：直接定义在py文件中，可以在整个py文件中被任意访问，当程序执行完毕会被自动销毁
>
> 局部变量：定义在函数内部，只能在当前函数中被访问，当函数调用完毕【出栈】则会被自动的销毁
>
> ```Python
> #全局变量
> total = 0
> 
> def add(num1,num2):
>  #print(total)
>  #局部变量
>  total = num1 + num2
>  print("内部：",total)
> 
> add(23,4)
> print(total)
> 
> ```

#### 4.global和nonlocal关键字

> global
>
> ```Python
> #1.
> num = 1
> def func1():
>  print(num)
> 
> func1()
> 
> #2.
> num = 1
> def func1():
>  num = 2
>  print(num)
> func1()
> print("*" * 20)
> 
> #3.
> num = 1
> def func1():
>  global num
>  print(num)  #UnboundLocalError: local variable 'num' referenced before assignment
>  #重新赋值
>  num = 2
>  print(num)
> func1()
> 
> print("num=%d" % (num))
> 
> 
> #面试题
> a = 20
> def test():
>  global a
>  a += 1    #a = a + 1
> 
> test()
> print(a)
> 
> 
> #总结：当全局变量和局部变量重名，在局部变量定义之前访问全局变量，则会报错，
> # 解决办法：在使用全局变量之前作出一个声明，告诉编译器当前的变量是全局变量
> 
> ```
>
> nonlocal只能使用在闭包中
>
> ```Python
> #全局作用域
> x = 0
> 
> def outter():
>  #函数作用域
>  x = 1
>  def inner():
>      #局部作用域
>      nonlocal x
>      x = 2
>      print("inner:",x)
> 
>  inner()
> 
>  print("outter:", x)
> 
> f = outter()
> print("global:",x)
> """
> inner: 2
> outter: 1  ---- >2
> global: 0
> """
> 
> #总结：当变量重名的前提下，修改内部函数的局部作用域为函数作用域，nonlocal扩大作用域
> 
> ```

### 七、装饰器基本用法

> 如果增强一个函数的功能但是又不希望原函数被修改，这种代码运行的期间动态增加函数功能的机制被称为装饰器【Decorator】
>
> 装饰器的本质：就是一个闭包，只是需要被装饰的函数当做参数传递给闭包，最后返回装饰之后的结果【内部函数的引用】
>
> 高阶函数：将一个函数作为另外一个函数的参数，返回一个结果
>
> ```Python
> def test():
>  print("hello")
> 
> 
> #装饰器的书写步骤;
> #a。定义一个闭包
> #b.将需要增强功能的函数作为参数传递给装饰器的外部函数
> def outter(func):
>  def inner():
>      #d.新增功能
>      print("abc")
> 
>      # c。调用原函数
>      func()
> 
>  return inner
> 
> f = outter(test)   #func = test   f = inner
> f()
> 
> print("********")
> 
> #练习
> def check(num):
>  print(num)
> 
> def outter(f):  #f = check
>  def inner(a,b):
>      f(39)
>      print(a + b)
> 
>      return a + b
>  return inner
> 
> f2 = outter(check)  #f2 = inner
> result = f2(3,5)
> print(result)
> 
> 
> #预习：装饰器，高阶函数，递归，栈和队列【遍历磁盘上的目录】
> 
> ```

# Day10

### 一、上堂回顾

#### 1.默写题目

> 1.举例说明函数的本质
>
> ```Python
> def test():
> pass
> 
> #1.变量可以指向函数
> f = test
> f()
> 
> #2.函数名就是一个变量名
> test = "hello"
> #test()   #报错
> 
> #3.函数可以作为参数使用
> def check(a):
> a()
> 
> check(test)
> ```
>
> 2.简述可迭代对象和迭代器的区别和联系
>
> ```Python
> """
> 区别：
> 	可迭代对象：只能使用for循环遍历的数据，如：集合类型【list,tuple.dict,set,string】和生成器【()生成器和函数生成器】
> 	迭代器：可以使用for循环或者next遍历的数据，如：生成器
> 联系：
> 	迭代器一定是可迭代对象，可迭代对象不一定是迭代器
> 	可以通过iter()将不是迭代器的可迭代对象转化为迭代器
> """
> ```
>
> 3.通过列表生成式生成列表[0,2,4,6,8,10]
>
> ```Python
> #
> list1 = list(range(0,11,2))
> 
> list2 = [i for i in range(0,11,2)]
> list2 = [i for i in range(0,11) if i % 2 == 0]
> ```
>
> 4.定义一个闭包，并调用闭包中的内外函数
>
> ```Python
> def outter():
>  def inner():
>      pass
>  return inner
> 
> f = outter()
> f()    
> ```

#### 2.知识点回顾

> 1.函数的本质
>
> 2.列表生成式和生成器【面试题】
>
> 3.可迭代对象和迭代器
>
> 4.函数的作用域
>
> ​	闭包
>
> ​	作用域的范围
>
> ​	global和nonlocal：只有在不同作用域下的变量重名的情况下，声明变量的作用域

### 二、装饰器【重点掌握】

> 学习思路：
>
> ​	a.如何自定义装饰器
>
> ​	b.装饰器的工作原理【系统的装饰器】
>
> ```Python
> """
> 装饰器的本质：就是一个闭包，只不过该闭包的外部函数的参数为另一个函数【需要被装饰的函数】
> 
> 在装饰器的使用过程中，应用到了函数的本质
> 
> 装饰器的好处：可以在不用修改原函数的基础上，给指定的函数增强新的功能
> """
> 
> #1.最简单的装饰器
> def now():
>  print("好好学习，天天向上")
> 
> def wrapper(fun):
>  print("外部函数被调用了")
> 
>  def inner():
>      #在inner中，调用原函数，增加新功能，顺序可以根据具体的需求进行调换
>      fun()
> 
>      print("新的功能")
> 
>  return inner
> 
> f1 = wrapper(now)  #f1 = inner
> f1()  #inner()
> 
> #练习：给下面的test函数增加新的功能，打印九九乘法表
> def test():
>  for i in range(10):
>      print(i)
> def wrapper(f):
>  def inner():
>      #原来的功能
>      f()
> 
>      #新的功能
>      for i in range(1,10):
>          for j in range(1,i + 1):
>              print("%dx%d=%d" % (j,i,i * j),end=" ")
>          print()
>  return inner
> 
> f = wrapper(test)
> f()
> 
> """
> 注意：
>  a.wrapper被称为装饰器的名称
>  b.应用场景：统计函数的执行时间，日志处理，函数执行完毕之后的清理功能，权限校验，缓存的处理
> """
> 
> print("*" * 30)
> 
> #2.有参数的装饰器
> def getage(age):
>  print("你的年龄是：%d" % (age))
> 
> # getage(18)
> # getage(-9)
> 
> def wrapper2(f):
>  def inner2(age):
>      #新增的功能：数据的校验
>      if age < 0:
>          age = -age
> 
>      #调用原函数
>      f(age)
> 
>  return inner2
> 
> f2 = wrapper2(getage)
> f2(-9)
> 
> #说明：如果原函数有参数，并需要对原函数的参数做操作，则可以给装饰器的内部函数设置参数
> 
> print("*" * 30)
> 
> #3.@xxxx简化装饰器的使用和调用
> 
> #注意：使用   @装饰器名  作用于原函数，则装饰器必须先存在，才能修饰函数
> 
> def wrapper3(f):
> 
>  print("外部wrapper~~~3333")
> 
>  def inner3(age):
>      print("内部iner~~~3333")
>      if age < 0:
>          age = -age
>      f(age)
> 
>      print("over")
>  return inner3
> 
> @wrapper3    #等价getage = wrapper3(getage)      getage = inner3
> def getage(age):
>  print("你的年龄是：%d" % (age))
> 
> getage(-18)
> 
> """
> @wrapper3 :完成了将原函数传参，执行了装饰器的外部函数
> 当外部函数加载完毕，返回值inner3会赋值给getage【使用装饰器，原函数的函数名修改了自己的指向，指向了装饰器的内部函数】
> """
> 
> print("*" * 30)
> 
> #4,一个装饰器作用于多个函数
> #多个不同的函数增加了同一个功能
> def wrapper4(fun):
>  def inner4(*args,**kwargs):
>      fun(*args,**kwargs)
> 
>      print("new")
>  return inner4
> 
> @wrapper4
> def func1():
>  print("func~~~111")
> 
> func1()
> 
> @wrapper4
> def func2(a):
>  print("func~~~222")
> 
> func2(10)
> 
> @wrapper4
> def func3(num1,num2,num3):
>  print("func~~~3333")
> 
> func3(10,20,30)
> 
> #结论：如果想让一个装饰器同时可以作用于多个函数，则给装饰器的内部函数设置不定长参数，用于接收个数不确定的参数
> 
> print("*" * 30)
> 
> #5.多个装饰器作用于同一个函数
> #给一个函数同时增加多个不同的功能
> #5.1
> def wrapper_1(func1):
>  def inner1():
>      print("装饰器~~~1111")
>      func1()
>  return inner1
> 
> def wrapper_2(func2):
>  def inner2():
>      print("装饰器~~~2222")
>      func2()
>  return inner2
> 
> def wrapper_3(func3):
>  def inner3():
>      print("装饰器~~~3333")
>      func3()
>  return inner3
> 
> @wrapper_1    #func1 = show[show---->inner2]  show = inner1
> @wrapper_2   #func2 = show[show--->inner3]   show = inner2
> @wrapper_3    #func3 = show    show = inner3
> def show():
>  print("showing")
> 
> show()    #inner1()
> """
> 装饰器~~~1111
> 装饰器~~~2222
> 装饰器~~~3333
> showing
> """
> 
> print("*" * 30)
> 
> #5.2
> def wrapper_1(func1):
>  def inner1():
>      print("装饰器~~~1111")
>      func1()
>  return inner1
> 
> def wrapper_2(func2):
>  def inner2():
>      print("装饰器~~~2222")
>      func2()
>  return inner2
> 
> def wrapper_3(func3):
>  def inner3():
>      print("装饰器~~~3333")
>      func3()
>  return inner3
> 
> @wrapper_1
> @wrapper_3
> @wrapper_2
> def show():
>  print("showing")
> show()
> """
> 装饰器~~~1111
> 装饰器~~~3333
> 装饰器~~~2222
> showing
> """
> print("*" * 30)
> 
> #5.3
> def wrapper_1(func1):
>  def inner1():
>      print("装饰器~~~1111")
>      func1()
>  return inner1
> 
> def wrapper_2(func2):
>  def inner2():
>      func2()
>      print("装饰器~~~2222")
>  return inner2
> 
> def wrapper_3(func3):
>  def inner3():
>      print("装饰器~~~3333")
>      func3()
>  return inner3
> 
> @wrapper_1   #func1 = show[show---->inner2]   show = inner1
> @wrapper_2   #func2 = show[show---->inner3]  show = inner2
> @wrapper_3   #func3=show   show = inner3
> def show():
>  print("showing")
> show()
> """
> 装饰器~~~1111
> 装饰器~~~3333
> showing
> 装饰器~~~2222
> """
> 
> #5.4
> def wrapper_1(func1):
>  def inner1():
>      func1()
>      print("装饰器~~~1111")
>  return inner1
> 
> def wrapper_2(func2):
>  def inner2():
>      func2()
>      print("装饰器~~~2222")
>  return inner2
> 
> def wrapper_3(func3):
>  def inner3():
>      print("装饰器~~~3333")
>      func3()
>  return inner3
> 
> @wrapper_1
> @wrapper_3
> @wrapper_2
> def show():
>  print("showing")
> show()
> """
> 装饰器~~~3333
> showing
> 装饰器~~~2222
> 装饰器~~~1111
> """
> 
> """
> 总结：
>  a。当多个装饰器修饰同一个函数时，采用的就近原则，从下往上进行传参【一直改变原函数的指向】，从上往下执行
>  b.原函数都只会被执行一次
>  c.通过不断修改原函数的指向完成整个装饰器的调用过程
> """
> ```

### 三、高阶函数【重点掌握】

> 一个函数的参数为另外一个函数，返回一个结果，该函数被称为高阶函数
>
> 参数部分的函数可以是def或者lambda表达式

#### 1.map映射

> ```Python
> #replace(old,new)
> 
> #maketrans():创建字符串的映射表
> #translate():通过映射表转换字符串
> 
> #参数：原字符串中的字符    转换的目标
> t = str.maketrans("abcdef","$#@%&*")
> print(t)
> 
> s1 = "aaahello"
> s2 = s1.translate(t)
> print(s2)
> 
> 
> #map的用法
> """
> map(fn,Iterable1,Iterable2.....)
>  fn:函数【def 和 lambda】
>  Iterable:可迭代对象
> 
> 功能：根据fn中的逻辑，依次作用域序列中的每一个元素，最终返回一个新的序列
> """
> 
> #1.需求：已知[1,2,3,4,5],生成[1,4,9,16,25]
> list1 = [1,2,3,4,5]
> #方式一
> newlist1 = []
> for num in list1:
>  newlist1.append(num ** 2)
> print(newlist1)
> #方式二
> newlist2  = [num ** 2 for num in list1]
> print(newlist2)
> 
> #方式三
> result3 = (num ** 2 for num in list1)
> print(list(result3))
> 
> #方式四
> #4.1
> #注意：如果序列只有一个，则函数的参数也只能是一个
> def func(x):
>  return x ** 2
> result4 = map(func,list1)
> print(result4)
> print(list(result4))
> 
> #4.2
> result42 = map(lambda x:x ** 2,list1)
> print(list(result42))
> 
> #2.需求：已知[1,2,3,4,5],生成['1','2','3'....]
> newlist1 = []
> for num in [1,2,3,4,5]:
>  newlist1.append(str(num))
> print(newlist1)
> 
> newlist2 = [str(num) for num in [1,2,3,4,5]]
> print(newlist2)
> 
> result21 = (str(num) for num in [1,2,3,4,5])
> print(list(result21))
> 
> result22 = map(str,[1,2,3,4,5])
> print(list(result22))
> 
> #3.有多个序列
> #
> newlist1 = [x + y for x in [1,2,3] for y in [4,5,6]]
> print(newlist1)
> 
> def add(x,y):
>  return  x + y
> result3 = map(add,[1,2,3],[4,5,6,7])
> print(list(result3))
> 
> """
> 注意：
>  1.map中的序列有几个，函数的参数一般设置几个【一一对应】
>  2.map中的函数一般都要设置返回值，否则生成的元素全部是None【将函数运算的结果存储在一个新的容器中】
>  3.多个序列的长度可以不一致，以元素个数少的序列作为参照
> """
> 
> #练习：将已知列表中的元素全部转化为大写字母，生成一个新的容器
> list1 = ["faf","Hello","AAA"]
> 
> newlist1 = [ch.upper() for ch in list1]
> print(newlist1)
> 
> result = list(map(lambda ch:ch.upper(),list1))
> print(result)
> ```

#### 2.reduce减少【累积】

> ```Python
> from functools import  reduce
> 
> """
> reduce(fn，Iterable)
> 
> 功能：使用fn首先将Iterable中第0和第1个元素进行运算，将得到的结果和第2个元素进行运算。。。。
> 直到Iterable中元素全部参与运算
> 
> 举例：
> func(x,y)
> [a,b,c,d]
> 
> reduce(func,[a,b,c,d])
> 
> 工作原理：
> func(func(func(a,b),c),d)
> """
> 
> #1.需求:求 一个列表中所有的元素和
> list1 = [1,2,3,4,5]
> 
> #方式一
> total1 = 0
> for num in list1:
>  total1 += num
> print(total1)
> 
> #方式二
> def add(a,b):
>  return  a + b
> result1 = reduce(add,list1)
> print(result1)
> 
> #2.练习：求10的阶乘
> #方式一
> result2 = 1
> for i in range(1,11):
>  result2 *= i
> print(result2)
> 
> #方式二
> def test(x,y):
>  return x * y
> result21 = reduce(test,range(1,11))
> print(result21)
> 
> #方式三
> result22 = reduce(lambda x,y:x * y,range(1,11))
> print(result22)
> 
> #3.练习：将列表[2,4,6,8]转换为整数2468
> """
> 2,4---->24---->2 * 10 + 4
> 
> 2,4,6
> 2,4---->24---->2 * 10 + 4
> 24,6---->246---->24 * 10 + 6
> """
> 
> def check(x,y):
>  return  x * 10 + y
> result3 = reduce(check,[2,4,6,8])
> print(result3)
> 
> result31 = reduce(lambda x,y:x * 10 + y,[2,4,6,8])
> print(result31)
> 
> #4.需求：使用map和reduce实现字符串转整型的操作
> #"6523" ----->6523
> #第一步：建立映射关系
> def strtoint(s):
>  dict1 = {'0':0,'1':1,'2':2,'3':3,'4':4,'5':5,'6':6}
>  return dict1[s]
> 
> result1 = list(map(strtoint,"6523"))
> print(result1)
> 
> #第二步：实现转换
> result2 = reduce(lambda x,y:x * 10 + y,result1)
> print(result2)
> 
> #合起来写
> result3 = reduce(lambda  x,y:x * 10 + y,map(strtoint,"6532"))
> print(result3)
> ```

#### 3.filter过滤

> ```Python
> """
> filter(fn,Iterable)
> 
> 功能：通过一定的条件过滤可迭代对象中数据，
>    根据函数的返回值为True或者False决定是否保留元素，如果为True则保留，为False则过滤
> """
> 
> #1.需求：将列表中的偶数元素保留，将奇数元素过滤
> list1 = list(range(1,11))
> 
> #方式一
> newlist1 = []
> for num in list1:
>  if num % 2 == 0:
>      newlist1.append(num)
> print(newlist1)
> 
> #方式二
> newlist2 = [num for num in list1 if num % 2 == 0]
> print(newlist2)
> 
> #方式三
> def check(num):
>  if num % 2 == 0:
>      return True
>  else:
>      return False
> 
> result1 = filter(check,list1)
> print(result1)
> print(list(result1))
> 
> #2.需求：将其中为“无”的数据过滤掉
> list2 = [["张三",18,100,"跳舞"],["lisi",15,95,"无"],["jack",19,60,"唱歌"]]
> 
> def test(ch):
>  if ch == "无":
>      return False
>  return True
> 
> newlist = []
> for sublist in list2:
>  m = filter(test,sublist)
>  newlist.append(list(m))
> print(newlist)
> ```

#### 4.sorted排序

> ```Python
> #一、sort
> list1 = [3,534,54,654,28]
> print(list1)
> #1.升序
> # list1.sort()
> # print(list1)
> 
> #2.降序
> list1.sort(reverse=True)
> print(list1)
> 
> #3.自定义排序规则
> list1 = ["ff","6fhufhua","hello","aba"]
> list1.sort(key=len,reverse=True)
> print(list1)
> 
> #4.
> list1 = ["ff","6fhufhua","hello","aba"]
> def func(ch):
>  return ch.upper()
> 
> list1.sort(key=func)
> print(list1)
> 
> 
> print("*" * 20)
> 
> 
> #二、sorted
> list1 = [3,534,54,654,28]
> print(list1)
> #1.升序
> list2 = sorted(list1)
> print(list1)
> print(list2)
> 
> #2.降序
> list3 = sorted(list1,reverse=True)
> print(list3)
> 
> #3.自定义排序规则
> list1 = ["ff","6fhufhua","hello","aba"]
> list4 = sorted(list1,key=len,reverse=True)
> print(list4)
> 
> #4.
> list1 = ["ff","6fhufhua","hello","aba"]
> def func(ch):
>  return ch.upper()
> 
> list2 = sorted(list1,key=func)
> print(list2)
> 
> """"
> 不同点：
>  1.经过排序，sorted相比较于sort，生成了一个新的列表
>  2.sort是属于列表的功能，但是，sorted中的数据可以是任意的可迭代对象
> 
> 相同点：
>  1.进行降序排序时，都使用reverse=True
>  2.如果要自定义排序的规则，可以自定义函数，二者使用的都是key=函数名
> """
> 
> ```

### 四、递归函数

#### 1.概念

> 递归函数：一个函数调用自身，该函数被称为递归函数
>
> 递归调用：整个代码执行的过程被称为递归调用
>
> 递归包含了一种隐式的循环，它会重复执行某段代码，但是，这种循环不需要条件进行控制
>
> 需要解决的问题：在合适的时机让隐式的循环停止下来
>
> 使用递归 解决问题的思路：
>
> ​	a.找到一个临界值【能够让递归停止下来的条件】
>
> ​	b.找到两次相邻循环之间的关系

#### 2.实现

> ```Python
> #1。需求，报一个数，在斐波那契数列中输出对应的数
> """
> 1   2    3 4   5  6   7   8   9  10  11  12
> 1   1   2  3   5  8  13  21  34  55  89  144....
> 
> 
> 规律：
>  a.第1个位置和第2个位置上的数是固定的是，都是1-----》临界值【条件】
>  b.第n个位置上数 = 第n - 1个位置上数  + 第n - 2个位置上数
> 
> 
> 分析：
> func(3) = func(2) + func(1)   ---->1  + 1 = 2
> 
> func(5) = func(4) + func(3)
> func(4) = func(3) + func(2)
> func(3) = func(2) + func(1)  ---->1 + 1 = 2
> func(4) = 2 + 1 = 3
> 
> func(3) = func(2) + func(1) ----->1 + 1 = 2
> 
> func(5) = 3 + 2 = 5
> .....
> 
> func(n) = func(n - 1) + func(n - 2)
> 
> """
> count = 0
> def func(n):
>  global count
>  count += 1
>  if n == 1 or n == 2:
>      return 1
>  else:
>      result = func(n - 1) + func(n - 2)
>      return result
> 
> print(func(10))
> print("执行的次数：",count)
> 
> #注意：递归中必须设置返回值，因为在下一次运算中，一般都要用到上一次运算的结果
> 
> 
> #2.练习：使用递归求1~某个数之间所有整数的和
> """
> gettotal(10) = gettotal(9) + 10
> gettotal(9) = gettotal(8) + 9
> gettotal(8) = gettotal(7) + 8
> ....
> gettotal(1) = 1  ---->临界值
> 
> 
> gettotal(num) = gettotal(num - 1) + num  ----》规律
> """
> def gettotal(num):
>  if num == 1:
>      return 1
>  else:
>      return gettotal(num - 1) + num
> 
> print(gettotal(100))
> 
> 
> """
> 总结：
>  优点：代码实现简单
>  缺点：过深的递归可能会造成栈溢出【StackOverflow】
> 
>  建议：在实际开发中，尽量不要使用递归【在Python中，设置了一个保护机制，只允许递归最多执行993次】
> """
> 
> ```

### 五、栈和队列

> 【面试题：栈和队列的区别和联系】
>
> 栈：Stack,是限定在表的一端进行插入和删除操作的线性表【抽象成一个开口向上的容器】
>
> 队列：Queue,是限定在表的一端进行插入操作，在表的另外一端进行删除操作的线性表【抽象成一个水平放置的水管】
>
> 线性表：属于一种线性结构【容器】，可以包含有限的序列节点，其中插入数据和删除数据都有一定的规律
>
> 相同点：
>
> ​	a.都是线性表
>
> ​	b.二者的插入操作都是表尾进行的
>
> ​	c.二者都可以通过顺序结构和链式结构实现
>
> ​	d.二者在实现插入和删除操作时，时间复杂度和空间复杂度是相同的【工作效率相同】
>
> 不同点：
>
> ​	a.删除的位置不同：栈的删除在表尾进行，队列的删除在表头进行
>
> ​	b.使用场景不同：
>
> ​		栈：Python中的基本语法【表达式的求值和转换，函数的定义和调用】
>
> ​		队列：计算机中各种资源的分配【系统】
>
> ​	c.工作原理不同：
>
> ​		栈：先进后出，后进先出
>
> ​		队列：先进先出，后进后出

#### 1.栈

> ```Python
> stack = []
> print(stack)
> 
> #入栈【向栈中添加数据】:append
> stack.append(11)
> print(stack)
> stack.append(22)
> print(stack)
> stack.append(33)
> print(stack)
> stack.append(44)
> print(stack)
> 
> 
> #出栈【从栈中删除数据】:pop
> stack.pop()
> print(stack)
> stack.pop()
> print(stack)
> stack.pop()
> print(stack)
> stack.pop()
> print(stack)
> 
> ```

#### 2.队列

> ```Python
> from collections import  deque
> 
> queue = deque()
> print(queue)
> 
> #入队【向队列中添加数据】：append
> queue.append(11)
> print(queue)
> queue.append(22)
> print(queue)
> queue.append(33)
> print(queue)
> queue.append(44)
> print(queue)
> 
> 
> #出队【从队列中删除数据】；popleft/pop
> queue.popleft()
> print(queue)
> queue.popleft()
> print(queue)
> queue.popleft()
> print(queue)
> queue.popleft()
> print(queue)
> 
> ```

### 六、目录遍历

> ```Python
> import  os
> 
> path = r"C:\Users\Administrator\Desktop\XA-Python1904"
> 
> #1.listdir,列出指定目录下所有的内容【文件或者文件夹】，返回一个列表,列表中的元素为文件或者文件夹的名称
> list1 = os.listdir(path)
> print(list1)
> 
> 
> #2.join,根据父路径和当前文件或者文件夹的名称拼接路径
> path1 = path + "\\" + "Day2Code"
> print(path1)
> 
> path2 = os.path.join(path,"Day2Code")
> print(path2)
> 
> #3.isfile/isdir:判断指定的路径是否是文件或者文件夹
> result = os.path.isfile(path2)
> print(result)
> 
> result = os.path.isdir(path2)
> print(result)
> 
> 
> ```

#### 1.递归遍历目录

> ```Python
> import  os
> 
> #递归遍历
> def getFile(path):
>  if os.path.isfile(path):
>      print("文件：",path)
>      return
> 
>  #说明path是一个文件夹【目录】
>  fileList = os.listdir(path)
> 
>  #遍历列表，拼接每个完整的路径
>  for fileName in fileList:
>      #拼接
>      filePath = os.path.join(path,fileName)
> 
>      if os.path.isdir(filePath):
>          print("目录：", filePath)
> 
>          #使用递归
>          getFile(filePath)
>      else:
>          print("文件：",filePath)
> 
> if __name__ == "__main__":
>  path = r"C:\Users\Administrator\Desktop\XA-Python1904"
>  getFile(path)
> 
> ```

#### 2.使用栈遍历目录【深度优先遍历】

> ```Python
> #使用栈遍历
> import  os
> #思路：定义一个空栈，如果路径是目录，则添加到栈中，如果是文件，则直接打印
> 
> 
> def getFile(path):
>  #定义一个空栈
>  stack = []
> 
>  #判断path是否是文件
>  if os.path.isfile(path):
>      print("文件：",path)
>      return
> 
>  #将path添加到栈中
>  stack.append(path)
> 
>  #处理栈，是一个循环的过程，循环的条件为：栈不为空
>  while len(stack) != 0:
>      print(stack)
>      dirpath = stack.pop()
> 
>      #获取初始路径下所有的内容
>      fileList = os.listdir(dirpath)
> 
>      #遍历，拼接路径
>      for fileName in fileList:
>          filePath = os.path.join(dirpath,fileName)
> 
>          if os.path.isdir(filePath):
>              #如果是目录，则添加到栈中
>              stack.append(filePath)
>          else:
>              print("文件：",filePath)
> 
> 
> if __name__ == "__main__":
>  path = r"C:\Users\Administrator\Desktop\XA-Python1904"
>  getFile(path)
> 
> ```

#### 3.使用队列遍历目录【广度优先遍历】

> ```Python
> #使用队列遍历
> import  os
> from collections import  deque
> 
> def getFile(path):
>  queue = deque()
> 
>  #判断path是否是文件
>  if os.path.isfile(path):
>      print("文件：",path)
>      return
> 
>  #将path添加到队列中
>  queue.append(path)
> 
>  #处理栈，是一个循环的过程，循环的条件为：栈不为空
>  while len(queue) != 0:
>      print(queue)
>      dirpath = queue.popleft()
> 
>      #获取初始路径下所有的内容
>      fileList = os.listdir(dirpath)
> 
>      #遍历，拼接路径
>      for fileName in fileList:
>          filePath = os.path.join(dirpath,fileName)
> 
>          if os.path.isdir(filePath):
>              #如果是目录，则添加到栈中
>              queue.append(filePath)
>          else:
>              print("文件：",filePath)
> 
> 
> if __name__ == "__main__":
>  path = r"C:\Users\Administrator\Desktop\XA-Python1904"
>  getFile(path)
> 
> ```

# Day11

### 一、上堂回顾

#### 1.默写题目

> 1.书写装饰器，使得可以对任何函数增加新功能
>
> ```Python
> def wrapper(f):
> def inner(*args,**kwargs):
>  f(*args,**kwargs)
>  
>  print()
>  
> return inner
> 
> @wrapper
> def check():
> pass
> 
> check()
> ```
>
> 2.使用至少三种方式生成列表[1,4,9,16,25]
>
> ```Python
> #方式一
> result1 = [i ** 2 for i in range(1,6)]
> 
> #方式二
> result2 = list((i ** 2 for i in range(1,6)))
> 
> #方式三
> result3 = list(map(lambda x :x ** 2,range(1,6)))
> ```
>
> 3.简述栈和队列的相同点和不同点【面试题】
>
> ```Python
> """
> 相同点：
> 	a.都是线性结构
> 	b.都可以进行删除和插入的操作
> 	c.插入操作都是在表尾进行的
> 	d.时间复杂度和空间复杂度是相同的
> 不同点：
> 	a.栈在表尾删除，队列在表头或者表尾都可以删除
> 	b.栈主要应用于基本语法【变量，函数等】，队列管理的计算机的资源分配
> 	c.特点：栈：先进后出，后进先出，队列：先进先出，后进后出
> """
> ```

#### 2.知识点回顾

> 1.装饰器
>
> 2.高阶函数
>
> ​	map,reduce,filter【True】，sorted
>
> 3.递归

### 二、模块

#### 1.包

> ```
> 初期理解为一个文件夹
> 
> 包是一种管理Python模块命名空间的一个工具，采用“点语法”形式
> 
> 说明：在一个文件夹下定义一个命名为__init__.py文件，该文件夹才被称为包，目前，__init__.py中不需要书写任何内容，在后期的项目开发中，会在其中添加项目的配置信息，在当前，仅仅为了标记当前目录是一个包
> 
> ```

#### 2.系统模块

##### 2.1time

> 时间间隔：秒
>
> 时间戳：自从1970.1.1 00:00：00开始经历的秒数
>
> UTC:格林威治事件，世界标准时间，在中国为UTC+8
>
> DST:夏令时格式，0表示正常格式，1为夏令时格式，-1表示按照自定义的格式
>
> 时间的表示形式：
>
> ​	a.时间戳
>
> ​	b.时间元组
>
> ​	c.时间字符串格式
>
> ```Python
> import  time
> 
> #1.获取当前时间的时间戳
> t1 = time.time()
> print(t1)
> 
> #2.获取UTC,为元组形式
> t2 = time.gmtime()
> print(t2)
> 
> #3.获取本地时间,为元组形式
> t3 = time.localtime()
> print(t3)
> 
> #4.将时间元组形式转换为时间戳
> t4 = time.mktime(t3)
> print(t4)
> 
> #5.将时间戳形式转换为时间字符串形式
> #5.1默认格式
> t5 = time.ctime(t1)
> print(t5)
> 
> #6.将时间元组转化为时间字符串形式
> #6.1默认格式
> t61 = time.asctime(t3)
> print(t61)
> 
> #6.2自定义格式
> """
> %Y:年
> %m:月
> %d:日
> %H:时，24小时制
> %M:分
> %S;秒
> """
> t62 = time.strftime("%Y-%m-%d %H:%M:%S",t3)
> print(t62)
> 
> #7.将字符串转换为元组
> #注意：将时间字符串转化为元组形式，注意字符串和解析格式的匹配，否则解析失败
> str1 = "2019-08-06 15:05:19"
> t7 = time.strptime(str1,"%Y-%m-%d %H:%M:%S")
> print(t7)
> 
> 
> #8.休眠
> #当执行了sleep，会让程序进入休眠状态【阻塞】，当指定的时间完成之后，会自动解除阻塞，继续执行后面的代码
> #使用场景：应用在多线程和多进程中
> time.sleep(5)
> 
> print("over")
> 
> #9.clock()，和time（）类似，
> #time():获取当前设备的时间
> #clock():获取cpu的时间，比time更加准确，用来衡量不同程序的耗时情况
> print(time.clock())
> 
> #练习
> #1.书写一个装饰器，统计任意一个函数的执行时间
> def wrapper(f):
>  def inner(*args,**kwargs):
>      start = time.time()
>      f(*args,**kwargs)
>      end = time.time()
> 
>      print("该函数的执行时间为：%f" % (end - start))
> 
>  return inner
> 
> @wrapper
> def check():
>  for i in range(100000):
>      pass
> check()
> 
> 
> #2.已知时间的字符串"2018-8-1",计算5天之后的时间
> timeStr = "2018-8-1"
> #方式一
> timeList = timeStr.split("-")
> day = int(timeList[-1]) + 5
> newtime = "%s-%.2d-%.2d" % (timeList[0],int(timeList[1]),day)
> print(newtime)
> 
> 
> #方式二
> timeStr = "2018-8-1"
> #1.将时间字符串转化为时间元组
> time1 = time.strptime(timeStr,"%Y-%m-%d")
> #2.将时间元组格式转换为时间戳
> time2 = time.mktime(time1)
> #3.进行加法运算，time2 + 5天的秒数
> time3 = time2 + 5 * 24 * 3600
> #4.将时间戳转换为时间元组
> time4 = time.localtime(time3)
> #5.将时间元组转换为时间字符串
> time5 =time.strftime("%Y-%m-%d",time4)
> print(time5)
> 
> #不同形式的时间之间的转换时间字符串《-----》时间元组《-----》时间戳
> 
> result = time.strftime("%Y-%m-%d",time.localtime(time.mktime(time.strptime(timeStr,"%Y-%m-%d")) + 5 * 24 * 3600))
> print(result)
> ```

##### 2.2datetime

> 在time模块的基础上做了封装，提供了更多的功能
>
> ```Python
> import  datetime
> 
> #1。获取的是当前时间，返回的是日期的对象，并不是一个字符串
> d1 = datetime.datetime.now()
> print(d1)
> print(type(d1))
> 
> #2.将一个指定的时间转换为日期对象
> d2 = datetime.datetime(2018,9,18,3,4,5)
> print(d2)
> 
> #3.将日期对象转换为字符串
> d3 = d1.strftime("%Y-%m-%d")
> print(d3)
> print(type(d3))
> 
> #4.将时间字符串转化为日期对象
> d4 = datetime.datetime.strptime("2019-08-06","%Y-%m-%d")
> print(d4)
> print(type(d4))
> 
> #5.两个日期对象之间可以进行减法运算
> date1 = datetime.datetime(2018,9,18,3,4,5)
> date2 = datetime.datetime(2018,9,20,3,6,20)
> date3 = date2 - date1
> print(date3)
> print(type(date3))
> 
> print(date3.days)
> print(date3.seconds)
> 
> #print(date1 + date2)  #TypeError: unsupported operand type(s) for +: 'datetime.datetime' and 'datetime.datetime'
> ```

##### 2.3calendar

> ```Python
> import  calendar
> 
> print(calendar.month(2019,8))
> 
> print(calendar.calendar(2019))
> 
> print(calendar.isleap(2000))
> 
> print(calendar.monthcalendar(2019,8))
> 
> print(calendar.leapdays(2000,2020))
> 
> ```

##### 2.4os

> ```Python
> import  os
> 
> #一、属性
> #获取操作系统的名称
> #nt---->Windows,posix---->Linux、Mac os
> print(os.name)
> 
> #获取当前操作系统中的环境变量
> print(os.environ)
> 
> #获取当前的工作路径，.代表当前路径，..代表上一级路径
> #获取相对路径
> print(os.curdir)
> #获取绝对路径
> print(os.getcwd())  #C:\Users\Administrator\Desktop\XA-Python1904\Day11Code
> 
> 
> #二、os下函数
> #获取指定路径下的所有内容        *******
> print(os.listdir(r"C:\Users\Administrator\Desktop\XA-Python1904\Day11Code"))
> 
> #创建目录
> #os.mkdir(r"C:\Users\Administrator\Desktop\aaa")
> #os.mkdir(r"check")
> 
> #删除目录
> #os.rmdir(r"check")
> #os.rmdir(r"C:\Users\Administrator\Desktop\aaa")
> 
> #获取文件的属性
> #print(os.stat(r"a1.txt"))
> 
> #对文件或者文件夹重命名
> #rename(old,new)
> #os.rename(r"a1.txt","file1.txt")
> #os.rename(r"aaa","newaaa")
> 
> 
> #删除普通文件
> #os.remove(r"file1.txt")
> 
> #运行shell命令
> #os.system("write")  #打开写字板
> #os.system("mspaint")  #打开画图板
> #os.system("msconfig")
> #os.system("notepad")
> 
> #os.system("shutdown - s -t 500")  #关机
> 
> 
> #三、os.path下的函数
> #拼接路径      *******
> p1 = os.path.join(r"C:\Users\Administrator\Desktop\XA-Python1904","Day11")
> print(p1)
> 
> #拆分路径
> #结果为一个元组（父路径，子路径）
> r0 = os.path.split(r"C:\Users\Administrator\Desktop\XA-Python1904\Day11")
> print(r0)
> #结果为一个元组（路径，扩展名），如果路径是一个目录，则第1个元素为""；如果路径是一个文件，则第1个元素为扩展名   *******
> r0 = os.path.splitext(r"C:\Users\Administrator\Desktop\XA-Python1904\Day11Code\dog.jpg")
> print(r0)
> 
> #判断路径是否存在     *******
> print(os.path.exists(r"C:\Users\Administrator\Desktop\XA-Python1903"))
> 
> #判断路径是文件还是文件夹      *******
> print(os.path.isfile(r"C:\Users\Administrator\Desktop\XA-Python1904"))
> print(os.path.isdir(r"C:\Users\Administrator\Desktop\XA-Python1904"))
> 
> #获取一个文件的大小,返回的结果为指定文件中的字节数     *******
> print(os.path.getsize(r"C:\Users\Administrator\Desktop\XA-Python1904\Day11Code\dog.jpg"))
> 
> #获取路径
> print(os.path.dirname(r"C:\Users\Administrator\Desktop\XA-Python1904"))
> print(os.path.basename(r"C:\Users\Administrator\Desktop\XA-Python1904"))
> 
> 
> #练习：封装函数，获取某个路径下所有py文件
> def getpyfile(path):
>  #判断
>  if not os.path.exists(path):
>      print("路径不存在")
>      return
> 
>  if os.path.isfile(path):
>      print("该路径是一个文件")
>      return
> 
>  #获取路径下的所有的内容
>  fileList = os.listdir(path)
> 
>  #遍历
>  for filename in fileList:
>      #拼接
>      filepath = os.path.join(path,filename)
> 
>      if os.path.isfile(filepath):
>          if os.path.splitext(filepath)[1] == ".py":
>              print("py文件：",filepath)
> 
> 
> def getpyfile(path):
>  # 判断
>  if not os.path.exists(path):
>      print("路径不存在")
>      return
> 
>  if os.path.isfile(path):
>      print("该路径是一个文件")
>      return
> 
>      # 获取路径下的所有的内容
>  fileList = os.listdir(path)
> 
>  # 遍历
>  for filename in fileList:
>      # 拼接
>      filepath = os.path.join(path, filename)
> 
>      if os.path.isfile(filepath):
>          if filepath.endswith(".py"):
>              print("py文件：", filepath)
> 
>      else:
>          #递归
>          getpyfile(filepath)
> ```

##### 2.5logging

> 追踪日志
>
> 日志：通过log的分析，可以了解软件存在的问题或者运行的状况，分析用户的行为
>
> 将log分成多个不同的级别，分析得到对应的软件的健康状态，、及时发现并快速定位问题的地方然后解决
>
> 作用：
>
> ​	a.程序调试
>
> ​	b.了解程序的运行状态
>
> ​	c.程序故障分析和问题定位
>
> 日志等级：
>
> ​	debug---->info----->notice----->warning---->error---->critical----->alter----->emergency
>
> 日志内容：
>
> ​	事件发生时间
>
> ​	事件发生位置
>
> ​	事件的严重程度----》级别
>
> ​	事件内容
>
> ```Python
> import  logging
> 
> logging.debug("这是一个debug log")
> logging.info("这是一个info log")
> logging.warning("这是一个warning log")
> logging.error("这是一个error log")
> logging.critical("这是一个critical log")
> 
> 
> """
> 问题说明：
>  1.为什么debug和info没有信息输出到控制台
>      系统设置了默认的级别，为warning，只有当前应用出现warning以及大于warnning的日志才会输出结果
>  2.ERROR:root:这是一个error log分别表示什么含义?
>      日志级别：日志器名称：日志内容
> 
>      如果要修改格式，可以自定义，只需要修改Basic_format
> """
> 
> ```
>
> ```Python
> import  logging
> 
> #自定义日志格式
> LOG_FORMAT = "%(asctime)s - %(levelname)s - %(message)s"
> # logging.basicConfig(level=logging.DEBUG)
> 
> #设置日期格式
> date_format = "%m/%d/%Y %H:%M:%S"
> logging.basicConfig(filename="my.log",level=logging.DEBUG,format=LOG_FORMAT,datefmt=date_format)
> 
> 
> #不同级别的日志监测
> logging.debug("这是一个debug log")
> logging.info("这是一个info log")
> logging.warning("这是一个warning log")
> logging.error("这是一个error log")
> logging.critical("这是一个critical log")
> 
> 
> 
> 
> ```

##### 2.6sys

> ```Python
> import sys
> 
> #获取当前的文件路径
> print(sys.argv)
> print(sys.argv[0])
> 
> #获取当前工程以及对应的环境的路径
> print(sys.path)
> 
> #获取平台名称
> print(sys.platform)   #win32
> 
> #print默认输出到控制台
> #print(sys.stdout)
> 
> print("hello")
> print("hfjhfg",file=sys.stdout)
> 
> print("1456124",file=open("file1.txt","w"))
> 
> 
> ```

##### 2.7hashlib

> MD5,SHA1
>
> ```Python
> import  hashlib
> 
> """
> Python中的hashlib中提供了常见的摘要算法【MD5,SHA1等】
> 摘要算法：哈希算法，散列算法，通过一个函数，把任意长度的数据转换为长度固定的数据，一般使用16进制的字符串表示
>       通过函数f()对任意长度的数据data计算出固定长度的摘要digest,目的是为了监测原始数据是否被人篡改过
> """
> 
> #MD5
> md5 = hashlib.md5()
> md5.update("this is a test".encode("utf-8"))
> print(md5.hexdigest())
> #print("中文23432this is a test".encode("utf-8"))
> 
> 
> #SHA1
> sha1 = hashlib.sha1()
> sha1.update("this is a test".encode("utf-8"))
> print(sha1.hexdigest())
> 
> """
> MD5加密的特点：
>  1.不同长度的数据，md5的值的长度有可能相等
>  2.从原始数据计算md5的值速度很快，hashlib.md5()
>  3.已知一个原始数据和对应的md5字符串，想要找到一个具有相同md5值的原始数据是很困难的，md5的加密是不可逆的
>  4.如果对原始数据做了任何修改，不管数据量多大，生成的md5的结果完全不同
> """
> 
> ```

#### 3.自定义模块

##### 3.1import  xxx

##### 3.2import   xxx   as   xxxx

##### 3.3from  xxx import xxx

> ```Python
> """
> 1.实际上，每个py文件都是一个模块
> 2.在一个模块中访问另外一个模块中的内容，必须想办法让两个模块之间产生联系【import加载】
> 3.import  模块
>  说明：模块的构成：包名.模块名
>  import是将指定文件中的内容从头到尾加载到内存中
> 4.在实际项目开开发中，一般使用相对路径，在模块中，默认的参照路径是当前的工程
> 
> 5.在导入模块的时候，其中的   .   代表的是目录的层级关系
> """
> 
> #一、import xxxx
> """
> import aaa.module
> import bbb.module
> #import  ccc.c1.module
> #注意：如果包或者文件夹的层级关系比较复杂的时候，可以修改默认的参照路径，
> # 选中指定文件夹---》右键，Mark as Directory----》source root,则可以简化模块的导入
> import module
> 
> #调用指定模块中的函数，则需要指明函数的来源
> aaa.module.func()
> bbb.module.func()
> #ccc.c1.module.func()
> module.func()
> """
> 
> """
> 总结：
>  1.缺点：如果一个模块中存在很多函数，每个函数的调用都必须标注该函数的来源，使得代码比较繁琐
>          import会一次性将指定模块中的所有的内容全部加载，如果只需要使用其中的一部分内容，则会造成内存空间的浪费
>  2.优点：在不同的模块中出现同名的函数，则调用的时候，相互之间没有任何影响
> """
> 
> 
> #二、import  xxxx as  xxx
> #注意：as关键字的作用是为了给前面指定的模块起别名，调用指定模块中的函数，就可以用别名调用
> #别名尽量简单，但是尽量做到见名知意
> """
> import  aaa.module as a
> import  bbb.module as b
> import  ccc.c1.module as c
> 
> a.func()
> b.func()
> c.func()
> """
> 
> """
> 总结：
>  1.缺点：如果一个模块中存在很多函数，每个函数的调用都必须标注该函数的来源，相比较于import xxx显得简单
>  2.优点：在不同的模块中出现同名的函数，则调用的时候，相互之间没有任何影响
> """
> 
> #三、from 模块 import 变量名或者类名
> #3.1
> #注意:如果需要导入多个变量或者类，使用逗号隔开即可
> """
> from bbb.module import func
> from  aaa.module import func,func1,num1
> 
> func1()
> print(num1)
> 
> #注意：覆盖问题
> def func():
>  print("textDemo")
> func()
> """
> 
> #3.2from xxx import *
> #如果采用from的方式导入，但是函数或者变量比较多的情况下，则使用*代替所有
> """
> from aaa.module import *
> #等价于import aaa.module
> 
> func()
> func1()
> func3()
> print(num1)
> """
> 
> """
> 总结：
>  1.缺点：
>      当不同的模块中出现了同名的函数，则调用函数或者访问变量的时候，后import谁，则访问谁【后出现的会将先出现的覆盖掉】
>  2.优点：
>      导入变量或者类的时候，可以选择性的导入，避免不使用的变量造成内存空间的浪费
>      调用函数或者访问变量的时候，不需要标明函数或者变量的来源
> """
> 
> #四、模块的工作原理
> import ccc.c1.module
> # import ccc.c1.module
> # import ccc.c1.module
> # import ccc.c1.module
> 
> """
> 一旦使用import加载一个指定的模块，在计算机中生成和该模块对应的一个.pyc文件，
> 当后期再import则加载的不再是源文件，直接加载.pyc文件，
> 这种现象被称为单例【在整个工程中只有一个实体存在，不管在工程的哪个模块中获取，获取的都是同一个】
> """
> 
> ```

#### 4.第三方模块

> pip
>
> python -m pip install --upgrade pip
>
> pip install setuptools
>
> ```Python
> #1.图像缩放
> """
> from PIL import  Image
> 
> #打开图像
> #绝对路径：\    相对路径：/
> im = Image.open("dog.jpg")
> 
> #获取原图像的尺寸
> w,h = im.size
> print("图像的原尺寸为,宽：%d,高：%d" % (w,h))
> 
> #缩放图片,传参的时候传递的是一个元组（宽，高）
> im.thumbnail((w // 2,h // 2))
> print("缩放之后的图片尺寸为,宽：%d,高：%d" % (w // 2,h // 2))
> 
> #保存缩放之后的新的图片
> im.save("newdog.jpg","jpeg")
> """
> 
> #2.模糊处理
> from PIL import  Image,ImageFilter
> 
> #打开图片
> im = Image.open("dog.jpg")
> 
> #应用模糊滤镜
> im2 = im.filter(ImageFilter.BLUR)
> 
> #保存图片
> im2.save("blurdog.jpg","jpeg")
> 
> ```
>
> ```Python
> #3.生成图形验证码
> from PIL import  Image,ImageDraw,ImageFont,ImageFilter
> import  random
> 
> #随机字母
> def randomchar():
>  return  chr(random.randint(65,90))
> 
> #随机颜色1
> def randomcolor1():
>  return (random.randint(50,255),random.randint(50,255),random.randint(50,255))
> 
> #随机颜色2
> def randomcolor2():
>  return (random.randint(25,127),random.randint(25,127),random.randint(25,127))
> 
> 
> if __name__ == "__main__":
>  width = 240
>  height = 60
> 
>  #创建图片
>  image = Image.new("RGB",(width,height),(255,255,255))
> 
>  #创建字体
>  #参数：本地字体的文件路径   字体大小
>  font = ImageFont.truetype(r"C:\Windows\Fonts\Arial.ttf",36)
> 
>  #创建draw【绘制】
>  draw = ImageDraw.Draw(image)
> 
>  #填充每个像素
>  for x in range(width):
>      for y in range(height):
>          #填充像素点
>          draw.point((x,y),fill=randomcolor1())
> 
>  #绘制文字
>  for i in range(4):
>      draw.text((60 * i + 10,10),randomchar(),font=font,fill=randomcolor2())
> 
>  #模糊处理
>  image = image.filter(ImageFilter.BLUR)
> 
>  #保存图片
>  image.save("imagecode.jpg","jpeg")
> 
> ```
>
> 

# Day12

### 一、上堂回顾

#### 1.默写题目

> 1.导入模块有哪几种方式，分别有什么特点【面试题】
>
> ```Python
> """
> 1.import xxx
> 2.import xxx   as   xxx
> 3.from xxx import  变量、函数或者类
> 4.from xxx import *
> 
> 特点：
> 	1.import：将一个指定模块中所有的内容加载，可能会造成内存空间的浪费
> 	2.import...as:可以给一个层级关系比较复杂的模块其别名，简化函数，变量以及类的访问
> 	3.from...import:可以选择性的导入需要使用的内容，从一定程度上可以节约资源
> """
> ```
>
> 2.封装函数，输出一个指定路径下的所有文件
>
> ```Python
> import os
> def getAllFile(path):
> if os.path.exists(path):
>  
>  if os.path.isdir(path):
>    
>    #获取
>    list1 = os.listdir(path)
>    
>    #遍历
>    for name in list1:
>      #拼接
>      subpath = os.path.join(path,name)
>      if os.path.isfile(subpath):
>        print("文件：",subpath)  
>  else:
>    print("该路径是一个文件："，path) 
> else:
>  print("该路径不存在")
> ```

#### 2.知识点回顾

> 1.自定义模块
>
> 2.第三方模块
>
> ​	pip  install xxx:安装第三方模块
>
> ​	pip list:列出所有的第三方模块
>
> ​	pip freeze:；列出最新安装的第三方模块
>
> ​	pip -V:查看pip的版本
>
> 3.系统模块
>
> ​	time:三种时间表示形式的转化
>
> ​	datetime:日期的对象之间可以进行减法运算
>
> ​	os:listdir,join,split/splitext,isfile/isdir,exists，getsize
>
> ​	logging:日志的作用
>
> ​	hashlib:md5算法的特点

### 二、面向对象

#### 1.案例

> 一切皆对象
>
> 案例一：我今天中午想吃大盘鸡
>
> 面向过程							面向对象
>
> 1.我需要取买菜						1.让一个喜欢跑腿的人去买菜和买鸡
>
> 2.我需要去买鸡						2.让一个勤快的人洗菜
>
> 3.我需要洗菜，杀鸡					3.让一个胆大的人杀鸡
>
> 4.我需要做饭							4.让一个厨师做饭
>
> 5.我吃掉								5.我吃掉
>
> 案例二：小明是一个电脑小白，想要组装一台电脑
>
> 面向过程							面向对象
>
> 1.小明补充电脑知识					1.委托一个懂电脑的人购买零件
>
> 2.小明购买零件						2.委托一个快递员将零件运回家里
>
> 3.小明将零件运回家里					3.委托一个动手能力里强的人组装电脑
>
> 4.小明组装							4.小明打开玩连连看
>
> 5.小明打开玩连连看

#### 2.面向对象和面向过程

> process，处理
>
> 1》面向过程：
>
> ​	在生活案例中：是一种解决问题的思维方式，在思考问题的时候，侧重于指定的问题是怎样一步一步解决的，然后亲力亲为的去解决问题
>
> ​	在程序中:
>
> ​		代码从上往下依次执行
>
> ​		各个模块之间的关系尽可能简单，在功能上独立
>
> ​		程序的执行流程在写程序时已经决定
>
> ​		分析出解决问题需要的步骤，然后使用函数封装单独的功能，使用的时候按照需求的顺序将各个函数依次的调用
>
> ​		程序员充当的是执行者的角色
>
> 2》面向对象
>
> ​	在生活案例中：也是一种解决问题的思维方式，在思考问题的时候，侧重于能够找到一个具有特殊功能的个体，然后委托该个体去帮忙完成某件事情，这个个体被称为对象
>
> ​	在程序中：
>
> ​		对同类对象抽取出其共性，形成类
>
> ​		程序的流程由用户决定
>
> ​		可以将复杂的问题简单化，将程序员由原来的执行者转换成了指挥者
>
> ​		使用面向对象的思想进行开发，先要找到一个具有特殊功能的个体，如果对象存在，则直接使用，如果对象不存在，则先创建再使用
>
> ​		注意：面向对象只是一种思想，并不是一门编程语言，使用面向对象思想的语言：Java，Python,OC,Javascript
>
> 面向对象和面向过程的优缺点
>
> 面向过程：
>
> ​	优点：性能比面向对象高，开销比较大，比较消耗资源，如：单片机和嵌入式开发使用的是面向过程
>
> ​	缺点;不易于维护，不易于复用，不易于扩展
>
> 面向对象：
>
> ​	优点：易于维护，易于复用，易于扩展【由于面向对象有封装，继承和多态的特性，可以设计出低耦合的系统，使得系统更加灵活，更加易于维护】
>
> ​	缺点：性能比面向过程低

### 三、类和对象

#### 1.概念

> 类和对象是面向对象的核心
>
> 类：对多个具有共同特征的个体进行抽取，形成一个类
>
> 对象：在一个类中，一个具有特殊功能的具体存在的个体，被称为实例【instance】
>
> 两者之间的关系：类是抽象的【用来描述某一类对象的共同特征】，对象是具体的【是类的具体的体现】
>
> 问题：先有对象还是先有类：
>
> 在程序中，一般先有类，然后通过类创建对象
>
> ```Python
> num = 10
> print(type(num))   #<class 'int'>
> s1 = "hello"
> print(type(s1))  #<class 'str'>
> 
> #实际上，int和str就是系统的类
> ```
>
> 帮助理解：类也是一种数据类型，只不过自定义的，跟之前的int，str，float,bool等类似，所以，创建一个对象其实就是定义一个指定类的变量

#### 2.类的定义

> 语法：
>
> ​	class   类名():
>
> ​		类体
>
> 说明：
>
> ​	a.class是专门用来定义类的关键字
>
> ​	b.类名：只要是一个合法的标识符即可，但是，尽量遵循大驼峰【每个单词的首字母都需要大写】    ,类似NameError/ValueError/Iterable/ImageDraw/ImageFilter等都是系统的类
>
> ​	c.()：Python2.x中的类被称为经典类，()可以省略;Python3.x中的类称为新式类，()尽量不要省略
>
> ​	d.类的定义包含两部分：类的声明和实现
>
> ​	e.类体：也需要通过缩进区分，其中可以定义变量，也可以定义函数，换句话说，类体中包含的内容两部分：对类的特征的描述和对类的行为的描述
>
> ```Python
> """
> 语法：
> 
> 	class   类名():
> 
> 		类体
> """
> #类的定义
> #类的声明
> class MyClass():
>  #类的实现
>  pass
> 
> 
> class MyClass1():
>  pass
> 
> #总结：在同一个py文件中可以定义多个类，但是，为了提高代码的可读性，结合模块的使用，
>  # 一般情况下，在一个py文件中定义一个类
> ```

#### 3.类的设计

> 三要素：
>
> ​	事物名称-----》类名，如：Person
>
> ​	特征---------》变量，如：name，age,height等  【名词】
>
> ​	行为---------》函数/方法，如：打游戏，打篮球，跑步等  【动词】	

### 四、类的成员

#### 1.类中成员的定义

> 一个类用来描述某一类对象的特征
>
> 类中对象的特征和行为被称为成员
>
> 成员变量：定义在类中的变量，也被称为属性
>
> 成员函数：定义在类中的函数
>
> ```Python
> #定义类
> #1.事物的名称：类名
> class Person():
>  #类的成员
>  #2.事物的特征：成员变量/属性
>  name = 'abc'
>  age = 18
> 
> 
>  #3.事物的行为：成员函数
>  """
>  成员函数和普通函数之间的区别：
> 
>  self:自己
> 
>  注意：self只要是一个合法的标识符即可，self不是关键字，一般出现在成员函数形参列表的第一位
>  但是，一般使用self，主要和其他语言靠拢，self代表的是当前的对象【实例】
>  """
>  def eat(self,food):
>      print("eating", food)
> 
>  def walk(self):
>      print("walking")
> ```

#### 2.对象的创建

> 创建对象的过程也被称为对象实例化的过程
>
> 语法：
>
> ​	变量名【对象名】  = 类名()
>
> 说明：
>
> ​	a.目前的情况下，()是空的，但是()不能省略
>
> ​	b.变量指向一个真正的对象
>
> ```Python
> #一、定义类
> #二、定义类中的成员
> #1.事物的名称：类名
> class Person():
>  #类的成员
>  #2.事物的特征：成员变量/属性
>  name = 'abc'
>  age = 18
> 
>  #3.事物的行为：成员函数
>  """
>  成员函数和普通函数之间的区别：
> 
>  self:自己
> 
>  注意：self只要是一个合法的标识符即可，self不是关键字，一般出现在成员函数形参列表的第一位
>  但是，一般使用self，主要是和其他语言靠拢，self代表的是当前的对象【实例】
>  """
>  def eat(self,food):
>      print("eating", food)
> 
>  def walk(self):
>      print("walking")
> 
> #三、创建对象
> #注意1：定义一个类之后，通过该类可以创建无数个对象
> p1 = Person()
> p2 = Person()
> #注意2：Person()一旦出现一次，则表示创建一个新的对象，在内存中开辟一份新的空间
> print(p1 is p2)
> 
> num1 = 10
> num2 = 10
> print(num1 is num2)  #True
> 
> #注意3：对象存储在内存中，p1 = Person()，p1被存储在栈中，Person()真正的对象被存储在堆中
> ```

#### 3.类中成员的访问

> 语法：对象.变量或者函数
>
> ```Python
> #一、定义类
> #二、定义类中的成员
> #1.事物的名称：类名
> class Person():
>  #类的成员
>  #2.事物的特征：成员变量/属性
>  name = 'abc'
>  age = 18
> 
>  #3.事物的行为：成员函数
>  """
>  成员函数和普通函数之间的区别：
> 
>  self:自己
> 
>  注意：self只要是一个合法的标识符即可，self不是关键字，一般出现在成员函数形参列表的第一位
>  但是，一般使用self，主要是和其他语言靠拢，self代表的是当前的对象【实例】
> 
>  当前的对象:哪个对象调用该函数，则self代表的就是谁
>            调用成员函数的时候，self不需要手动传参，由系统自动将当前的对象传参
>  """
>  def eat(self,food):
>      print("self的地址为;",id(self))
>      print("eating", food)
> 
>  def walk(self):
>      print("walking")
> 
> #三、创建对象
> #注意1：定义一个类之后，通过该类可以创建无数个对象
> p1 = Person()
> p2 = Person()
> #注意2：Person()一旦出现一次，则表示创建一个新的对象，在内存中开辟一份新的空间
> print(p1 is p2)
> 
> num1 = 10
> num2 = 10
> print(num1 is num2)  #True
> 
> #注意3：对象存储在内存中，p1 = Person()，p1被存储在栈中，Person()真正的对象被存储在堆中
> 
> #四、类中的成员的访问
> #1.访问成员变量
> per1 = Person()
> #获取
> print(per1.name)
> print(per1.age)
> #修改
> per1.name = "小姐姐"
> per1.age = 20
> print(per1.name)
> print(per1.age)
> 
> #2.访问成员函数
> print("per1的id为：",id(per1))
> per1.eat("apple")
> per1.walk()
> 
> per2 = Person()
> print("per2的id为：",id(per2))
> per2.eat("aaa")
> 
> #注意：如果将变量直接定义在类中，则对象.变量 表示访问该变量，但是，对象.变量 = 值  则表示重新定义了一个新的变量
> print(per2.name)
> print(per2.age)
> ```
>
> ```Python
> class Person():
>  # name = "aaa"
>  # age = 10
>  pass
> 
> p1 = Person()
> # print(p1.name)
> # print(p1.age)
> 
> #对象属性的动态绑定
> p1.name = "zhangsan"
> p1.age = 18
> print(p1.name)
> print(p1.age)
> 
> p1.score = 100
> p1.num = 18
> p1.height = 172.0
> print(p1.score)
> print(p1.height)
> ```

#### 4.属性的动态绑定和限制绑定

> ```Python
> class Animal():
>  #2.限制属性的动态绑定
>  #注意3：当对动态绑定的属性做出限制之后，通过该类创建出来的对象只能绑定__slots__指定的属性
>  __slots__ = ("name","kind","color")
>  def eat(self):
>      print("eating")
> 
> 
> #1.给对象动态绑定属性
> a1 = Animal()
> #注意1：给一个对象动态的绑定属性，从理论来说，可以无限个属性的绑定
> a1.name = "大黄"
> a1.kind = "土狗"
> print(a1.name,a1.kind)
> 
> a2 = Animal()
> a2.name = "小白"
> a2.kind = "猫"
> print(a2.name,a2.kind)
> 
> #注意2：通过动态绑定的方式给不同的对象绑定同一个属性【属性名称重名】，这些属性指向不同的内存空间
> a1.name = "旺财"
> print(a2.name)
> 
> a3 = Animal()
> a3.name = "aaa"
> a3.name = "BBB"
> 
> 
> #
> a1.color = "red"
> a2.color = "black"
> a3.color = "blue"
> 
> 
> #注意4：一个对象绑定了属性【开辟了空间】，和其他的对象没有任何关系
> a4 = Animal()
> a4.name = "444"
> 
> a5 = Animal()
> #a5.name = "fag"
> #print(a5.name)   #AttributeError: name
> 
> ```

#### 5.案例一

> ```Python
> #测试文件
> """
> 情景：开学了，王老师让学生小花，小丽，小明做自我介绍
>  自我介绍的内容包含：姓名，年龄，爱好，来一段才艺展示
> 
> 
> 分类
> 老师类：
>  特征：姓名
>  行为：让。。。。
> 
> 学生类：
>  特征：姓名，年龄，爱好
>  行为：做自我介绍，来一段才艺展示
> """
> from practice01.teacher import Teacher
> from  practice01.student import Student
> 
> 
> #1.创建对象并绑定属性
> wang = Teacher()
> wang.name = "王老师"
> 
> xiaoming = Student()
> xiaoming.name = "小明"
> xiaoming.age = 18
> xiaoming.hobhy = "吹牛逼"
> 
> #2.程序员作为一个指挥者，指挥某个对象执行自己的行为
> wang.letStuIntroduce(xiaoming)
> 
> print("*" * 20)
> 
> xiaohua = Student()
> xiaohua.name = "小花"
> xiaohua.age = 16
> xiaohua.hobhy = "唱歌"
> wang.letStuIntroduce(xiaohua)
> 
> print("*" * 20)
> 
> xiaoli = Student()
> xiaoli.name = "小丽"
> xiaoli.age = 17
> xiaoli.hobhy = "跳舞"
> wang.letStuIntroduce(xiaoli)
> 
> ```
>
> ```Python
> #实体文件【类文件】
> 
> """
> 
> 学生类：
>  特征：姓名，年龄，爱好
>  行为：做自我介绍，来一段才艺展示
> """
> class Student():
>  __slots__ = ("name","age","hobhy")
> 
>  def introduce(self):
>      print("大家好，我是%s,今年%s,爱好：%s" % (self.name,self.age,self.hobhy))
> 
>  def sing(self):
>      print("娘子~~~~啊哈")
> 
>  def dance(self):
>      print("广场舞")
> 
>  def lie(self):
>      print("我家有几百头牛，几百头羊~~~~~")
> ```
>
> ```Python
> #实体文件【类文件】
> 
> """
> 老师类：
>  特征：姓名
>  行为：让xxx做自我介绍
> """
> class Teacher():
> 
>  __slots__ = ("name")
> 
>  #stu是一个学生的对象
>  def letStuIntroduce(self,stu):  #stu = xiaoming  = Student()
>      print(self.name + "让" + stu.name + "做自我介绍")
> 
>      #学生执行自己的行为
>      stu.introduce()
> 
>      if stu.name == "小花":
>          stu.sing()
>      elif stu.name == "小丽":
>          stu.dance()
>      else:
>          stu.lie()
> ```

### 五、构造函数和析构函数

#### 1.构造函数

> ```
> 很多类都倾向于将对象创建为有初始状态，Python提供了一个特殊的函数__init__,该函数被称为构造函数，也被称为构造器，主要用于创建对象并将对象的数据初始化
> 
> __init__调用的时机：当创建对象的第一个被自动调用的函数
> 
> 语法：
> 	def __init__(self,xx,xx,xx,.....):
> 		pass
> 		
> 说明：构造函数实际上仍然是一个成员函数，第一个参数为self
> 
> 注意：
> 	a.默认情况下，系统提供了一个无参的构造函数，该函数是隐式的，可以根据该构造函数创建一个无参的对象 p1 = Person()
> 
> ```
>
> ```Python
> #1.构造函数的调用时机
> class People1():
>  def __init__(self):
>      print("构造函数被调用了")
> 
> p1 = People1()
> #注意：创建对象的过程中被自动调用的函数
> 
> #2.有参的构造函数
> class People2():
>  def __init__(self,name,age):
>      #print(id(self))
>      #注意：一般情况下，有参的构造函数目的是为了定义属性，再给属性进行赋值
>      #print(n,a)
>      self.name = name
>      self.age = age
> 
>  def show(self):
>      print("showing")
> 
> #注意：当给类提供了有参的构造函数之后，系统无参的构造函数会被覆盖掉，使用构造函数，则必须严格按照要求进行传参
> p2 = People2("zhangsan",18)
> #print(id(p2))
> print(p2.name,p2.age)
> # p2.name = "jack"
> # print(p2.name)
> 
> p3 = People2("aaa",10)
> print(p3.name,p3.age)
> 
> p3.show()
> p3.show()
> p3.show()
> p3.show()
> 
> """
> 面试题：构造函数和普通成员函数之间的区别和联系：
>  区别：
>      1.构造函数的函数名是固定的，是__init__,普通成员函数的名可以自定义
>      2.构造函数是在创建对象的时候自动被调用，但是，普通成员函数必须手动调用
>      3.对于同一个对象而言，构造函数只被调用一次，但是，普通的成员函数可以被无限次调用
> 
>  联系：
>      1.遵循函数的基本用法，默认参数，关键字参数和不定长参数同样都适用
>      2.构造函数也是一个成员函数，形参列表的第一个参数都是self，代表的是当前对象
> """
> ```

#### 2.析构函数

> ```
> 和构造函数相反，当对象被销毁的时候自动调用的函数，被称为析构函数，Pyhon中提供了特殊函数__del__
> 
> 使用场景：对象即将被销毁的时候做的一些清理工作，比如：关闭文件，关闭数据库等
> 
> ```
>
> ```Python
> import  time
> 
> class Animal():
>  #构造函数
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
>      print("构造函数被调用了")
> 
>  #析构函数
>  def __del__(self):
>      print("析构函数被调用了")
> 
> #情况一：当程序执行完毕，对象被自动销毁
> # a1 = Animal("小白",2)
> # time.sleep(5)
> 
> #情况二：使用      del 变量    强制销毁对象
> # a1 = Animal("小白",2)
> # del  a1
> # print("over")
> 
> #情况三：将对象创建在函数内部，为一个局部变量，当函数调用完毕，对象会被自动销毁
> def test():
>  a1 = Animal("小白", 2)
>  print("test被调用了")
> 
> test()
> 
> print("over")
> ```

#### 3.案例二

> ```Python
> """"
> 情景：富二代王思聪开着新买的豪车，自豪的向他的新女友炫耀起来
> 
> 
> 分类：
> 富二代类
>  特征：姓名，有钱
>  行为：开车，炫耀
> 
> 汽车类
>  特征：品牌，颜色，价格
>  行为：跑
> 
> 女友类
>  特征：姓名，是否网红
> """
> from  practice02.car import  Car
> from  practice02.gf import  Gf
> from  practice02.richman import RichMan
> 
> 
> #1.创建对象
> wang = RichMan("王思聪")
> 
> car = Car("五菱宏光","银白色","50000￥")
> 
> gf = Gf("凤姐",True)
> 
> #2.让对象执行自己的行为
> wang.drive(car)
> wang.show(gf,car)
> 
> ```
>
> ```Python
> class Car():
>  def __init__(self,brand,color,price):
>      self.brand = brand
>      self.color = color
>      self.price = price
> 
> 
>  def run(self):
>      print(self.name + "running")
> ```
>
> ```Python
> class Gf():
>  def __init__(self,name,isInterStar):
>      self.name = name
>      self.isInterStar = isInterStar
> ```
>
> ```Python
> class RichMan():
>  def __init__(self,name):
>      self.name = name
> 
> 
>  def drive(self,car):
>      print(self.name + "开着豪车" + car.brand)
> 
> 
>  def show(self,gf,car):
>      print(self.name + "向" + gf.name + "炫耀" + car.brand + "啧啧啧，你看看这颜色" + car.color + ",值好多钱哪" + car.price)
> ```

# Day13

### 一、上堂回顾

#### 1.默写题目

> 1.简述面向过程和面向对象的区别
>
> ```Python
> """
> 面向过程
> 	思路：问题是怎样分步骤解决的，然后亲力亲为的去解决问题
> 	程序中：代码从上往下依次执行
> 	优点：性能较高
> 
> 面向对象
> 	思路：将复杂的问题简单化，找到一个具有特殊功能的个体，然后委托该个体帮忙完成某件事情
> 	程序中：程序的执行顺序由用户决定，类和对象和面向对象的核心
> 	优点：易于维护，易于扩展，易于复用
> """
> ```
>
> 2.简述类和对象的区别和联系
>
> ```Python
> """
> 区别：
> 	类：对多个具有共同特征和行为的对象的描述，将多个对象的共同特征和行为抽取，形成一个类，类是抽象的存在
> 	对象：在一个类中，具有某个特征和行为的一个个体，是具体的存在
> 联系：
> 	类是对象的抽象描述，对象是类的具体的存在
> """
> ```
>
> 3.自定义一个类，其中书写构造函数，普通成员函数，析构函数，并在类外面创建对象并调用普通成员函数
>
> ```Python
> #1.定义类
> class MyClass():
>  #2.定义类的成员
>  #构造函数
>  def __init__(self,num):
>      #实例属性
>      self.num = num
>  #普通成员函数
>  def show(self):
>      pass
>  #析构函数
>  def __del__(self):
>      pass
>  
> #3.创建对象
> m = MyClass(17)
> #4.调用类中的成员函数
> m.show()
> ```

#### 2.知识点回顾

> ```
> 1.属性的动态绑定和限制绑定
> 	__slots__ =  ()
> 	
> 2.构造函数和普通成员函数的区别
> ```

#### 3.作业讲解

> ```Python
> import  math
> 
> """
> 1.定义一“圆”（Circle）类，圆心为“点”Point类，构造一圆，求圆的周长和面积，并判断某点与圆的关系
> """
> 
> """
> 半径：数字，圆心：点的对象
> """
> class Circle():
>  def __init__(self,radius,circlePoint):
>      """
>      定义半径和圆心的属性
>      :param radius: 半径
>      :param circlePoint: 圆心【Point类创建的对象】
>      """
>      self.radius= radius
>      self.circlePoint = circlePoint
> 
>  def circleArea(self):
>      return  3.14 * self.radius ** 2
> 
>  def circleLength(self):
>      return  3.14 * 2 * self.radius
> 
> 
> """
> （x,y）
> """
> class Point():
>  def __init__(self,x,y):
>      self.x = x
>      self.y = y
> 
> 
> if __name__ == "__main__":
>  #创建圆心的对象
>  circlePoint = Point(3,5)
> 
>  #创建圆的对象
>  circle = Circle(8,circlePoint)
> 
>  #求圆的面积和周长
>  print(circle.circleLength())
>  print(circle.circleArea())
> 
>  #判断某点与圆的关系
>  #创建一个某点的对象
>  point = Point(23,5)
> 
>  #判断
>  #（x1,y1）  (x2,y2)  ---->sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2)
>  distance = math.sqrt((point.x - circle.circlePoint.x) ** 2 + (point.y - circle.circlePoint.y) ** 2)
>  if circle.radius == distance:
>      print("点在圆上")
>  elif circle.radius > distance:
>      print("点在圆内")
>  else:
>      print("点在圆外")
> ```

> 封装，继承，多态：
>
> 分别是什么？
>
> 如何使用？
>
> 有什么作用？

### 二、封装

#### 1.概念

> 广义的封装：函数和类的定义，都是封装的体现
>
> 狭义的封装：一个类的某些属性，在使用的过程中，如果不希望被外界直接访问，而是将该属性设置为私有的【只有当前类持有】，然后暴露给外界一个访问的函数即可
>
> 封装的本质：将属性和方法私有化的过程
>
> 封装的好处：提高了代码的安全性，提高了数据的复用性
>
> 举例：插排，不需要关心属性在类的内部做了什么样的操作，只需要关心如何将值传递进去，如果将值获取出来

#### 2.属性私有化

> private:私有的  public：公开的
>
> 只需要在构造函数中定义的变量名的前面添加两个下划线，则该属性就是一个私有属性
>
> 私有化属性的特点：只能在当前类中直接访问，不能在外界直接访问
>
> ```Python
> #1.属性未被私有化
> class Person1():
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
> 
>  def show(self):
>      print("name;%s,age:%d" % (self.name,self.age))
> 
> p1 = Person1("111",11)
> #直接访问
> print(p1.name,p1.age)
> p1.name = "aaa"
> p1.age = 12
> print(p1.name,p1.age)
> 
> p1.show()
> 
> #2.属性被私有化
> class Person2():
>  def __init__(self,name,age):
>      self.name = name
>      self.__age = age
>  def show(self):
>      print("name;%s,age:%d" % (self.name,self.__age))
> 
> p2 = Person2("222",22)
> #直接访问
> print(p2.name)
> #注意：如果一个属性被私有化，则在类的外面不能直接访问
> #print(p2.age)
> #print(p2.__age)
> 
> #动态绑定
> # p2.age = 18
> # print(p2.age)
> 
> #私有化属性的工作原理
> #__xxx,在计算机的底层，该变量被Python解释器解释成了_类名__xxx
> #使用_类名__xxx虽然可以访问到被私有化的属性，但是不建议这么访问，，Python语言是跨平台的，
> # 在不同的平台下，Python解释器对同一条语句解释的结果可能不同
> #print(p2._Person2__age)
> 
> p2.show()
> ```

#### 3.get函数和set函数[了解]

> get函数和set函数并不是系统的函数，而是自定义的，为了和封装的概念相吻合，起名为getXxx或者setXxx
>
> get:获取.获取私有属性的值
>
> set：设置，给私有属性传值
>
> ```Python
> #问题：在外界不能直接访问私有属性，但是非要访问？
> #解决办法：提供给外界一个访问的接口即可
> #3.get函数和set函数
> class Person3():
>  def __init__(self,name,age):
>      self.__name = name
>      self.__age = age
>  def show(self):
>      print("name;%s,age:%d" % (self.__name,self.__age))
> 
>  #get函数：
>  #作用：将私有属性的值返回给外界
>  #命名格式：getXxx,xxx表示被私有化属性的名称
>  #特点：设置返回值
>  def getAge(self):
>      return self.__age
> 
>  #set函数
>  #作用：给私有化型重新赋值
>  #命名格式：setXxx
>  #特点：设置参数
>  def setAge(self,age):
>      self.__age = age
> 
>  def getName(self):
>      return self.__name
>  def setName(self,name):
>      self.__name = name
> 
> p3 = Person3("333",33)
> #获取值
> print(p3.getAge())
> #传值，给私有化属性重新赋值
> p3.setAge(35)
> print(p3.getAge())
> 
> print(p3.getName())
> p3.setName("hello")
> print(p3.getName())
> ```

#### 4.@property装饰器

> ```Python
> #4.使用装饰器间接访问私有属性
> #@property装饰器，可以将函数当做属性访问
> #@xxx.setter装饰器
> #4.1@property的作用：处理私有化属性
> class Person4():
>  def __init__(self,name,age):
>      self.__name = name
>      self.__age = age
>  def show(self):
>      print("name;%s,age:%d" % (self.__name,self.__age))
> 
>  #@property装饰器，相当于get函数，设置返回值，将私有化属性的值返回
>  #注意：函数名可以是任意的标识符，但是，为了提高代码的可读性，一般命名一致
>  @property
>  def name(self):
>      return self.__name
> 
>  #@name.setter装饰器，相当于set函数，设置参数，给私有属性赋值
>  #注意：@xxx.setter,xxx的命名必须和@property修饰的函数的名称完全一致
>  @name.setter
>  def name(self,name):
>      self.__name = name
> 
>  @property
>  def age(self):
>      return self.__age
> 
>  @age.setter
>  def age(self,age):
>      if age < 0:
>          age = -age
>      self.__age = age
> 
> p4 = Person4("4444",10)
> # print(p4.name())
> print(p4.name)     #调用的是@property修饰的函数
> p4.name = "hfajhf"   #调用的是@xx.setter修饰的函数
> print(p4.name)
> 
> print(p4.age)
> p4.age = -19
> print(p4.age)
> 
> #面试题
> #注意：@property可以单独使用，可以将任意一个成员函数转化为属性使用
> class MyClass():
>  @property
>  def show(self):
>      print("showing")
>      return "fahjkfh"
> 
> m = MyClass()
> print(m.show)
> 
> #5.属性的其他形式
> """
> 【面试题】解释下面定义在类中的不同形式变量的含义
> a:普通的变量【public】，在类的内部和外部都可以直接访问
> _a:受保护的变量【Protected】，只能在子类中直接访问，建议在类的外面不要直接访问
> __a：私有化属性【private】，只能在当前类的内部访问，在外界不能直接访问
> __a__：系统的变量，如：__init__,__del__,__name__,__slots__等，自定义的变量尽量不要这种形式
> """
> class Person5():
>  def __init__(self,name,age):
>      self._name = name
>      self.__age__ = age
>  def show(self):
>      print("name;%s,age:%d" % (self._name,self.__age__))
> 
> p5 = Person5("555",5)
> print(p5._name)
> print(p5.__age__)
> ```

#### 5.函数私有化

> ```Python
> #6.函数私有化
> #和属性的私有化相同，如果想让一个函数只能在类的内部被调用，可以在函数名的前面添加两个下划线
> class Person6():
>  def __init__(self,name,age):
>      self.__name = name
>      self.__age = age
>  def __show(self):
>      print("name;%s,age:%d" % (self.__name,self.__age))
> 
>  def func(self):
>      #注意：在类的内部，任意两个函数之间进行调用，调用格式为：self.xxx()
>      self.__show()
> 
> p6 = Person6("66",6)
> #p6.show()   #AttributeError: 'Person6' object has no attribute 'show'
> p6.func()
> ```

### 三、继承

#### 1.概念

> 类和类之间的关系：
>
> ​	is-a:继承或者泛化，比如：学生类和人类，手机类和电子产品类等都是继承关系
>
> ​	has-a：关联，比如：部门和员工的关系，关联关系表示的整体和部分的关联
>
> ​	use-a：依赖，比如：司机有一个驾驶的行为
>
> 如果两个或者两个以上的类中存在相同的属性或者函数，我们可以抽取一个类，在抽取出来的类中定义公共的属性或者函数，
>
> ​	被抽取出来的类：父类   超类   基类
>
> ​	两个或者两个以上的类：子类   派生类
>
> ​	他们之间的关系：子类 继承自  父类    或者  父类 派生了 子类

#### 2.单继承

> 一个子类只有一个父类，被称为单继承
>
> 语法：
>
> 父类：
>
> class  父类类名(object):
>
> ​	类体
>
> 子类：
>
> class  子类类名(父类类名)：
>
> ​	类体
>
> 注意：object是Python中所有类的根类，如果一个类的父类没有被明确，默认为object
>
> 基本使用
>
> ```Python
> from  extends01.student import Student
> from  extends01.worker import Worker
> from extends01.person import  Person
> 
> 
> #1.如果子类中没有定义构造函数
> #注意1：如果子类中没有定义构造函数，创建子类对象的时候，会默认调用父类中的构造函数，
> # 同时通过子类对象访问父类中未被私有化的属性和成员函数
> #s1 = Student()  #TypeError: __init__() missing 2 required positional arguments: 'name' and 'age'
> s1 = Student("zhangsan",19)
> s1.study()
> s1.eat()
> print(s1.name,s1.age)
> 
> #2.如果子类中定义了构造函数
> #注意2：如果子类中定义了构造函数,创建子类对象的时候，会调用子类中的构造函数，但是，如果想要使用父类中的属性，
> # 则在子类IDE构造函数中需要手动调用父类的构造函数
> w1 = Worker("jack",18,"工人")
> w1.work()
> w1.eat()
> print(w1.name,w1.age,w1.kind)   #AttributeError: 'Worker' object has no attribute 'name'
> 
> #注意3：不管是什么类型的继承，创建对象的时候，都要保证参数的匹配
> 
> #3.父类的对象访问子类中特有的数据
> #注意4：父类不能访问子类中特有的属性或者方法
> p1 = Person("lisi",10)
> p1.eat()
> #p1.study()   #AttributeError: 'Person' object has no attribute 'study'
> 
> ```
>
> ```Python
> class Person(object):
>  def __init__(self, name, age):
>      self.name = name
>      self.age = age
> 
>  def eat(self):
>      print("eating")
> 
> ```
>
> ```Python
> from  extends01.person import Person
> class Student(Person):
>  def study(self):
>      print("studying")
> 
> ```
>
> ```Python
> from  extends01.person import Person
> class Worker(Person):
>  def __init__(self,name,age,kind):
>      self.kind = kind
> 
>      #在子类的构造函数中调用父类的构造函数
>      #方式一：super(当前类,self).__init__(属性列表)
>      #super(Worker,self).__init__(name,age)
> 
>      #方式二：父类名.__init__(self,属性列表)
>      #Person.__init__(self,name,age)
> 
>      #方式三:super().__init__(属性列表)
>      super().__init__(name,age)
> 
>  def work(self):
>      print("working")
> 
> ```
>
> slots在继承中的使用
>
> ```Python
> class SuperClass(object):
>  __slots__ = ("name", "num")
>  def __init__(self,name,num):
>      self.name = name
>      self.num = num
> 
> 
> s = SuperClass("fea",10)
> print(s.name)
> s.name = "hello"
> print(s.name)
> 
> # s.age = 18
> # print(s.age)
> 
> class SubClass(SuperClass):
>  __slots__ = ("name", "num")
> 
> 
> s1 = SubClass("aaa",20)
> print(s1.name)
> s1.name = "hello"
> print(s1.name)
> 
> 
> #注意：在父类中限制属性的动态绑定，该操作对子类没有任何作用，如果子类也需要限制绑定，必须手动在子类中设置
> # s1.age = 18
> # print(s1.age)
> # s1.score = 100
> # s1.ste1 = "fafghj"
> 
> ```

#### 3.函数的重写

##### 3.1系统函数

> ```Python
> class Animal(object):
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
>  def show(self):
>      print("父类~~~show")
> 
>  #重写object类中的__str__
>  def __str__(self):
>      #return 199   #__str__ returned non-string (type int)
>      return  "name=%s,age=%s" % (self.name,self.age)
> 
>  # def __repr__(self):
>  #     return "fajkfgah"
> 
>  __repr__ = __str__
> 
> a = Animal("aaa",10)
> 
> #1.未重写
> #需求：打印对象，获取对象的信息
> #print(a)  #<__main__.Animal object at 0x0000021ED10A9128>
> #注意1：打印一个对象的时候，默认调用object中的__str__,该函数默返回当前对象的地址
> #print(a.__str__())  #<__main__.Animal object at 0x0000021ED10A9128>
> 
> #2.重写
> print(a)
> #print(a.__str__())
> 
> a1 = Animal("小白",10)
> print(a1)
> 
> 
> #__repr__和__str__一样，只不过__str__是给用户识别的，__repr__是给计算机识别的
> """
>  1.当repr和str都未被重写，打印对象，优先调用的是str
>  2.当str被重写，repr未被重写，打印对象，优先调用的是str
>  3.当repr被重写，str未被重写，打印对象，优先调用的是repr
>  4.当repr和str都被重写，打印对象，优先调用的是str
> """
> 
> ```

##### 3.2自定义函数

> ```Python
> class Animal(object):
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
>  def show(self):
>      print("父类~~~show")
> 
> class Cat(Animal):
>  pass
> 
> class Dog(Animal):
>  def __init__(self,name,age,color):
>      super().__init__(name,age)
>      self.color = color
> 
>  #重写：如果父类中的函数满足不了子类的需求，则在子类中需要重新实现指定的函数
>  def show(self):
>      print("子类~~~~show")
> 
> #创建子类的对象
> d = Dog("大黄",5,"黄色")
> #结论：如果在子类中重写了父类中的函数，则通过子类的对象调用，优先调用子类中的函数
> d.show()
> 
> ```

#### 4.多继承

> 一个子类可以有多个父类，被称为多继承
>
> 语法：
>
> class 子类类名(父类1，父类2.。。。)：
>
> ​	类体
>
> 基本使用
>
> ```Python
> from extends03.bird import Bird
> 
> #创建子类的对象
> 
> #1.父类和子类中都没有定义构造函数，默认调用的是父类列表中第一个父类中的构造函数
> #2.如果父类中定义了构造函数，子类中没有定义，默认调用的是父类列表中第一个父类中的构造函数
> # b1 = Bird()
> # b1.fly()
> # b1.run()
> 
> 
> #3.在子类中定义了构造函数
> b2 = Bird(2,43,4)
> print(b2.num1,b2.num2,b2.num3)
> 
> #注意：如果哦在多个父类中出现了重名的函数，使用子类对象调用，默认调用父类列表中第一个父类中的函数
> b2.eat()
> 
> ```
>
> ```Python
> class Flyable(object):
>  def __init__(self,num1):
>      print("fly~~~init")
>      self.num1 = num1
> 
>  def fly(self):
>      print("flying")
> 
>  def eat(self):
>      print("fly~~~~eat")
> 
> ```
>
> ```Python
> class Runable(object):
>  def __init__(self,num2):
>      print("run~~~init")
>      self.num2 = num2
> 
>  def run(self):
>      print("running")
> 
>  def eat(self):
>      print("run~~~~eat")
> 
> ```
>
> ```Python
> from  extends03.flyable import Flyable
> from  extends03.runable import Runable
> class Bird(Flyable,Runable):
>  def __init__(self,num1,num2,num3):
>      self.num3 = num3
> 
>      #调用父类中的构造函数
>      #注意：如果在子类中要调用所有父类的构造函数，则使用父类类名.__init__(属性列表)
>      Runable.__init__(self,num2)
>      Flyable.__init__(self,num1)
> ```
>
> 继承树
>
> ```Python
> #父类
> class BaseClass(object):
>  def show(self):
>      print("baselass")
> 
> #子类
> class SubClassA(BaseClass):
>  def show(self):
>      print("enter subclass~~~~A")
>      super().show()
>      print("exit subclass~~~~A")
> 
> class SubClassB(BaseClass):
>  def show(self):
>      print("enter subclass~~~~B")
>      super().show()
>      print("exit subclass~~~~B")
> 
> class SubClassC(SubClassA):
>  def show(self):
>      print("enter subclass~~~~C")
>      super().show()
>      print("exit subclass~~~~C")
> 
> class SubClassD(SubClassB,SubClassC):
>  def show(self):
>      print("enter subclass~~~~D")
>      super().show()
>      print("exit subclass~~~~D")
> 
> s = SubClassD()
> s.show()
> 
> """
> 继承树：
>  在多继承树中，如果在中间某层有向上一层解析的迹象，则会按照父类列表中父类的顺序解析，
>  将所有类中的方法全部解析完毕，然后从本层继续向上解析，这种现象被称为从子类到超类的反向树中广度优先解析
> 
>  在上面的代码中，先从D开始进入B，因为B有向上一层解析的迹象，所以先解析C,然后由C进入了A,最后直接解析根类BaseClass
> 
> 
> 经典类：Py2.x，没有继承object的类以及它的子类，采用的深度优先解析
> 新式类：py3.x，继承自object的类以及它的子类，采用的广度优先解析
> 
> """
> ```

### 四、综合练习

> 奥特曼打小怪兽
>
> ```Python
> #父类：战斗者
> class Fighter(object):
>  __slots__ = ("__name","__hp")
>  def __init__(self,name,hp):
>      """
>      初始化方法
>      :param name: 姓名
>      :param hp: 生命值
>      """
>      self.__name = name
>      self.__hp = hp
>  #姓名
>  @property
>  def name(self):
>      return self.__name
>  @name.setter
>  def name(self,name):
>      self.__name = name
> 
>  #生命值
>  @property
>  def hp(self):
>      return  self.__hp
>  @hp.setter
>  def hp(self,hp):
>      #三目运算符,为了保证输入的生命值一定是大于0的
>      self.__hp = hp if hp >= 0 else 0
> 
>  #检测战斗者的生命值是否为0
>  @property
>  def alive(self):
>      return  self.__hp > 0
> 
>  #攻击
>  def attack(self,other):
>      pass
> 
> ```
>
> ```Python
> #奥特曼
> from extends05.fighter import Fighter
> from random import  *
> 
> class Superman(Fighter):
>  __slots__ = ("__name","__hp","__mp")
> 
>  def __init__(self,name,hp,mp):
>      """
>      初始化方法
>      :param name: 姓名
>      :param hp: 生命值
>      :param mp: 魔法值
>      """
>      super().__init__(name,hp)
>      self.__mp = mp
> 
>  #重写父类中的函数
>  def attack(self,other):
>      """
>      普通的攻击
>      :param other:被攻击的对象
>      :return:
>      """
>      other.hp -= randint(15,25)
> 
>  def huge_attack(self,other):
>      """
>      必杀技：打掉对方至少50%的生命值或者四分之三的生命值
>      :param other:被攻击的对象
>      :return:
>      """
>      if self.__mp >= 50:
>          self.__mp -= 50
>          injury = other.hp * 3 // 4
>          injury = injury if injury >= 50 else 50
>          other.hp -= injury
>          return  True
>      else:
>          self.attack(other)
>          return  False
> 
>  def magic_attack(self,others):
>      """
>      魔法攻击
>      :param others: 被攻击的群体
>      :return: 使用魔法成功则返回True
>      """
>      if self.__mp >= 20:
>          self.__mp -= 20
> 
>          for temp in others:
>              if temp.alive:
>                  temp.hp -= randint(10,15)
> 
>          return True
>      else:
>          return False
> 
>  def resume(self):
>      #恢复魔法值
>      point = randint(1,10)
>      self.__mp += point
>      return point
> 
>  def __str__(self):
>      return "****%s奥特曼****\n" % (self.__name) + "生命值：%s\n" % (self.__hp) + "魔法值：%s" % (self.__mp)
> 
> ```
>
> ```Python
> #小怪兽
> from extends05.fighter import Fighter
> from random import  *
> class Monster(Fighter):
>  __slots__ = ("__name","__hp")
> 
>  def attack(self,other):
>      other.hp -= randint(1,5)
> 
>  def __str__(self):
>      return "****%s小怪兽****\n" % (self.__name) + "生命值：%s" % (self.__hp)
> ```
>
> ```Python
> from  extends05.superman import Superman
> from  extends05.monster import Monster
> from  random import  *
> import  time
> 
> 
> #判断是否有小怪兽是存活的
> def isanyalive(monsters):
>  for monster in monsters:
>      if monster.alive > 0:
>          return True
>  return False
> 
> #选中一只活着的小怪兽
> def selectalive(monsters):
>  mon_len = len(monsters)
> 
>  while True:
>      monster = monsters[randint(0,mon_len - 1)]
>      if monster.alive > 0:
>          return monster
> 
> def main():
>  #创建奥特曼的对象
>  man = Superman("王大锤",1000,500)
>  #创建小怪兽的对象
>  m1 = Monster("张三",300)
>  m2 = Monster("李四", 200)
>  m3 = Monster("王五", 400)
> 
>  ms = [m1,m2,m3]
> 
>  figthround = 1
> 
>  while man.alive and isanyalive(ms):
>      print("======第%d回合=====" % (figthround))
>      #选中一只小怪兽
>      m = selectalive(ms)
>      skill = randint(1,10)   #通过随机数确定选择哪种技能
>      if skill <= 6:
>          #普通攻击
>          print("%s使用普通攻击打了%s" % (man.name,m.name))
>          man.attack(m)
>          print("%s的魔法值恢复了%s点" % (man.name, man.resume()))
>      elif skill <= 9:
>          #魔法攻击
>          if man.magic_attack(ms):
>              print("%s使用了魔法攻击" % (man.name))
>          else:
>              print("%s的魔法攻击失败" % (man.name))
>      else:
>          #必杀技
>          if man.huge_attack(m):
>              print("%s使用了必杀技攻击了%s" % (man.name,m.name))
>          else:
>              print("%s使用普通攻击打了%s" % (man.name,m.name))
> 
>      #如果小怪兽没死则反击
>      if m.alive > 0:
>          print("%s回击了%s" % (m.name,man.name))
>          m.attack(man)
> 
>      #显示一个回合结束之后所有对象的信息
> 
>      figthround += 1
> 
>      time.sleep(1)
> 
>  print("=======战斗结束======")
>  if man.alive > 0:
>      print("奥特曼%s胜利" % (man.name))
>  else:
>      print("小怪兽胜利")
> 
> if __name__ == "__main__":
>  main()
> ```

# Day14

### 一、上堂回顾

#### 1.默写题目

> 1.分别简述封装和继承，并说明它们的特点
>
> ```Python
> """
> 封装：在面向对象中，将类中的某些个属性私有化，在类的外面不能直接访问，而是暴露出来一个访问的函数，函数和类的定义本身，就是封装的体现
> 特点：
> 	a.提高了数据的安全性
> 	b.提高了数据的复用性
> 	
> 继承：两个类，一个是父类，另外一个是子类，如果子类能够访问父类中未被私有化的属性或者成员函数，则子类继承自父类
> 特点：
> 	a.提高了代码的可维护性
> 	b.提高了代码的可扩展性
> 	c.提高了代码的可复用性
> 	d.在继承关系中，耦合性相对较高【如果修改父类，相关的子类都会随着更改】
> 	e.子类对象可以访问父类中未被私有化的属性和方法
> 	f.父类对象不能访问子类中特有的属性和方法
> """
> ```
>
> 2.使用封装的思想，将类中的属性私有化，在类外面创建对象并传值和获取值
>
> ```Python
> class Person(object):
> def __init__(self,name):
>  self.__name = name
>  
> @property
> def name(self):
>  return self.__name
> 
> @name.setter
> def name(self,name):
>  self.__name = name
>  
> p1 = Person("fserg")
> print(p1.name)
> p1.name = "fg"
> ```
>
> 3.分别定义一个父类和子类，在子类的构造函数中调用父类的构造函数
>
> ```Python
> class Father(object):
>  def __init__(self,name):
>      self.name = name
>       
> class Child(Father):
>  def __init__(self,name):
>      super().__init__(name)
>      super(Child,self).__init__(name)
>      Father.__init__(self,name)
> ```

### 二、复习

#### 1.问题补充

> ```Python
> #1.
> class Parent(object):
>  x = 1
> 
> class Child1(Parent):
>  pass
> 
> class Child2(Parent):
>  pass
> 
> print(Parent.x,Child1.x,Child2.x)    #1 1 1,实现了继承，三者指向同一块地址
> Child1.x = 2
> print(Parent.x,Child1.x,Child2.x)   #1   2   1 ，更改child1,指向了一块新的内存空间
> Parent.x = 3
> print(Parent.x,Child1.x,Child2.x)   # 3   2   3  ，更改parent，指向了一块新的内存空间
> #如果子类中没有重新赋值，则默认继承父类中的数据，但是一旦子类进行更改，指向一个新的内存空间
> 
> 
> #2.
> class A(object):
>  def go(self):
>      print("go~~~~A")
> class B(A):
>  def go(self):
>      super(B,self).go()
>      print("go~~~~B")
> class C(A):
>  def go(self):
>      super(C,self).go()
>      print("go~~~~C")
> 
> a = A()
> b = B()
> c = C()
> 
> a.go()   #A
> b.go()   #A    B
> c.go()   #A    C
> ```

#### 2.作业讲解

> ```Python
> """
> 使用封装的思想结合列表完成下面题目
> 	学生类：姓名、年龄、学号、成绩
> 	班级类：班级名称、学生列表
> 		显示所有学生
> 		根据学号查找学生
> 		添加一个学生
> 		删除一个学生（学生对象、学号）
> 		根据学号升序排序
> 		根据成绩降序排序
> """
> from  homework.student import Student
> from  homework.grade import Grade
> 
> #1.创建对象
> stu1 = Student("1001","lisi",18,50)
> stu2 = Student("1005","aaa",20,89)
> stu3 = Student("1003","ddd",16,60)
> stu4 = Student("1002","ccc",18,100)
> stu5 = Student("1004","abc",8,89)
> 
> stulist = [stu1,stu2,stu3,stu4,stu5]
> 
> 
> grade1 = Grade("Python1904",stulist)
> 
> #2.让班级执行自己的行为
> grade1.showAll()
> grade1.searchByStuid("1003")
> #grade1.addStu(stu4)
> 
> stu6 = Student("1006","abc",8,89)
> grade1.addStu(stu6)
> 
> grade1.delStu("1003")
> ```
>
> ```Python
> #学生类：姓名、年龄、学号、成绩
> class Student(object):
>  def __init__(self,stuid,name,age,score):
>      self.name = name
>      self.stuid = stuid
>      self.age = age
>      self.score = score
> 
>  def __str__(self):
>      return "%s-%s-%s-%s" % (self.stuid,self.name,self.age,self.score)
> ```
>
> ```Python
> """
> 班级类：班级名称、学生列表
> 		显示所有学生
> 		根据学号查找学生
> 		添加一个学生
> 		删除一个学生（学生对象、学号）
> 		根据学号升序排序
> 		根据成绩降序排序
> """
> class Grade(object):
>  def __init__(self,name,stulist):
>      self.name = name
>      self.stulist = stulist
> 
>  #显示所有学生
>  def showAll(self):
>      print("学生信息如下：")
>      for stu in self.stulist:
>          print(stu)
> 
>  #根据学号查找学生
>  def searchByStuid(self,stuid):
>      print("查找结果如下：")
>      for stu in self.stulist:
>          if stu.stuid == stuid:
>              print(stu)
>              return
> 
>      print("没有该学号对应的学生信息")
> 
>  #添加一个学生
>  def addStu(self,stu):
>      if stu not in self.stulist:
>          self.stulist.append(stu)
>          print("添加成功")
>      else:
>          print("该学生已经存在")
> 
> 
>      print("添加完成之后，学生信息如下：")
>      self.showAll()
> 
>  #删除一个学生（学生对象、学号）
>  def delStu(self,stuid):
>      for stu in self.stulist:
>          if stu.stuid == stuid:
>              self.stulist.remove(stu)
> 
>      print("删除完成之后学生信息如下:")
>      self.showAll()
> 
>  def sortByScore(self):
>      for i in range(len(self.stulist) - 1):
>          for j in range(len(self.stulist) - i - i):
>              if  self.stulist[j].score   < self.stulist[j + 1].score:
>                  self.stulist[j],self.stulist[j + 1] = self.stulist[j + 1],self.stulist[j]
> ```

### 三、多态

#### 1.概念

> 一个事物的多种体现形式
>
> 定义时的类型和运行时的类型不一致，当确定类型之后，才能确定能够调用哪个函数或者访问哪个变量
>
> 注意：继承是多态的前提

#### 2.使用

> ```Python
> #1
> class Animal(object):
>  pass
> 
> class Dog(Animal):
>  pass
> 
> a = list()
> a1 = Animal()
> d = Dog()
> 
> #isinstance()
> print(isinstance(a,list))
> print(isinstance(a1,Animal))
> print(isinstance(d,Dog))
> 
> #如果一个类继承自另外一个类，通过子类创建的对象，可以是当前类的类型，同时还是父类的类型
> print(isinstance(d,Animal))
> print(isinstance(a1,Dog))
> 
> #2
> class Dog(object):
>  def show(self):
>      print("dog")
> 
> class SmallDog(Dog):
>  def show(self):
>      print("small ~~~~dog")
> 
> def introduce(temp):
>  temp.show()
> 
> d1 = Dog()
> d2 = SmallDog()
> 
> #当确定类型之后，才能确定能够调用哪个函数或者访问哪个变量
> introduce(d1)
> introduce(d2)
> ```
>
> ```Python
> #需求：人饲养动物园里的动物
> 
> class Person(object):
>  # def feeddog(self,dog):
>  #     dog.eat()
>  # def feedcat(self,cat):
>  #     cat.eat()
>  # def feedmouse(self,mouse):
>  #     mouse.eat()
> 
>  #多态的优点：可以简化代码
>  def feedanimal(self,ani):
>      print(type(ani))
>      ani.eat()
> 
> class Animal(object):
>  def __init__(self,name):
>      self.name = name
> 
>  def eat(self):
>      print(self.name + "eating")
> 
> class Dog(Animal):
>  pass
> class Cat(Animal):
>  pass
> 
> class Tiger(Animal):
>  pass
> 
> class mouse(Animal):
>  pass
> 
> 
> p = Person()
> 
> d = Dog("aaa")
> p.feedanimal(d)
> 
> c = Cat("bbb")
> p.feedanimal(c)
> 
> ```

### 四、获取对象信息

> type():获取一个对象的类型
>
> isinstance():判断一个对象是否属于指定的类型
>
> dir()：获取一个对象中的全部信息
>
> ```Python
> import  types
> #1.type()，返回一个type类型，<class 'xxx'>
> #int,str,bool,float等都是系统提供的类
> print(type(123))
> print(type("abc"))
> print(type(True))
> print(type(type(True)))
> 
> #type类型的变量用于比较
> print(type(123) == type("123"))
> print(type(123) == int)
> 
> #获取函数类型:借助于types模块
> def func():
>  pass
> 
> print(type(func))
> print(type(lambda  x:x))
> print(type(abs))
> 
> print(type(func) == types.FunctionType)   #def自定义函数
> print(type(lambda  x:x) == types.LambdaType)  #匿名函数
> print(type(abs) == types.BuiltinFunctionType)  #系统的内置函数
> print(type((x for x in range(4))) == types.GeneratorType)  #生成器
> 
> #2.isinstance(),返回结果的为布尔值，一般结合if语句
> print(isinstance(123,int))
> print(type(123) == int)
> 
> print(isinstance([1,2,3],(list,tuple,dict,int)))
> print(type([1,2,3]) in (list,tuple,dict,int))
> 
> #3.dir(),返回一个对象的所有信息【属性或者函数】
> #注意：返回一个列表，其中的元素为指定对象的信息的字符串
> 
> #获取系统类的信息
> print(dir("abc"))
> 
> print(dir([1,2,3]))
> 
> print(len("hello"))
> print("hello".__len__())
> 
> #获取自定义类的信息
> class Person(object):
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
> 
>  def show(self):
>      pass
>  def func(self):
>      pass
> 
> p = Person("a",17)
> print(dir(p))
> 
> print("abc" == "fahf")
> print("abc".__eq__("fahf"))
> 
> print(dir(10))
> 
> print(10 > 20)
> # print(10.__gt__(20))
> 
> ```

### 五、类中特殊属性和方法【重点掌握】

#### 1.类属性和实例属性

> 【面试题：类属性和实例属性的区别】
>
> a.定义的位置不同：类属性直接定义在类中，实例属性定义在构造函数中【包含动态绑定的属性】
>
> b.访问方式不同：类属性可以通过类名或者对象访问，实例属性一般只通过对象访问
>
> c.在内存中出现的时机不同：类属性随着类的加载而出现，实例属性随着对象的出现而出现
>
> d.优先级不同：当类属性和实例属性重名的时候，使用对象访问，优先访问的是实例属性
>
> ```Python
> #1
> class Person(object):
>  #定义位置
>  #类属性
>  name = "fahjg"
>  age = 19
> 
>  def __init__(self,name):
>      #实例属性
>      self.name = name
> 
> #访问方式
> #类属性：对象  或者 类名
> print(Person.name)
> p1 = Person("hello")
> print(p1.age)
> 
> #实例属性：对象
> print(p1.name)
> 
> 
> del p1.name
> 
> print(p1.name)
> 
> 
> #注意：只要  对象.属性  = 值，不管指定的属性在类属性中是否被定义，都表示动态绑定
> #不同的对象访问类属性，指向的是同一块内存空间
> p2 = Person("aaa")
> print(p2.age)
> 
> Person.age = 100
> print(p2.age)
> print(p1.age)
> 
> 
> #2
> class Person(object):
>  def __init__(self,name):
>      self.name = name
> 
> p1 = Person("aaa")
> p2 = Person("bbb")
> print(p1.name)
> print(p2.name)
> 
> p2.name = "ccc"
> print(p1.name)
> 
> 
> """
> 使用场景：如果是多个对象的共享数据，则一般定义为类属性
> 如果是每个对象的特有的数据，则一般定义为实例属性
> """
> 
> ```
>
> 动态绑定属性和方法
>
> ```Python
> from  types import  MethodType
> 
> class Person(object):
>  __slots__ = ("name","age","show")
> 
> #1.动态绑定属性
> p1 = Person()
> p1.name = "tom"
> print(p1.name)
> 
> #p1.score = 100  #AttributeError: 'Person' object has no attribute 'score'
> 
> 
> #2.动态绑定成员函数
> # def func(self):
> #     print("func")
> #
> # p1.show = func
> # p1.show(p1)
> 
> 
> def func(self):
>  print(self.name)
> 
> p1.show = MethodType(func,p1)
> p1.show()
> 
> ```

#### 2.类方法和静态方法

> 类方法：在一个方法的前面使用@classmethod修饰
>
> 静态方法：在一个方法的前面使用@staticmethod修饰
>
> ```Python
> class Person(object):
>  #构造函数【成员函数】
>  def __init__(self,name):
>      self.name = name
> 
>  #成员函数
>  def show(self):
>      print("showing")
> 
>  #类函数
>  #形参列表的第一个参数为cls，也可以是任意的标识符，表示当前类
>  @classmethod
>  def func1(cls):
>      print(cls)  #<class '__main__.Person'>
>      print(Person)  #<class '__main__.Person'>
>      print("func~~~111")
> 
>      #可以通过cls来创建当前类的对象，该对象也可以调用当前类中的函数
>      p = cls("hello")
>      print(p.name)
>      p.show()
> 
>  @classmethod
>  def func11(cls):
>      print("func~~~11111111")
> 
>  #静态函数
>  #静态函数对形参列表没有任何要求，一旦设定参数，则都必须手动传参
>  @staticmethod
>  def func2():
>      print("func~~~~2222")
> 
> #1.类函数和静态函数都可以通过类名调用
> Person.func1()
> Person.func2()
> 
> # Person.show()   #TypeError: show() missing 1 required positional argument: 'self'
> 
> #2.成员函数，类函数和静态函数都可以通过对象调用
> per = Person("aaa")
> per.show()
> per.func1()
> per.func2()
> 
> 
> """
> 【面试题】成员函数，静态函数和类函数之间的区别和联系
> 联系：
>  a.都必须手动调用
>  b.都必须定义在类中
>  c.都可以使用默认参数，关键字参数，不定长参数
>  d.都可以使用对象调用
>  e.在继承关系中，父类中的三者都可以被子类继承，同时，都可以在子类中重写
> 
> 区别：
>  a.参数：成员函数第一个参数必须为self。类函数第一个参数必须为cls，静态函数的参数没有要求
>  b.调用方式：静态函数和 类函数可以通过类名或者对象调用，成员函数只能通过对象调用
>  c.使用场景：如果定义的是一个工具类，一般其中的函数都是静态函数或者类函数，直接可以通过类名调用
>             如果要获取对象的信息，则定义成员函数
> """
> 
> ```

#### 3.类常用属性

> ```
> __name__
> 		只能通过类名访问，获取当前类的类名字符串
> 		
> __dict__
> 		通过类名访问，获取的是指定类的信息【类方法，类属性等】
> 		通过对象访问，获取的对象的信息
> 		
> __bases__
> 		通过类名访问，获取一个指定类的所有的父类
> 
> ```
>
> ```Python
> class A(object):
>  pass
> 
> class B(object):
>  pass
> 
> class C(A,B):
>  age = 10
>  height = 199
> 
>  def __init__(self,name):
>      self.name = name
> 
>  def func(self):
>      pass
> 
>  @classmethod
>  def func1(cls):
>      pass
> 
>  @staticmethod
>  def func2():
>      pass
> 
> print(C.__name__)
> print(type(C.__name__))
> 
> c = C("fhaf")
> 
> #类名.__dict__；类属性，成员函数，类函数，静态函数
> print(C.__dict__)   #dir
> #对象.__dict__:实例属性
> print(c.__dict__)
> 
> print(C.__bases__)   #<class '__main__.A'>, <class '__main__.B'>)
> 
> ```

### 六、运算符重载

> 重写：override
>
> 重载：overload
>
> 在Python中，重写和重载都是为了将一个已经存在的函数重新实现，只不过重写必须以继承
>
> ```Python
> #1.+支持的数据类型
> print(2 + 5)
> print(True + False)
> print(True + 6)
> print("fah" + "hello")
> print(10.23 + 3)
> 
> #print("abc" + 6)  #TypeError: must be str, not int
> #print(6 + "abc")  #TypeError: unsupported operand type(s) for +: 'int' and 'str'
> 
> #原因：Python解释器对不同的数据类型有不同解释
> 
> #工作原理:一旦使用+，在计算机的底层调用了__add__函数
> print("abc" + "def")
> print("abc".__add__("def"))
> 
> print("*" * 20)
> 
> #2.
> class Person(object):
>  def __init__(self,age):
>      self.age = age
> 
>  #运算符重载：将add函数重新实现
>  def __add__(self, other):
>      #参与加法运算的是self和other两个对象
>      #两个相同类型的数据相加，得到的结果应该也为该种类型
>      #Person + Person = int不符合常理,应该为Person + Person = Person，所以设置add函数返回一个Person对象
>      #return self.age + other.age
>      return Person(self.age + other.age)
> 
>  #注意：__str__返回值必须是字符串
>  def __str__(self):
>      return str(self.age)
> 
>  def __gt__(self, other):
>      if self.age > other.age:
>          return True
>      else:
>          return False
> 
> p1 = Person(10)
> p2 = Person(18)
> print(p1 + p2)   #28
> print(p1.__add__(p2))
> 
> print(p1 > p2)
> 
> ```

### 七、单例设计模式【重点掌握】

#### 1.案例

> ```Python
> class Person(object):
>  def __init__(self,name):
>      self.name = name
> 
>  def dance(self):
>      print(self.name + "dancing")
> 
> ```
>
> ```Python
> import  singleton01.text01
> import  singleton01.text02
> import  singleton01.text03
> 
> from  singleton01.person import Person
> 
> if __name__ == "__main__":
>  print("中央卫视")
>  p = Person("小彩旗")
>  print(id(p))
>  p.dance()
> 
> ```
>
> ```Python
> from singleton01.person import Person
> 
> if __name__ != "__main__":
>  print("浙江卫视")
>  p = Person("小彩旗")
>  print(id(p))
>  p.dance()
> 
> ```
>
> ```Python
> from singleton01.person import Person
> 
> if __name__ != "__main__":
>  print("江苏卫视")
>  p = Person("小彩旗")
>  print(id(p))
>  p.dance()
> 
> ```
>
> ```Python
> from singleton01.person import Person
> 
> if __name__ != "__main__":
>  print("陕西卫视")
>  p = Person("小彩旗")
>  print(id(p))
>  p.dance()
> 
> ```
>
> 问题：不管在哪个卫视看到的额小彩旗应该都是同一个对象，没有必要占用更多的内存空间，解决这种问题的方案：单例设计模式

#### 2.概念

> 什么是设计模式？
>
> ​	经过总结，优化，对我们经常遇到的问题作出的可重用的解决方案
>
> ​	设计模式更加高级，相当于解决特定问题的模板，设计模式不会绑定特定的编程语言
>
> ​	常用的设计模式有23种，常用的是单例设计模式，工厂设计模式，生产者消费者设计模式，代理委托设计模式等
>
> 什么是单例设计模式？
>
> ​	单个实例，单个对象
>
> ​	程序在运行的过程中，只要确保某一个类只能创建一个对象，不管在该程序的哪个模块中获取该对象，获取的都是同一个对象
>
> ​	单例设计模式的核心：一个类有且只有一个实例，并且该实例可以应用在整个项目中、

#### 3.实现

##### 3.1模块

> Python中的模块就是一个天然的单例，因为模块第一次被导入的时候，会生成一个.pyc文件，当第二次导入时，就会直接加载.pyc文件，而不是执行源代码
>
> 只需要将相关的函数和数据定义在一个模块中，就可以得到一个单例对象
>
> ```Python
> #单例类
> class Person(object):
>  def fun(self):
>      pass
> 
> p = Person()
> 
> ```
>
> ```Python
> from singleton02.single import p
> from singleton02.single import p
> from singleton02.single import p
> from singleton02.single import p
> from singleton02.single import p
> from singleton02.single import p
> 
> #from singleton02.single import Person
> 
> print(p)
> p.fun()
> 
> ```

##### 3.2使用new

> ```Python
> #__new__  __init__
> 
> class Person(object):
>  # def __init__(self,name):
>  #     self.name = name
>  #     print("构造函数被调用了")
> 
>  def __new__(cls, *args, **kwargs):
>      print("new函数被调用了")
> 
>      return super(Person,cls).__new__(cls, *args, **kwargs)
> 
> p1 = Person()
> print(type(p1))
> 
> """
> Python中的构造函数是一个体系，其中包含__init__和__new__,
> 当x = 类名()创建对象的时候，首先调用的__new__,__new__用来创建实例并返回该实例，__init_将传入的参数用来初始化实例
> 
> 如果使用了__init__，则不使用new
> 如果使用了new，则不使用init
> """
> 
> ```

##### 3.3装饰器

> ```Python
> #装饰器不但可以装饰函数，也可以装饰类
> def singleton(cls):
> 
>  instance = None
> 
>  #一般使用getInstance,currentInstance,defaultInstance
>  def getInstance(*args,**kwargs):
>      nonlocal instance
>      if not instance:
>          instance = cls(*args,**kwargs)
> 
>      return instance
>  return getInstance
> 
> @singleton
> class Person(object):
>  def __init__(self,name):
>      pass
> 
> 
> p1 = Person("dd")
> p2 = Person("ff")
> print(id(p1) == id(p2))
> print(p1 is p2)
> 
> #使用装饰器实现单例类，除了当前类只能创建一个对象之前，其他的用法和普通类的用法完全相同
> 
> ```
>
> ```Python
> #装饰器不但可以装饰函数，也可以装饰类
> def singleton(cls):
> 
>  #当前类名作为key，唯一的实例作为value
>  instanceDict = {}
> 
>  def getInstance(*args,**kwargs):
>      if not instanceDict:
>          instanceDict[cls] = cls(*args,**kwargs)
> 
>      return instanceDict[cls]
> 
>  return getInstance
> 
> @singleton
> class Person(object):
>  def __init__(self,name):
>      pass
> 
> p1 = Person("dd")
> p2 = Person("ff")
> print(id(p1) == id(p2))
> print(p1 is p2)
> 
> ```

#  Day15                                             

### 一、上堂回顾

#### 1.默写题目

> 1.书写一个单例类
>
> ```Python
> #用装饰器实现单例类
> 
> #1.引用
> def singleton(cls):
> instance = None
> def getInstance(*args,**kwargs):
>  nonlocal instance
>  if not instance:
>    instance = cls(*args,**kwargs)
>  return instance   
> return getInstance
> 
> @singleton    #cls = Text    Text----->getInstance
> class Text(object):
> 	def __init__(self,name,age):
>    pass
> 
> t1 = Text("aaa",23)   #t1 =  instabce
> t2 = Text("bbb",17)    #t2 = instance
> 
> #2.字典
> def singleton(cls):
> instancedict = {}
> def getInstance(*args,**kwargs):
>  if not instancedict:
>    instancedict[cls] = cls(*args,**kwargs)
>  return instancedict[cls]  
> return getInstance
> 
> @singleton    #cls = Text    Text----->getInstance
> class Text(object):
> 	def __init__(self,name,age):
>    pass
> 
> t1 = Text("aaa",23)   #t1 =  instancedict[cls]  
> t2 = Text("bbb",17)    #t2 = instancedict[cls]  
> ```
>
> 2.简述类属性和实例属性之间的区别
>
> ```Python
> """
> a.定义位置不同
> b.访问的方式不同
> c.在内存中出现的时机不同
> d.重名的情况下，通过对象访问的优先级不同
> """
> ```

#### 2.知识点回顾

> 1.多态
>
> ​	继承是多态的前提【通过子类定义的变量，是子类的类型，同时也是父类的类型】
>
> 2.获取对象信息
>
> ​	type  isinstance   dir()
>
> ​	__name__:类名的字符串
>
> ​	__dict__:获取类或者对象的信息
>
> ​	__bases__:获取当前类的所有的父类
>
> ​	__class__:类
>
> 3.成员函数，类函数和静态函数之间的区别
>
> 类属性和实例属性
>
> 4.单例设计模式

### 二、错误和异常

#### 1.概念

> Python中有两种错误比较容易辨认：语法错误【直接报错】和异常【代码正常，运行会报错】
>
> 有些异常是输入造成的，有些异常是代码在执行过程中的突发状态，比如：写入文件，磁盘满了，或者从网络抓取数据，但是网络突然断掉等
>
> ```Python
> #1.
> # list1 = [23,54,54,5,6]
> # print(list1[1])
> # print(list1[10])
> # print("over")
> 
> #异常的特点：在代码执行的过程中遇到了异常，而且该异常未被处理，则代码会终止向下执行，整个程序结束
> 
> #处理异常的方式：想办法将可能出现异常的代码检测起来，当异常出现的时候，
> # 将出现异常的代码"屏蔽"起来，为了能够让后面的代码继续执行
> 
> #2.
> try:
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[1])
>  print(list1[10])
> 
>  print("hello")
> except IndexError as e:
>  print("出现了异常")
> 
> print("over")
> ```

#### 2.常见的异常

> ```Python
> #1.NameError:当一个变量或者函数未被定义就使用
> # print(num)
> 
> #2.KeyError:当访问了字典中不存在的key
> # dict1 = {"a":1}
> # print(dict1["b"])
> 
> #3.ValueError:当进行类型转换的时候【int,float】
> # s = int("faf")
> 
> #4.TypeError:当类型不匹配的时候
> #print("af" + 18)
> 
> #5.AttributeError:当试图访问了一个对象不存在的属性或者函数
> # print("faf".reverse())
> 
> #6.UnboundLocalError:变量的作用范围不明确的时候
> # def singleton(cls):
> #   instance = None
> #   def getInstance(*args,**kwargs):
> #     nonlocal instance
> #     if not instance:
> #       instance = cls(*args,**kwargs)
> #     return instance
> #   return getInstance
> #
> # @singleton    #cls = Text    Text----->getInstance
> # class Text(object):
> #     def __init__(self,name,age):
> #         pass
> #
> # t1 = Text("aaa",23)
> 
> # num = 10
> # def text():
> #     global  num
> #     num += 1
> # text()
> 
> #7.IndexError:下标越界异常【str,list,tuple等访问元素的时候】
> 
> #8.ImportError:无法导入模块或者包【一般是路径问题】
> 
> #9.SyntaxError；Python代码非法，代码不能编译【缩进，冒号，括号等】
> ```

#### 3.处理异常

##### 3.1try-except-else/finally捕获

> 语法：
>
> try:
>
> ​	语句1
>
> except  错误表示码1  as   变量：
>
> ​	语句2
>
> except  错误表示码2  as   变量：
>
> ​	语句3
>
> 。。。。
>
> else/finally:
>
> ​	语句n
>
> 说明：
>
> ​	a.try语句被称为检测区，检测其中的代码是否存在异常，try语句不能省略
>
> ​	b.except表示当try中的语句出现异常，需要处理的语句，可以省略，可以写一个，也可以写多个
>
> ​	c.else可以省略，组合语句try-except-else,或者try-else
>
> ​	d.finally也可以省略，组合语句try-except-finally或者try-finally
>
> ​	e.如果try中的代码存在异常，则执行顺序try-except---->finally
>
> ​	f.如果try中代码不存在异常，则执行顺序try-finally
>
> ```Python
> #1.只使用一个except
> """
> try:
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[1])
>  #注意：在Python中，异常也被面向对象化了，出现的具体的异常就是一个对象，对象的类型在出现异常的时候已经被确定
>  print(list1[10])
> 
>  print("hello")
> #IndexError是一个错误表示码，实际上是一个系统类
> #e只是一个变量名，指向当前出现的异常的对象 e = IndexError(xx)
> except IndexError as e:
>  #默认直接打印对象，结果为该对象在内存中的地址，但是，直接打印e结果为一个异常的信息描述，原因：在异常的类中，已经重写了object中的__str__
>  print(e)
> 
> print("over")
> 
> 
> #注意：如果try中的代码出现异常，如果要处理该异常，则必须存在一个匹配的except语句，否则原本的异常仍然未被处理
> 
> #2.使用多个except
> #注意：当try中的异常可能存在多个，就需要有多个except语句匹配，不管出现多少个except，都只会匹配其中的一个
> #原理：根据try中出现的异常类型进行匹配执行的except，从上往下依次查找，直到找到匹配的类型，否则指定的异常仍然存在
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> except IndexError as e:
>  print(e)
> except ValueError as e:
>  print(e)
> 
> print("over")
> 
> #注意：不管try中出现多少个异常，不管书写了多少个except语句，都只会处理其中的一个异常【if多分支】
> 
> #3.错误表示码为父类
> #系统的异常都是类，他们共同的父类为BaseException---->Exception---->object
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> except ValueError as e:
>  print(e)
> except Exception as e:
>  print(e)
>  print("BaseException")
> 
> print("over")
> 
> 
> #注意：当父类出现在except的第一条时，会“包揽”所有的异常，使用了多态【e可以有两种数据类型，一种是BaseException，另一种是IndexError】
> 
> #4.只使用一个except，不表明异常的类型
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> #可以匹配所有的异常，但是缺点：不能确定是哪种异常
> except:
>  print("出现了异常")
> 
> print("over")
> 
> 
> #5.只使用一个except，表明异常的类型
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> #可以匹配元组中指定的的异常，相比较4，仅仅是缩小了异常的范围，但是缺点：不能确定是元组中的哪种异常
> except(TypeError,IndexError,ValueError,NameError):
>  print("出现了异常")
> 
> print("over")
> 
> 
> 
> #6.else语句：只有当try中的语句没有任何异常的时候，才会被执行
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> except IndexError as e:
>  print(e)
> except ValueError as e:
>  print(e)
> else:
>  print("else被执行了")
> 
> print("over")
> 
> 
> 
> #7.finally语句：不管try中的语句是否存在异常，都会被执行
> try:
>  num = int(input("请输入数字："))
>  list1 = [23, 54, 54, 5, 6]
>  print(list1[num])
> 
>  print("hello")
> except IndexError as e:
>  print(e)
> except ValueError as e:
>  print(e)
> finally:
>  print("finally被执行了")
> 
> print("over")
> 
> 
> #【面试题】特殊情况:当函数内部出现异常，在try或者except中书写return，不会影响finally的执行，finally仍然会被执行
> #finally语句的作用：一般用来处理一些清理行为，包括文件关闭，数据库关闭等
> def show():
>  try:
>      num = int(input("请输入数字："))
>      list1 = [23, 54, 54, 5, 6]
> 
>      return
> 
>      print(list1[num])
> 
>      print("hello")
>  except IndexError as e:
>      print(e)
>  except ValueError as e:
>      print(e)
>  finally:
>      print("finally被执行了")
> 
>  print("over")
> 
> show()
> """
> 
> #8.省略掉except语句，如果try中没有异常，则直接执行finally。，如果有异常，则直接报出异常
> try:
>  num = int(input("输入："))
>  #除数或者分母不能为0
>  print(10 / num)
> finally:
>  print("finally")
> ```

##### 3.2raise抛出

> 在异常中，异常对象的出现有两种方式：1，根据具体的问题体现  2.通过系统的异常类创建对象
>
> 语法：raise  异常对象
>
> ```Python
> #raise关键字的作用：代码本来没有异常，通过具体的需求想要在程序的某个地方出现一个异常，
> # 则需要抛出一个具体的异常的对象，最终还是需要通过try-except捕获
> 
> #a.具体的代码
> #异常只是一种可能性
> # try:
> #     num = int(input(""))
> #     print(10 / num)
> # except ZeroDivisionError as e:
> #     print(e)
> 
> #b。创建一个异常对象
> #指定的异常100%存在的
> try:
>  raise ZeroDivisionError("除数不能为0")
> except ZeroDivisionError as e:
>  print(e)
> 
> #说明：raise关键字一般结合自定义异常使用，系统的异常一般都是通过具体的问题体现
> ```

##### 3.3assert断言

> print:辅助调试
>
> assert：替代print，在可能存在问题的代码处设置一个断言，如果断言成功，则代码正常执行，如果断言失败，则会报出AssertionError
>
> ```Python
> def divide(num1,num2):
> 
>  #在可能存在异常的代码之前添加一个断言【预测】，如果预测成功，则正常执行；如果预测失败，则后面的代码不执行，报=出一个新的异常AssertionError
>  assert num2 != 0,"~~~~除数num2不能为0~~~~"
> 
>  return num1 / num2
> 
> print(divide(19,0))
> ```

### 4.自定义异常

> 自定义异常的原理：需要继承自系统的异常类，为了保持系统的异常机制
>
> ```Python
> #1.定义类，继承自系统的异常类【继承自BaseException或者Exception】
> class MyException(BaseException):
>  #2.书写构造函数
>  #message用来记录异常的描述信息,为一个字符串
>  def __init__(self,message):
> 
>      #3.调用父类的构造函数
>      super(MyException,self).__init__()
> 
>      self.message = message
> 
>  #4.重写str函数，当打印异常对象的时候，得到的结果为异常 的信息描述
>  def __str__(self):
>      return str(self.message)
> 
>  #5.定义普通的成员函数，当异常出现的时候，需要解决异常
>  def handle(self):
>      print("处理了异常")
> 
> try:
>  raise MyException("出现了异常")
> except MyException as e:
>  print(e)
> 
>  e.handle()
> ```

### 三、文件读写【重点掌握】

> Python中内置了文件读写的函数，用法和c语言是兼容的
>
> 工作原理：操作系统不允许在磁盘上直接读写文件，所以，读写就是请求操作系统打开 一个文件对象【被称为文件描述符】，然后，通过操作系统提供的接口从这个文件对象中读取数据【读文件】，或者将数据写入到文件对象中【写文件】

#### 1.常用文件的读写

##### 1.1读文件

> 步骤：
>
> a.打开文件：open()
>
> b.读取内容：read()
>
> c.关闭文件：close()
>
> ```Python
> """
> 读文件：从磁盘到内存，Input
> 写文件：从内存到磁盘,Output
> 
> IO：Input/Output
> 
> IOError:当文件读取完毕，还继续读取
> """
> 
> import  os
> 
> #读文件
> 
> #一、打开文件
> """
> open(path,flag,encoding,errors)
>  path:需要打开的文件的路径，绝对路径或者相对路径都可以，一般r"xxxx"
>  flag：打开文件的方式：
>      r:以只读的方式打开文件，文件描述符出现在文件的开头
>      rb:以二进制的方式打开一个文件用于只读，文件描述符出现在文件的开头
>      r+:打开一个文件用于读写，文件描述符出现在文件的开头
>  encoding：编码格式，常用utf-8和gbk
>  errors：进行读取文件的时候的错误处理，一般使用异常，可忽略
> """
> path = r"致橡树.txt"
> #以只读的方式打开文件
> #f是一个变量，指向一个被打开的文件，被称为文件对象
> f = open(path,"r",encoding="gbk")
> 
> """
> 注意：
>  1.如果flag采用的是rb，encoding则必须省略，否则报错
>  2.如果flag采用的是r，如果文件格式是gbk，则可以省略encoding='gbk';
>     如果文件格式是utf-8.则不能省略encoding='utf-8'
>     open函数默认可以识别gbk的文件
> """
> 
> #二、读取文件内容
> #1.read
> #1.1默认读取文件中的所有内容
> #使用场景：读取内容较少的文件
> # str1 = f.read()
> # print(str1)
> 
> #1.2一次读取指定字节的内容
> #使用场景：结合循环，读取内容较多的文件
> # str1 = f.read(3)
> # print(str1)
> # str1 = f.read(3)
> # print(str1)
> # str1 = f.read(3)
> # print(str1)
> 
> #采用read(num)方式读取文件中的全部的内容，借助于循环
> #在读取数据量大的文件时，一次读取的大小一般为1024
> # size = os.path.getsize(path)
> # num = 1024
> # while size > 0:
> #     str1 = f.read(num)
> #     print(str1)
> #     size -= num
> 
> #2.readline
> #2.1一次读取一行内容【回车，换行符】
> # str2 = f.readline()
> # print(str2)
> # str2 = f.readline()
> # print(str2)
> # str2 = f.readline()
> # print(str2)
> # str2 = f.readline()
> # print(str2)
> 
> #借助于循环读取全部的内容,如果返回值为假，则表示没有内容可读
> # result = f.readline()
> # while result:
> #     print(result)
> #     result = f.readline()
> 
> #2.1readline(num),类似read(num),但是一般不这样使用，使用的目的是为了一次读取一行内容
> # str2 = f.readline(3)
> # print(str2)
> # str2 = f.readline(3)
> # print(str2)
> 
> #3.readlines，按照行进行读取，结果为一个列表，其中会显示换行符和空格
> str3 = f.readlines()
> print(str3)
> 
> #三、关闭文件
> #注意：关闭的文件的目的时候为了避免系统资源的浪费
> f.close()
> 
> ```

##### 1.2写文件

> 步骤：
>
> a.打开文件：open()
>
> b.写入内容：write()
>
> ​    刷新：flush()
>
> c.关闭文件：close()
>
> ```Python
> #写文件
> 
> #一、打开文件
> """
> open(path,flag,encoding,errors)
>  flag:文件的打开方式
>      w:以写入的方式打开一个文件，文件描述符存在文件的开头
>      wb:以二进制的方式打开一个文件用于写入，文件描述符存在文件的开头
>      w+:打开一个文件用于读写，文件描述符出现在文件的开头
>      a：append，在源文件内容的后面进行追加内容
> """
> f = open(r"file1.txt","a",encoding="gbk")
> 
> #二、写入内容
> f.write("啊啊啊啊jgghhg")
> 
> #一般在写入内容之后需要做一个刷新，加快数据的写入速率
> f.flush()
> 
> 
> #三、关闭文件
> f.close()
> 
> 
> """
> 总结：
>  1.不管是读取文件还是写入文件，都需要先打开文件，打开的方式取决于需要进行的操作
>  2.如果是读取文件，则文件必须存在，而如果是写入文件，则文件可以不存在，在写入的过程中会自动创建
>  3.在写入文件的过程中，如果采用的是w，则表示覆盖，如果采用的是a则表示追加
>  4.在进行文件读写的时候，一定要注意使用的编码格式和文件本身的编码格式需要保持一致，否则乱码
> """
> 
> ```

##### 1.3简写形式

> ```Python
> #文件读写的简写形式
> #with。。。。。as...
> """
> 通过with...as..简化文件读写过程中的异常
> 优点：当文件读写完毕之后，可以自动关闭文件，不需要手动关闭
> """
> 
> #读文件
> #f只是一个变量，只是指向打开的文件对象
> with open(r"致橡树.txt","r",encoding="gbk") as f:   #f = open(path,"r",encoding="gbk")
>  print(f.read())
> 
> 
> #写文件
> with open(r"file1.txt","w",encoding="gbk") as f:
>  f.write("读写文件aaaa")
>  f.flush()
> 
> 
> #注意：一旦代码执行完with...as代码块，则文件就会自动被关闭，但是，对于变量不会引入新的作用域
> 
> ```

##### 1.4文件拷贝

> ```Python
> #需求：封装函数，实现一个文件内容的拷贝
> # path = r"致橡树.txt"
> # f = open(path,"rb")
> # #print(f.read())
> #
> # print(f.read().decode("gbk"))
> 
> import  os
> 
> #考虑问题：要拷贝的是哪种类型的文件，使用哪种编码格式拷贝
> def mycopy(srcpath,srcencode,despath,desencode):
>  """
>  实现任意文件的拷贝
>  :param srcpath: 源文件的路径
>  :param srcencode: 源文件的编码格式
>  :param despath: 目标文件的路径
>  :param desencode: 目标文件的编码格式
>  :return: None
>  """
> 
>  #判断源文件是否存在
>  if not os.path.exists(srcpath):
>      print("源路径不存在，无法拷贝")
>      return
>  #判断源路径是否是文件
>  if os.path.isdir(srcpath):
>      print("源路径是一个目录，无法拷贝")
>      return
> 
>  #打开文件
>  if os.path.splitext(srcpath)[1] in [".jpg",".png",".mp3",".mp4"]:
>      srcfile = open(srcpath,"rb")
>      desfile = open(despath,"wb")
>  else:
>      srcfile = open(srcpath, "r",encoding=srcencode)
>      desfile = open(despath, "w",encoding=desencode)
> 
>  #开始拷贝
>  #获取源文件的大小
>  size = os.path.getsize(srcpath)
>  while size > 0:
>      content = srcfile.read()
>      desfile.write(content)
>      desfile.flush()
> 
>      size -= 1024
> 
>  #关闭文件
>  srcfile.close()
>  desfile.close()
> 
> if __name__ == "__main__":
>  # mycopy(r"dog.jpg","","image.jpg","")
>  mycopy(r"file1.txt", "gbk", "file4.txt", "utf8")
> 
> ```

#### 2.csv文件的读写

> csv也是一种纯文本文件的格式，是一组字符序列，字符之间使用英文的逗号或者tab键隔开
>
> 作用：在不同的程序之间实现数据的交互

##### 2.1写文件

> ```Python
> #读取csv文件
> 
> import  csv
> 
> #1.csv文件特有的读取方式
> def readcsv1(path):
>  #1.打开文件
>  csvfile = open(path,"r")
>  #2.读取文件内容
>  #区别于普通文件，返回一个可迭代对象,如果要获取文件中的具体内容，则可以遍历该可迭代对象
>  result = csv.reader(csvfile)
>  print(result)
> 
>  for content in result:
>      #可迭代对象中的元素为列表
>      print(content)
> 
>  #3.关闭文件
>  csvfile.close()
> 
> #2.csv文件特有的读取方式
> def readcsv2(path):
>  with open(path,"r") as f1:
>      result = csv.reader(f1)
>      for content in result:
>          #可迭代对象中的元素为列表
>          print(content)
> 
> #3.使用普通文件的读取方式读取csv文件
> def readcsv3(path):
>  with open(path,"r") as f1:
>      result = f1.read()
>      print(result)
> 
> 
> if __name__ == "__main__":
>  readcsv3(r"text01.csv")
> 
> ```

##### 2.2读文件

> ```Python
> #写入csv文件
> import  csv
> 
> #注意：向csv文件中写入任意的可迭代对象
> def writecsv1(path):
>  #1.打开文件
>  csvfile = open(path,"w")
> 
>  #2.写入
>  #获取写入对象
>  result = csv.writer(csvfile)
>  #写入
>  #列表
>  #result.writerow(['aaa','bbbb','ccc','dd'])
>  #字符串
>  #result.writerow("hello")
>  #字典：只写入字典的key
>  result.writerow({"1111":1,"2222":2,"3333":3})
> 
>  #3.关闭文件
>  csvfile.close()
> 
> 
> #简写形式
> def writecsv2(path):
>  with open(path, "w") as f:
>      result = csv.writer(f)
>      result.writerow({"aaaa": 1, "gsdfgf": 2, "bbbb": 3})
> 
> if __name__ == "__main__":
>  writecsv2(r"text02.csv")
> 
> ```

#### 3.编码和解码

> 乱码：utf-8存储中文3个字节，gbk存储中文占用2个字节
>
> 注意：编解码格式要保持一致，如果不一致，修改文件本身的编码格式
>
> ```Python
> path = r"text03.txt"
> 
> #1.编码
> with open(path,"wb") as f1:
>  str1 = "今天是个好日子today is a good day"
>  f1.write(str1.encode("utf-8"))
> #
> # with open(path,"w",encoding="utf-8") as f1:
> #     str1 = "今天是个好日子today is a good day"
> #     f1.write(str1)
> 
> 
> #2.解码
> # with open(path, "rb") as f1:
> #     data = f1.read().decode("utf-8")
> #     print(data)
> 
> with open(path, "r", encoding="utf-8") as f1:
>  data = f1.read()
>  print(data)
> 
> 
> ```

# Day16

### 一、上堂回顾

#### 1.默写题目

> 1.使用装饰器的方式书写一个单例类
>
> 2.封装函数，实现常用文件内容的拷贝【面试题】
>
> ```Python
> import os
> def mycopy(srcpath,despath):
> srcfile = open(srcpath,"rb")
> desfile= open(despath,"wb")
> 
> size = os.path.getsize(srcpath)
> num = 1024
> while size > 0:
>  content = srcfile.read(num)
>  desfile.write(content)
>  desfile.flush()
>  size -= num
>  
> srcfile.close()
> desfile.close()
> 
> #with...as类似if语句，可以嵌套
> with open()  as f1:
>  #读取
>  with open() as f2:
>    #写入
> ```

#### 2.知识点回顾

> 1.异常
>
> ​	常用的异常
>
> ​	异常的捕获：try-except-finally
>
> ​	自定义异常步骤
>
> 2.文件读写
>
> ​	常用文件：文本文件和二进制文件:read()    write()
>
> ​	csv文件：reader()      writer()

### 二、文件读写

> 在Python中，如果要实现序列化和反序列化，可以使用pickle和json
>
> 【面试题：简述什么是序列化和反序列化】
>
> 序列化：将对象持久化到磁盘上【写：write】,英文表示为pickling,serialiation
>
> 反序列化：将磁盘上的对象读取出来【读：read】,英文表示为unpickling

#### 1.pickle模块

> ```Python
> import  pickle
> 
> """
> pickle提供了简单的持久化功能，可以将对象以文本的形式存储到磁盘上
> pickle只能在Python中使用，
> Python中所有的数据类型【list,tuple,dict,set,str,对象】都可以通过pickle模块持久化到磁盘上
> 
> 注意：通过pickle序列化之后的数据，人一般无法识别，只能计算机识别【区别于乱码】
> """
> 
> class Person(object):
>  def __init__(self,name,age):
>      self.name = name
>      self.age = age
> 
>  def show(self):
>      print("姓名：%s,年龄：%s" % (self.name,self.age))
> 
> p = Person("zhangsan",10)
> 
> #1.以普通文件的方式操作对象
> #缺点：write只能写入字符串
> #f = open(r"file1.txt","w",encoding="utf8")
> #f.write(p)#TypeError: write() argument must be str, not Person
> #f.close()
> 
> #2.思考问题：如果向文件中写入一个对象，该如何做？---》pickle模块
> 
> #2.1序列化【写】
> """
> pickle.dump(obj,file)
>  obj:将要写入文件的对象
>  file：obj将要写入的文件对象，注意：file必须以二进制的方式打开，为wb
> """
> #a。打开文件
> f1 = open(r"obj.txt","wb")
> 
> #b.写入对象
> pickle.dump(p,f1)
> 
> #c.关闭文件
> f1.close()
> 
> 
> #2.反序列化【读】
> """
> pickle.load(file)
>  file：将要读取的文件对象，注意：file必须以二进制的方式打开，为rb
> """
> #a.打开文件
> f2 = open(r"obj.txt","rb")
> 
> #b。读取对象
> result = pickle.load(f2)
> print(result)
> result.show()
> 
> #c.关闭文件
> f2.close()
> 
> """
> w,w+,wb都会覆盖源文件中的内容，
> r，r+,rb都必须保证源文件存在
> w,w+,wb,a如果文件不存在，会自动创建
> """
> ```

#### 2.json模块

> 思考问题：将文本或者二进制数据保存到文件中，使用write操作，如果将一个列表或者字典直接保存到文件中该如何实现？-----》使用json格式保存数据
>
> JSON:JavaScript  Object Notation,本来是javascript语句中创建对象的一种字面量方式，被广泛应用于跨平台的语言的数据交换【因为JSON是纯文本，任何系统任何编程语言都可以处理纯文本】
>
> 使用场景：在两种不同的编程语言之间传递对象，将数据序列化为json，json表示出来就是一个字符串，可以被所有语言读取，也可以存储到磁盘或者通过网络传输
>
> 在web开发中，不仅使用json，还是用xml，但是使用json较多，json更快，而且可以直接在web中读取
>
> Python中的数据类型和json数据类型的区别;
>
> json			Python
>
> object 			dict
>
> array			list
>
> string			str
>
> number                int/float
>
> true/false 		True/False
>
> null   			None
>
> 注意：json和pickle将数据序列化之后的区别
>
> ```Python
> import  pickle
> dict2 = dict(name="jack",age=10,score=100)
> with open(r"pickle1.txt","wb") as f2:
>  pickle.dump(dict2,f2)
> ```
>
> ```Python
> import  json
> 
> #一、基本用法
> #1.写【序列化】
> """
> dump():将Python对象按照json格式序列化到文件中
> dumps()：将Python对象处理成json格式的字符串
> """
> #1.1
> dict1 = dict(name="jack",age=10,score=100)
> print(dict1)
> r1 = json.dumps(dict1)
> print(r1)
> print(type(r1))
> 
> #1.2
> dict2 = dict(name="jack",age=10,score=100)
> with open(r"data1.json","w",encoding="utf8") as f2:
>  json.dump(dict2,f2)
> 
> #2.读【反序列化】
> """
> load():将文件中的json数据反序列化为对象
> loads()：将字符串的内容反序列化为Python对象
> """
> #2.1
> str1 = '{"name": "jack", "age": 10, "score": 100}'
> r1 = json.loads(str1)
> print(r1)
> print(type(r1))
> 
> #2.2
> with open(r"data1.json","r",encoding="utf8") as f2:
>  r2 = json.load(f2)
>  print(r2)
>  print(type(r2))
> 
> 
> #练习：
> #序列化
> def jsonwrite(dict1):
>  with open(r"data2.json","w",encoding="utf8") as f1:
>      json.dump(dict1,f1)
> 
>  print("数据保存成功！")
> 
> #反序列化
> def jsonread():
>  with open(r"data2.json","r",encoding="utf8") as f2:
>      result = json.load(f2)
>      print(result)
> 
> if __name__ == "__main__":
>  mydict = {
>      "name":"杨阳",
>      "age":18,
>      "qq":1736363,
>      "friends":['王大锤',"马化腾"],
>      "cars":[
>          {"brand":"polo","price":100000},
>          {"brand":"五菱宏光","price":50000},
>          {"brand":"qq","price":20000}
>      ]
>  }
>  jsonwrite(mydict)
> 
>  jsonread()
> ```

#### 3.StringIO和BytesIO

> 数据的读写不一定只能在文件中操作，也可以在内存中操作，StringIO在内存中读写字符串，BytesIO在内存中读写字节，字节数据其实就是二进制数据
>
> 注意：StringIO和BytesIO是系统的类
>
> ```Python
> from  io import  StringIO,BytesIO
> 
> #一、StringIO
> #1.写入
> #创建对象
> si = StringIO()
> #写入
> #注意：将数据写入到了内存中
> si.write("hello")
> si.write("Python")
> si.write("2141412")
> 
> #获取写入到内存中的数据
> r1 = si.getvalue()
> print(r1)
> 
> #2.读取
> si2 = StringIO("hello\nPython\n2141412")
> #全部读取
> # r2 = si2.read()
> # print(r2)
> #按行读取
> # r2 = si2.readline()
> # print(r2)
> 
> while True:
>  r2 = si2.readline()
>  if r2 == "":
>      break
> 
>  print(r2)
> 
> #二、BytesIO
> #1.写入
> bi = BytesIO()
> #编码
> # bi.write("中文fahjghahg".encode("utf-8"))
> bi.write(bytes("中文fahjghahg",encoding="utf-8"))
> print(bi.getvalue())
> 
> #2.读取
> bi2 = BytesIO(b'\xe4\xb8\xad\xe6\x96\x87fahjghahg')
> r2 = bi2.read()
> print(r2)
> #解码
> #print(r2.decode("utf-8"))
> print(str(r2,encoding="utf-8"))
> ```

### 三、collections模块

#### 1.namedtuple

> ```Python
> #1.namedtuple
> from  collections import  namedtuple
> """
> tuple是一个有序的集合
> 其中允许存储重复元素，但是，一旦被定义之后，将不可改变
> """
> 
> #需求：使用元组表示一个二维坐标
> #方式一
> tuple1 = (2,4)
> #方式二
> class Point(object):
>  def __init__(self,x,y):
>      self.x = x
>      self.y = y
> print(Point)
> p = Point(2,4)
> print(p.x,p.y)
> p.x = 10
> p.y = 20
> print(p.x,p.y)
> 
> print("*" *20)
> 
> #方式三
> #第一步：导入模块
> #第二步：调用函数，定义了类
> #namedtuple("名称"，[属性])
> Point = namedtuple("Point",["x","y"])
> print(Point)
> p = Point(2,4)
> #第三步：访问属性
> print(p.x,p.y)
> # p.x = 10
> # p.y = 20
> # print(p.x,p.y)
> 
> """
> namedtuple是一个函数，它用来创建一个自定义的tuple对象
> 并且规定了tuple元素的个数，并可以用属性而不是索引访问元组中的元素
> 
> 好处：可以很方便的定义一种新的数据类型，它具备元组的不可变性，又可以通过引用访问属性
> """
> 
> print(isinstance(p,Point))
> print(isinstance(p,tuple))
> 
> 
> Circle = namedtuple("Circle",['x','y','r'])
> ```

#### 2.deque

> ```Python
> from collections import  deque
> 
> 
> """
> 使用list存储数据，按照索引访问元素速度较快，但是，插入和删除的速度较慢，因为list是线性存储
> 
> deque是为了实现高效的插入和删除操作的双向列表
> 
> 添加元素
>  append:在末尾追加/appendleft：在头部添加
> 删除元素
>  pop：删除末尾元素/popleft:删除头部元素
> """
> 
> queue = deque([2,3,4])
> print(queue)
> 
> #添加
> queue.append(5)
> print(queue)
> queue.appendleft(6)
> print(queue)
> 
> #删除
> queue.pop()
> print(queue)
> queue.popleft()
> print(queue)
> ```

#### 3.defaultdict

> ```Python
> from  collections import  defaultdict
> 
> """
> 普通的dict，如果访问了一个不存在的key，则会报出异常KeyError
> """
> dict1 = {"a":1,"b":2}
> v1 = dict1["a"]
> print(v1)
> # v2 = dict1["c"]
> # print(v2)   #KeyError: 'c'
> 
> print(dict1)
> 
> #问题：如果key存在，则获取对应的value，但是如果key不存在，返回一个默认值，需要使用defaultdict
> 
> #defaultdict(有返回值的函数[，字典])
> d = defaultdict(lambda : "aaaa")
> print(d)
> print(type(d))
> 
> #注意：和普通的dict相同，如果key不存在，dict[key] = value则表示将键值对添加到字典中
> d["key1"] = 34
> print(d)
> 
> #如果访问的key不存在，则默认获取的是函数的返回值
> print(d["key2"])
> 
> 
> ```

#### 4.OrderedDict

> ```Python
> from collections import  OrderedDict
> 
> 
> """
> 字典：key是无序的
> """
> 
> #字典的写法
> 
> #1.无序字典
> dict1 = {"a":1}
> print(dict1)
> dict2 = dict(x=1,y=3)
> print(dict2)
> dict3 = dict([("a",1),("b",2),("c",3)])
> print(dict3)
> 
> #2.有序字典
> dict4 = OrderedDict([("a",1),("b",2),("c",3)])
> print(dict4)
> 
> 
> #练习：
> od = OrderedDict()
> od["2"] = 20
> od["1"] = 10
> 
> print(list(od.keys()))
> ```

#### 5.Counter

> ```Python
> from  collections import  Counter
> 
> #需求：统计一个单词中每个字符出现的次数
> data = input("请输入文本：")
> 
> #方式一
> dict1 = {}
> 
> for ch in data:
>  if ch not in dict1:
>      dict1[ch] = 1
>  else:
>      dict1[ch] += 1
> print(dict1)
> 
> #方式二
> #Counter是Collections中提供的一个计数器
> c = Counter()
> for ch in data:
>  c[ch] += 1
> print(c)
> 
> print(type(c))
> print(isinstance(c,Counter))
> print(isinstance(c,dict))
> 
> #Counter实际上是dict的一个子类，专门用来统计可迭代对象个数
> c = Counter()
> for num in [2,3,43,43,3,3,3,3,22,100]:
>  c[num] += 1
> print(c)
> ```

### 四、购物车

> user
>
> ```Python
> """
> 用户类：
> 	姓名  用户id【这个标识对于每个用户而言是唯一的]】    密码
> 	 拥有购物车  用户登录状态【默认为 False 表示没有登录】
> 
> """
> class User(object):
>  def __init__(self,username,password,uid,shoppingcar):
>      self.username = username
>      self.password = password
>      self.uid = uid
>      self.shoppingcar= shoppingcar
>      #默认为False,表示没有登录,如果进行了实际的登录，只需要将该状态 改为True
>      self.islogin = False
> 
>  def __str__(self):
>      return "【User】:%s-%s-%s-%s" % (self.uid,self.username,self.password,self.islogin)
> ```
>
> shoppingcar
>
> ```Python
> """
> 购物车类：
> 	商品列表：程序初始时，商品列表为空
> """
> class ShopingCar(object):
>  def __init__(self):
>      #购物车中的商品以字典的方式存储，商品对象为key，商品的数量作为value
>      self.goodsdict = {}
> 
> 
>  def __str__(self):
>      return "【Shoppingcar】：%s" % (self.goodsdict)
> ```
>
> storage
>
> ```Python
> """
> 仓库类：【信息保存在本地磁盘：程序刚启动时把列表先存储到文件中，之后使用再读取出来】
> 	商品列表
> 	    商品名称    	价格        剩余量
> 		Mac电脑	   	20000       100
> 		PthonBook 	30	  	   200
> 		草莓键盘       80      	   60
> 		iPhone		7000		   70
> """
> import  os,pickle
> from shopcar.goods import Goods
> 
> 
> #不同的用户访问到的仓库应该为同一个，所以将仓库类设置为单例类，保证不管在哪个文件中获取，获取到的都是同一个仓库对象
> def single(cls):
>  instance = None
>  def getinstance(*args,**kwargs):
>      nonlocal  instance
>      if not instance:
>          instance = cls(*args,**kwargs)
>      return instance
>  return getinstance
> 
> @single
> class Storage(object):
>  def __init__(self):
>      self.preparegoods()
> 
>  #如果文件存在，则加载，如果文件不存在，则将代码中的列表存储到文本中
>  def preparegoods(self):
>      if not os.path.exists("goodslist.txt"):
>          #定义一个商品列表，用来存储仓库中的商品对象
>          self.goodslist = []
> 
>          #设置商品
>          names = ["mac电脑","PthonBook","机械键盘","iphone"]
>          prices = [20000,78,800,6666]
>          balances = [100,43,298,555]
> 
>          #遍历列表，获取商品信息，通过信息创建商品对象，将对象添加到商品列表中
>          for i in range(len(names)):
>              goods = Goods(names[i],prices[i],balances[i])
>              self.goodslist.append(goods)
> 
>          #将商品列表序列化到磁盘上
>          self.savegoods()
>      else:
>          #将磁盘上的商品列表读取出来
>          self.loadgoods()
> 
>  #序列化
>  def savegoods(self):
>      with open(r"goodslist.txt", "wb") as f:
>          pickle.dump(self.goodslist, f)
> 
>  #反序列化
>  def loadgoods(self):
>      with open(r"goodslist.txt", "rb") as f:
>          self.goodslist = pickle.load(f)
> ```
>
> goods
>
> ```Python
> """
> 商品类：
> 	商品名称   商品价格   商品剩余量
> """
> class Goods(object):
>  def __init__(self,name,price,balance):
>      self.name = name
>      self.price = price
>      self.balance = balance
>  def __str__(self):
>      return "【goods】：%s-%s-%s" % (self.name,self.price,self.balance)
> ```
>
> operation
>
> ```Python
> import  os,pickle,random
> from shopcar.shoppingcar import ShopingCar
> from  shopcar.user import User
> from  shopcar.storage import Storage
> from shopcar.goods import Goods
> 
> class Operation(object):
>  #当程序启动之后，加载本地的用户文本
>  def __init__(self):
>      self.loadalluser()
> 
>  def loadalluser(self):
>      if not os.path.exists("user.txt"):
>          #如果文件不存在，则定义一个字典，当用户完成注册之后，用于存储用户【uid作为key，用户对象作为value】
>          self.userdict = {}
>      else:
>          with open("user.txt","rb") as f:
>              self.userdict = pickle.load(f)
> 
>  #保存文件
>  def saveuser(self):
>      with open("user.txt", "wb") as f:
>        pickle.dump(self.userdict,f)
> 
>  #产生随机用户id
>  def getuid(self):
>      """
>      问题：用户的id应该是唯一的，但是随机数可能会重复
>      为了避免uid的重复，如果uid在字典中已经存在，则重新获取
>      """
>      while True:
>          uid = str(random.choice(range(10000, 100000)))
>          if uid not in self.userdict:
>              print("用户id已经生成，为：%s" % (uid))
>              return uid
> 
>  #注册
>  def userregister(self):
>      #获取uid
>      uid = self.getuid()
>      #创建购物车的对象
>      sc = ShopingCar()
>      #用户名和密码
>      username = input("请输入用户名：")
>      password = input("请输入密码：")
>      #通过信息创建一个用户对象
>      user = User(username=username,password=password,uid=uid,shoppingcar=sc)
> 
>      #将用户添加到字典中
>      self.userdict[uid] = user
> 
>      #同步到本地文件中
>      self.saveuser()
> 
>  #登录
>  def userlogin(self):
>      uid = input("请输入用户id：")
>      if uid not in self.userdict:
>          print("请先注册")
>          #self.userregister()
>          return
> 
>      #判断用户的登录状态
>      user = self.userdict[uid]
>      if user.islogin:
>          print("已经登录")
>          return user
> 
>      # 实现登录操作
>      while True:
>          pwd = input("请输入登录密码：")
>          if pwd == user.password:
>              print("登录成功")
>              #修改用户的登录状态
>              user.islogin = True
>              return  user
>          else:
>              print("密码错误，请输入正确的密码")
> 
>  #购买商品
>  def addgoods(self):
>      #在添加商品之前，验证用户是否登录成功
>      user = self.userlogin()
>      if user == None:
>          print("请先进行登录，然后购买商品")
>          return
> 
>      print("""仓库中的商品如下：
>      0.Mac电脑
>      1.pythonbook
>      2.机械键盘
>      3.iphone
>      """)
>      #引导用户选择商品
>      index = input("请输入需要购买的商品编号：")
>      if index.isdigit():
>          index = int(index)
> 
>          if index >= 0 and index <= 3:
>              #获取仓库对象
>              storage = Storage()
>              goods = storage.goodslist[index]
> 
>              #引导用户输入需要购买的商品数量
>              num = input("请输入需要购买的商品数量：")
> 
>              if num.isdigit():
>                  num = int(num)
> 
>                  while num > goods.balance:
>                      num = int(input("商品剩余量为：%s,请重新输入需要购买的商品数量：" % (goods.balance)))
>                  else:
>                      #重新实例化商品对象，添加到购物车中
>                      shop_goods = Goods(goods.name,goods.price,num)
>                      user.shoppingcar.goodsdict[shop_goods] = num
> 
>                      #将仓库中的商品的数量修改
>                      goods.balance -= num
> 
>                      #同步商品信息到本地
>                      storage.savegoods()
> 
>                      #同步用户信息到本地
>                      self.saveuser()
>          else:
>              print("商品还未上架")
>      else:
>          print("输入有误")
> 
>  #删除商品
>  def delgoods(self):
>      # 在删除商品之前，验证用户是否登录成功
>      user = self.userlogin()
>      if user == None:
>          print("请先进行登录，然后删除商品")
>          return
> 
>      #引导用户输入需要删除的商品的名称
>      d_name = input("请输入需要删除的商品的名称：")
> 
>      #定义变量，获取购物车中的商品对象
>      shop_goods = None
> 
>      #遍历购物车的字典
>      for key in user.shoppingcar.goodsdict:
>          if key.name == d_name:
>              shop_goods = key
> 
>      if shop_goods == None:
>          print("商品不存在")
>          return
> 
>      #操作仓库
>      #在仓库中获取商品
>      storage = Storage()
>      index = 0
>      for i in range(len(storage.goodslist)):
>          if storage.goodslist[i].name == d_name:
>              index = i
> 
>      #获取商品对象
>      sto_goods = storage.goodslist[index]
> 
>      #引导用户输入需要删除的商品的数量
>      num = int(input("请输入需要删除的商品的数量："))
>      if num >= shop_goods.balance:
>          #将商品对象从列表中直接移除
>          user.shoppingcar.goodsdict.pop(shop_goods)
>          #在仓库中加上
>          sto_goods.balance += shop_goods.balance
>      else:
>          shop_goods.balance -= num
>          sto_goods.balance += num
> 
>      #同步
>      storage.savegoods()
>      self.saveuser()
> 
>  #结算
>  def gettotal(self):
>      user = self.userlogin()
>      if user == None:
>          print("请先进行登录，然后结算购物车")
>          return
> 
>      total = 0
> 
>      for key,value in user.shoppingcar.goodsdict.items():
>          total += key.price * value
> 
>      print("总计为：%s" % (total))
> 
>      #清空购物车
>      user.shoppingcar.goodsdict.clear()
> 
>      self.saveuser()
> 
>  #退出
>  def userexit(self):
>      user = self.userlogin()
>      if user != None:
>          user.islogin = False
>          self.saveuser()
> ```
>
> text
>
> ```Python
> from shopcar.operation import Operation
> 
> op = Operation()
> 
> print("**********欢迎进入xxx自选超市*********")
> 
> while True:
>  print("本超市提供如下功能：\n0.注册  1.登录  2.添加商品 3.删除商品  4.结算购物车  5.退出")
>  num = int(input("请输入你的选择："))
>  if num == 0:
>      op.userregister()
>  elif num == 1:
>      op.userlogin()
>  elif num == 2:
>      op.addgoods()
>  elif num == 3:
>      op.delgoods()
>  elif num == 4:
>      op.gettotal()
>  elif num == 5:
>      op.userexit()
>      break
>  else:
>      print("暂未开通此功能")
> 
> ```

# Day17

### 一、上堂回顾

#### 1.默写题目

> 1.分别封装函数，实现csv文件的读写
>
> ```Python
> import csv
> def readcsv(path):
> with open(path,"r") as f1:
>  result = csv.reader(f1)
>  for data in result:
>    print(data)
> 
> def writecsv(path):
> with open(path,"w") as f2:
>  result = csv.writer(f2)
>  result.writerow("gsg")
>  
>  
> import csv
> #newline默认每行的后面会添加一个空行，如果消除，则给newline重新赋值
> with open(r"file1.csv", "w",newline="") as f2:
>  result = csv.writer(f2)
>  for sublist in [[23,3,545],[56,56,56],[65,6,56,5,6]]:
>      result.writerow(sublist)
> ```
>
> 2.使用不同的方式实现对象的序列化和反序列化
>
> ```Python
> #pickle
> import pickle
> #反序列化
> with open(r"","rb") as f1:
>  result = pickle.load(f1)
> 
> #序列化
> with open(r"","wb") as f1:
>  pickle.dump([],f1)
> 
> #json
> import json
> #反序列化
> with open(r"","r",encoding="utf8") as f1:
>  result = json.load(f1)
> 
> #序列化
> with open(r"","w",encoding="utf8") as f1:
>  json.dump([],f1)
> ```

#### 2.知识点回顾

> StringIO和BytesIO:在内存层面上进行读写
>
> read/write,reader/writer,pickle/json:在磁盘层面上读写

### 二、反射

#### 1.概念

> 通过字符串操作对象中的字段【类的字段：类属性  ，对象的字段的：实例属性     类属性和实例属性】
>
> 反射就是通过字符串的方式，导入模块，去模块中查找指定的函数；去到对象中操作【查找、获取、删除、添加】成员
>
> 本质：是一种基于字符串的驱动

#### 2.使用

> getattr：获取属性
>
> setattr:修改属性的值
>
> hasattr:判断某个属性是否存在
>
> delattr:删除某个属性
>
> ```Python
> class Person(object):
>  country = "CH"
> 
>  def __init__(self,name,age):
>      self.name = name
>      self.__age = age
> 
>  def show(self):
>      print("show")
>  @classmethod
>  def func1(cls):
>      print("111")
>  @staticmethod
>  def func2():
>      print("222")
> 
> #1.以往的用法
> p1 = Person("jack",10)
> print(p1.name)
> 
> #2.反射
> #问题：通过一个字符串"name"获取jack，“age”获取10
> print("name","age")
> 
> #方式一:__dict__
> print(p1.__dict__)
> print(p1.__dict__["name"])
> 
> #方式二：反射
> #getattr(obj,name[,default])获取某个对象的某个字段的值，如果字段不存在，则返回default
> r0 = getattr(p1,"name")
> print(r0)
> #r0 = getattr(p1,"score")  #AttributeError: 'Person' object has no attribute 'score'
> r0 = getattr(p1,"score",100)
> print(r0)
> 
> #私有化属性
> # r0 = getattr(p1,"age")
> # print(r0)
> r0 = getattr(p1,"_Person__age")
> print(r0)
> 
> #类属性
> #对象或者类名访问类属性
> r0 = getattr(Person,"country")
> print(r0)
> r0 = getattr(p1,"country")
> print(r0)
> 
> #成员函数
> r0 = getattr(p1,"show")
> print(r0)
> r0()
> 
> #类函数和静态函数
> r0 = getattr(Person,"func1")
> print(r0)
> r0()
> r0 = getattr(p1,"func1")
> print(r0)
> r0()
> 
> r0 = getattr(Person,"func2")
> print(r0)
> r0()
> r0 = getattr(p1,"func2")
> print(r0)
> r0()
> 
> #3.setattr(obj,name,value)
> p1 = Person("jack",10)
> #p1.name = "zhangsan"
> 
> setattr(p1,"name","zhangsan")
> print(getattr(p1,"name"))
> 
> #4.hasattr(obj,name)
> print(hasattr(p1,"name"))
> print(hasattr(p1,"score"))
> 
> #5.delattr(obj,name)
> delattr(p1,"name")
> #print(getattr(p1,"name"))  #AttributeError: 'Person' object has no attribute 'name'
> ```

#### 3.模块中的反射

> ```Python
> import  reflect02.moduleA
> 
> 
> #1.以往的方式
> print(reflect02.moduleA.num)
> 
> reflect02.moduleA.show()
> 
> a = reflect02.moduleA.A(47)
> 
> #2.反射
> #Python中一切皆对象，模块也是一个对象
> print(getattr(reflect02.moduleA,"num"))
> 
> s = getattr(reflect02.moduleA,"show")
> s()
> 
> A = getattr(reflect02.moduleA,"A")
> print(A)
> r = A(36)
> print(r.a)
> ```
>
> ```Python
> num = 18
> 
> def show():
>  print("aaaaa")
> 
> class A(object):
>  def __init__(self,a):
>      self.a = a
> ```

#### 4.练习

> ```Python
> def video():
>  return "视频"
> def image():
>  return "图片"
> def games():
>  return "游戏"
> def music():
>  return "音乐"
> def movie():
>  return "电影"
> 
> ```
>
> ```Python
> #需求：根据用户输入的内容，执行对应的操作
> 
> import  reflect03.news
> 
> #方式一
> # data = input("请输入你要执行的操作：")
> # if data == "music":
> #     print(reflect03.news.music())
> # elif data == "movie":
> #     print(reflect03.news.movie())
> # elif data == "games":
> #     print(reflect03.news.games())
> # elif data == "image":
> #     print(reflect03.news.image())
> # elif data == "video":
> #     print(reflect03.news.video())
> # else:
> #     print("还未开通此功能")
> 
> #方式二
> data = input("请输入你要执行的操作：")
> 
> result = hasattr(reflect03.news,data)
> if result:
> 
>  f = getattr(reflect03.news,data)
>  print(f())
> else:
>  print("还未开通此功能")
> 
> 
> #总结：反射的好处：可以简化代码，提高了代码的可维护性
> ```

### 三、单元测试和文档测试

#### 1.单元测试

> 指的是对一个函数，一个类或者一个模块来进行正确性的校验工作
>
> 结果：
>
> ​	a.单元测试通过，说明所测试的单元是正常
>
> ​	b.单元测试未通过，要么程序有bug，要么测试的条件有误
>
> ```Python
> def mysum(x,y):
>  return  x + y
> 
> def mysub(x,y):
>  return  x - y
> ```
>
> ```Python
> from  test01.mathfunc import mysum,mysub
> import  unittest
> 
> #1.自定义测试类，继承自unittest.TestCase
> class Test(unittest.TestCase):
>  #2.重写父类中的函数
>  def setUp(self):
>      print("开始测试时自动调用")
>  def tearDown(self):
>      print("结束测试时自动调用")
> 
>  #3.定义成员函数，测试指定的函数
>  #命名格式：test_需要被测试的函数名
> 
>  def test_mysum(self):
>      #使用断言：对函数的结果做一个预判【代入法】
>      #参数:调用原函数的结果   预判的结果  如果预测失败的提示信息
> 
>      #含义：用自己预判的结果和函数的运算结果做比对，如果相等，则说明测试通过
>      self.assertEqual(mysum(1,2),3,"加法有误")
> 
>  def test_mysub(self):
>      self.assertEqual(mysub(2,1),1,"减法有误")
> 
> #4.开始测试
> if __name__ == "__main__":
>  #调用main函数，会触发Test类中所有函数的调用
>  unittest.main()
> 
> ```

#### 2.文档测试

> ```Python
> import  doctest
> 
> def add(x,y):
>  """
>  求两个数的和
>  :param x: 第一个数字
>  :param y: 第二个数字
>  :return: 和
> 
>  example:
>  >>> add(2,3)
>  5
>  """
>  return  x + y
> 
> print(add(10,43))
> 
> #开始进行文档测试
> doctest.testmod()
> 
> #注意：必须严格按照命令行中的格式书写代码
> 
> ```

### 四、排列组合

> ```Python
> #排列：从n个不同的元素中取出m【m <= n】个元素，按照一定的顺序排成一列,
> # 称为从n个元素中获取m个元素的排列【Arrangement】,当.m = n时，则成为全排列【Permutation】
> 
> """
> 例如：
> 1 2 3 4，从中取出3个，排列的方式？
> 123
> 213
> 321
> 312
> 132
> 231
> 
> 123  124  134  234
> """
> import  itertools
> 
> #itertools.permutations(可迭代对象，num)
> result = list(itertools.permutations([1,2,3,4],1))
> print(result)
> 
> print(len(result))
> 
> """
> 4-4   24
> 4-3    24
> 4-2    12
> 4-1    4
> 
> 从n个元素中取出m个元素的排列的可能性：n! / (n - m)!
> """
> 
> ```
>
> ```Python
> #组合：从n个不同的元素中，取出m个元素为一组，叫做从n个不同元素中取出m个元素的组合
> 
> import  itertools
> 
> result = list(itertools.combinations([1,2,3,4],3))
> print(result)
> print(len(result))
> 
> """
> 4-4    1
> 4-3    4
> 4-2     6
> 4-1     4
> 
> 从n个不同元素中取出m个元素的组合的可能性：n！/ (m! * (n -m)!)
> """
> 
> ```
>
> ```Python
> import  itertools
> 
> 
> #验证码
> #
> result = list(itertools.permutations("0123456789",6))
> # #print(result)
> # print(len(result))
> #
> # result = list(itertools.product("0123456789",repeat=6))
> # #print(result)
> # print(len(result))
> 
> #密码
> #result = list(itertools.permutations("0123456789qwertyuioplkjhgfdsazxcvbnm",6))
> #print(result)
> #print(len(result))
> 
> result = list(itertools.product("0123456789qwertyuioplkjhgfdsazxcvbnm",repeat=4))
> #print(result)
> print(len(result))
> 
> ```

### 五、正则表达式

#### 1.案例

> 需求：校验一个qq号的合法性
>
> 需求：校验一个手机号的合法性

#### 2.概念

> 正则表达式：Regular Expression,Python中提供一个模块为re
>
> 使用单个字符串来描述、匹配、查找或者替换指定字符串的操作
>
> 正则表达式的作用：
>
> ​	a.可以匹配：match
>
> ​	b.可以搜索:search,findall
>
> ​	c.可以替换：sub，subn
>
> 注意：正则表达式其实只是一个字符串，该字符串具有一定的规律，使用特定的符号来匹配特定的内容
>
> 使用场景：校验数据【qq号，手机号，身份证号，银行卡号，用户名和密码，邮箱等】
>
> ​    		    爬虫【按照指定的条件将一个网页中的指定的数据筛选出来】	

#### 3.使用

# Day18

### 一、上堂回顾

#### 1.默写题目

> 1.封装函数，使用选择排序实现列表的降序排序
>
> 2.分别获取时间的时间戳，元组形式和字符串形式
>
> 3.书写装饰器，统计一个函数的执行时间

### 二、进程

#### 1.概念

##### 1.1多任务

> 程序的运行都是cpu和内存协同工作的结果
>
> 常用的操作系统都支持“多任务”的操作
>
> 问题1：什么是多任务？
>
> ​	操作系统上同时运行多个任务，除了手动打开的应用程序之外，还有很多的后台程序
>
> 问题2：单核cpu是怎样执行多任务？
>
> ​	操作系统会让多个任务轮流交替执行，由于不同的任务之间的切换速度很快，导致肉眼无法识别
>
> ​	多核cpu实现多任务：真正的并行执行只能在多核cpu上执行，但是现实情况下，任务的数量可能会远远大于cpu的核心数量，操作系统会将每个任务调度，让在每个cpu核心上轮流执行
>
> ​		并行：真正一起执行，任务数量小于cpu的核心数量【理想型】
>
> ​		并发：看上去一起执行，任务数量大于cpu的核心数量【现实型】
>
> 问题3：什么是进程？
>
> ​	对于操作系统而言，一个任务就是一个进程【Process】
>
> ​	例如：打开一个浏览器启动了一个浏览器进程，打开一个word启动了一个word进程，但是，一个进程可以同时干多件事情，
>
> ​	在一个进程的内部，要同时干多件事情，就需要同时执行多个子任务，将一个进程中的多个子任务被称为线程【Thread】

##### 1.2进程

> 是对一个程序的运行状态和占用资源【cpu，内存】的描述
>
> 进程是程序的一个动态过程，它指的是从代码加载到最后代码加载完毕的整个过程
>
> 进程的特点：
>
> ​	a.独立性：不同的进程之间是相互独立的，在操作系统中互不影响，相互之间资源不共享
>
> ​	b.动态性：进程一旦被启动之后，在操作系统中并不是静止不动的，一直处于动态状态
>
> ​	c.并发性：在操作系统上在交替执行
>
> 多任务的实现方式：
>
> ​	a.多进程模式：启动多个进程，每个进程虽然只有一个线程，通过该线程执行一个任务
>
> ​	b.多线程模式：启动一个进程，该进程启动多个线程，每个线程执行一个任务
>
> ​	c.协程模式：yield【函数生成器】
>
> ​	d.多进程模式+多线程模式：启动多个进程，每个进程启动多个线程，执行的任务的数量会更多

#### 2.使用

##### 2.1单任务现象

> ```Python
> import  time
> 
> #单任务：一个函数执行了某个特定的功能
> def run():
>  while True:
>      print("hello")
>      time.sleep(0.5)
> 
> if __name__ == "__main__":
>  while True:
>      print("main")
>      time.sleep(1)
> 
>  run()
> 
> #说明：单任务现象代码从上往下依次执行，前面的代码执行完毕，后面的代码才有执行的机会
> ```

##### 2.2启动进程实现多任务

> ```Python
> import  time,os
> #如果要实现多任务，Python中提供了相应的模块
> #每通过Process创建一个对象，则表示创建一个进程
> from  multiprocessing import  Process
> 
> #子进程中的任务
> def run(s):
>  #os.getpid()获取当前正在执行的进程id
>  #os.getppid(获取当前正在执行进程的父进程id
>  print("子进程启动：%s-%s" % (os.getpid(),os.getppid()))
>  print(s)
>  while True:
>      print("hello")
>      time.sleep(1)
> 
> if __name__ == "__main__":
>  #1.__main__中执行的代码表示主进程，也称为父进程
>  #os.getpid获取当前正在执行的进程id
>  print("主进程启动：%s" % (os.getpid()))
> 
>  #2.在主进程中创建子进程
>  #Process(target,args),target表示子进程需要执行的任务【函数】，args表示需要执行的任务的参数，类型为元组
>  #2.1任务函数没有参数
>  #p1 = Process(target=run)
> 
>  #2.2任务函数有参数
>  #注意：给子进程中的任务传参的时候，函数有几个参数，元组中的元素需要保持一致
>  p1 = Process(target=run,args=("text",))
> 
>  #如果想要启动一个子进程，则必须调用start
>  p1.start()
> 
>  #主进程中的任务
>  while True:
>      print("main")
>      time.sleep(1)
> 
>  run()
> 
> ```

##### 2.3父子进程的执行顺序

> ```Python
> from  multiprocessing import  Process
> import  time,os
> 
> def run():
>  print("子进程启动~~~~~")
>  time.sleep(2)
>  print("子进程结束~~~~~")
> 
> 
> if __name__ == "__main__":
>  print("父进程启动")
>  time.sleep(2)
> 
>  p = Process(target=run)
> 
>  p.start()
> 
>  p.join()
> 
>  print("父进程结束")
> 
> """
> 默认情况下，都是主进程结束之后子进程才启动
> 使用join之后，主进程会等待子进程结束之后才结束
> 
> 注意：join的调用只能在start之后
> """
> ```

##### 2.4多个进程中的全局变量

> 验证多个进程之间的独立性
>
> ```Python
> from  multiprocessing import  Process
> from time import  sleep
> import  os
> 
> #需求：在一个进程中修改全局变量的值，观察另一个进程中全局变量的值的变化
> 
> #全局变量
> num = 100
> 
> def run():
>  print("子进程开始：%s" % (os.getpid()))
>  global  num
>  num += 1
>  print("子进程结束：num=%d" % (num))
> 
> if __name__ == "__main__":
>  print("父进程开始：%s" % (os.getpid()))
> 
>  p = Process(target=run)
>  p.start()
> 
>  p.join()
> 
>  print("父进程结束:num=%d" % (num))
> 
> """
> 说明：在子进程中修改全局变量对父进程中的全局变量没有影响
> 工作原理;在创建子进程的时候，实际上对全局变量做了一个备份，父进程中的num和子进程中的num是两个不同的变量
> 进程是系统中程序执行和系统资源分配的基本单位，每个进程都有自己的数据段，代码段，堆栈段
> 【进程之间是相互独立的，资源不共享】
> """
> ```

##### 2.5启动大量子进程

> 如果要大量的创建子进程，可以使用进程池的方式批量创建子进程
>
> ```Python
> #进程池
> from  multiprocessing import  Pool
> import  os,time,random
> 
> #需求：创建多个子进程，让子进程执行同一个任务，根据传入的参数作为进程的名称进行区分
> 
> def run(name):
>  print("子进程%s启动：%s" % (name,os.getpid()))
> 
>  #通过time计算耗时的时间差
>  start = time.time()
>  time.sleep(random.choice(range(1,4)))
>  end = time.time()
> 
>  print("子进程%s结束，进程号：%s，耗时：%s" % (name, os.getpid(),end - start))
> 
> if __name__ == "__main__":
>  print("父进程启动")
> 
>  #创建多个进程，采用进程池的方式，通过系统类Pool创建多个进程对象
>  #Pool(num),num表示需要同时执行的任务的数量，可以省略，默认为cpu的核心数量
>  p = Pool(8)
> 
>  #通过循环的方式创建多个子进程
>  for i in range(5):
>      #创建子进程，放到进程池统一管理
>      #apply_async(target,args)
>      p.apply_async(run,args=(i,))
> 
>  #必须在join之前调用close，调用close之后将不能再添加新的进程
>  p.close()
> 
>  #进程池对象调用join，触发进程的启动，父进程会等待所有的子进程执行结束之后才结束
>  p.join()
> 
>  print("父进程结束")
> 
> """
> 如果要使用进程池创建多个进程，必须调用close和join
> """
> ```

> 练习：
>
> ```Python
> #需求：实现文件内容的拷贝
> 
> import  os,time
> 
> #实现文件的拷贝
> def copyfile(rpath,wpath):
>  fr = open(rpath,"rb")
>  fw = open(wpath,"wb")
> 
>  content = fr.read()
>  fw.write(content)
> 
>  fr.close()
>  fw.close()
> 
> if __name__ == "__main__":
>  path = r"C:\Users\Administrator\Desktop\text1"
>  topath = r"C:\Users\Administrator\Desktop\text2"
> 
>  #获取path下面的所有的内容
>  filelist = os.listdir(path)
> 
>  start = time.time()
> 
>  for filename in filelist:
>      copyfile(os.path.join(path,filename),os.path.join(topath,filename))
> 
>  end = time.time()
> 
>  print("总耗时：%.2f" % (end - start))
> ```
>
> ```Python
> # 需求：实现文件内容的拷贝
> 
> import os, time
> from  multiprocessing import  Pool
> 
> 
> # 实现文件的拷贝
> def copyfile(rpath, wpath):
>  fr = open(rpath, "rb")
>  fw = open(wpath, "wb")
> 
>  content = fr.read()
>  fw.write(content)
> 
>  fr.close()
>  fw.close()
> 
> 
> if __name__ == "__main__":
>  path = r"C:\Users\Administrator\Desktop\text1"
>  topath = r"C:\Users\Administrator\Desktop\text3"
> 
>  # 获取path下面的所有的内容
>  filelist = os.listdir(path)
> 
>  p = Pool(4)
> 
>  start = time.time()
> 
>  for filename in filelist:
>      #copyfile(os.path.join(path, filename), os.path.join(topath, filename))
>      p.apply_async(copyfile,args=(os.path.join(path, filename),os.path.join(topath, filename)))
> 
>  p.close()
>  p.join()
> 
>  end = time.time()
> 
>  print("总耗时：%.2f" % (end - start))
> ```

##### 2.6封装进程对象

> ```Python
> from  multiprocessing import  Process
> 
> import  os,time
> 
> #1.自定义一个类，继承自Process
> class CustomProcess(Process):
>  #2.书写构造函数，定义实例属性，表示当前进程的名称
>  def __init__(self,name):
>      #3.调用服了你的构造函数
>      Process.__init__(self)
>      self.name = name
> 
>  #4.定义成员函数，任务的执行函数
>  def run(self):
>      print("子进程(%s-%s)启动" % (self.name,os.getpid()))
>      #子进程的功能
>      time.sleep(2)
>      print("子进程(%s-%s)结束" % (self.name, os.getpid()))
> 
> if __name__ == "__main__":
>   print("父进程启动")
> 
>   p = CustomProcess("1111")
>   p.start()
> 
>   p.join()
> 
>   print("父进程结束")
> ```

##### 2.7进程之间的通信

> Process之间是需要相互通信的，操作系统提供了很多的办法实现进程间的通信，Python中的multiprocessing包装了底层的机制，提供了Queue【队列】，Pipes等多种方式实现交换数据
>
> ```Python
> #需求：在主进程中创建两个子进程，一个进程用来向队列中写数据，另外一个进程用来从队列中读数据
> 
> from  multiprocessing import  Process,Queue
> import  os,time,random
> 
> #1.写数据的任务
> def write(queue):
>  print("进程%s开始" % (os.getpid()))
>  print("开始写入")
> 
>  for value in ["A","B","C"]:
>      print("add %s to queue" % (value))
> 
>      #向队列中添加数据
>      queue.put(value)
> 
>      #稍休息片刻，接着加
>      time.sleep(random.random())
> 
>  print("进程%s结束" % (os.getpid()))
> 
> #2.读数据的任务
> def read(queue):
>  print("进程%s开始" % (os.getpid()))
>  print("开始读取")
> 
>  n = 0
>  while n < 3:
>      #从队列中获取数据
>      value = queue.get(True)
>      print("get %s from queue" % (value))
>      n += 1
> 
>  print("进程%s结束" % (os.getpid()))
> 
> #3.在主进程中分别创建子进程，执行相应的任务
> if __name__ == "__main__":
>  print("父进程启动")
> 
>  #3.1创建队列对象，并传参给每个进程
>  q = Queue()
> 
>  #3.2创建进程对象，
>  pr = Process(target=read,args=(q,))
>  pw = Process(target=write,args=(q,))
> 
>  #3.3启动子进程，让进行数据的读写
>  pw.start()
>  pr.start()
> 
>  #3.4设置，让所有子进程结束之后，才结束父进程
>  pr.join()
>  pw.join()
> 
>  print("父进程结束")
> ```

### 二、线程

#### 1.概念

> 是进程的组成部分，一个进程可以有多个线程，每个线程去处理一个特定的子任务
>
> 注意：一个进程至少需要有一个线程，否则该进程没有意义
>
> 线程的执行是抢占式的，多个线程在同一个进程中可以并发执行，其实就是在cpu之间进行快速的切换【每个线程都有争抢时间片的机会，谁抢到时间片，则执行对应的线程，剩下的线程都会被挂起】
>
> ​	例如：打开网易云音乐------》启动一个进程
>
> ​		    播放歌曲和刷新歌词-----》启动了两个线程
>
> 【面试题】进程和线程之间的关系
>
> ​	a.一个程序启动之后至少有一个进程
>
> ​	b.一个进程可以包含多个线程，但是至少需要一个线程，否则该进程没有意义
>
> ​	c.进程之间的资源不共享，线程之间是资源共享的
>
> ​	d.系统创建进程需要为该进程重新分配系统资源，而创建线程容易的多，因此使用多线程实现多任务比多进程实现效率更高

#### 2.创建线程

> ```
> _thread模块：提供了低级别的，原始的线程【低级别并不是不好，只是功能有限，底层采用的c语言】
> threading模块：高级模块，对_thread进行了封装，提供了_thread没有的功能
> 
> ```
>
> ```Python
> import  threading,time
> 
> 
> #2.定义子线程需要执行的任务
> def run(num):
>  print("子线程%s启动" % (threading.current_thread().name))
> 
>  time.sleep(2)
>  print("num=%d" % (num))
> 
>  print("子线程%s结束" % (threading.current_thread().name))
> 
> if __name__ == "__main__":
>  #1.任何进程默认会启动一个线程，称为主线程，在主线程中启动其他的子线程
>  #threading.current_thread()返回一个当前正在执行的线程对象
>  #threading.current_thread().name获取当前正在执行的线程的名称，主线程默认的名称为MainThread
>  print("主线程%s启动" % (threading.current_thread().name))
> 
>  #3.创建子线程
>  #threading.Thread(target,name,args),target需要执行的任务，name表示线程的名称，args执行的任务函数的参数
>  #3.1任务函数没有参数
>  #注意：name也可以省略，每个子线程默认有名称，根据线程被创建的顺序，为Thread-1，Thread-2.....
>  #t1 = threading.Thread(target=run,name="11111")
> 
>  #3.2任务函数有参数
>  t1 = threading.Thread(target=run,args=(10,))
> 
>  #4.手动启动子线程
>  t1.start()
> 
>  #5.想让主线程等待子线程执行结束之后才结束，设置join
>  t1.join()
> 
>  print("主线程%s结束" % (threading.current_thread().name))
> ```

#### 3.线程中的共享数据

> 问题：在多线程中，全局变量被所有线程所共享，所以，任何一个全局变量可以被任何一个线程修改，因此，线程之间共享数据最大的危险在于多个线程同时修改同一个变量，容易将数据改乱
>
> ```Python
> #需求：使用一个全局变量代表银行卡余额，两个线程都可以访问银行卡的余额
> 
> from  threading import  Thread
> 
> balance = 0
> 
> def change(n):
>  global balance
>  balance = balance + n
>  balance = balance - n
> 
> #子线程的任务
> def run(n):
>  for _ in range(1000000):
>      change(n)
> 
> if __name__ == "__main__":
> 
>  t1 = Thread(target=run,args=(5,))
>  t2 = Thread(target=run,args=(8,))
> 
>  t1.start()
>  t2.start()
> 
>  t1.join()
>  t2.join()
> 
>  #理论上，balance最终的结果为0
>  print(balance)
> 
> """
> 问题：
>  先加后减，理论上结果为0，但是，如果访问的次数变多，则结果不一定为0
> 
> 原因：
>  使用多线程容易出现的临界资源问题
>  高级语言中一条语句分步执行的，所以balance = balance + n在内存中执行的顺序是：
>      a.计算balance + n，将结果存储到一个临时变量中   x = balance + n
>      b.将临时变量的值赋值给balance   balance = x
> 
>  1.正常情况下
>      t1:x = balance + n  #5
>      t1:balance = x   #balance = 5
>      t1:x = balance - n   #0
>      t1:balance = x    #0
> 
>      t2:x = balance + n  #8
>      t2:balance = x   #balance = 8
>      t2:x = balance - n   #0
>      t2:balance = x    #0
> 
>  2.实际情况下：
>      t1:x1 = balance + n  #x1 = 5
> 
>      t2:x2 = balance + n   #x2 = 8
>      t2: balance = x2    #balance = 8
> 
>      t1:balance = x1   #balance = 5
>      t1:x1 = balance - n  #x1 = 0
>      t1:balance = x1   #balance = 0
> 
>      t2:x2 = balance - n #x2 = -8
>      t2:balance = x2   #balance = -8
> 
>  总结：修改balance需要多条语句，执行多条语句的时候，线程随时可能会被中断，从而导致多个线程将一个变量修改乱了
> 
> 解决：上锁【给多线程中的临界资源上一把锁，当一个线程访问的时候，其他的线程则必须在锁外面进行等待，直到锁被释放之后，
> 其他线程才有再次争抢时间片的机会】
> """
> ```

#### 4.线程锁

> ```Python
> from  threading import  Thread,Lock
> 
> balance = 0
> 
> #创建一个锁对象
> lock = Lock()
> 
> def change(n):
>  global balance
>  balance = balance + n
>  balance = balance - n
> 
> #子线程的任务
> def run(n):
>  for _ in range(1000000):
>      #获取锁
>      lock.acquire()
> 
>      try:
>          # 临界资源
>          change(n)
>      finally:
>          #释放锁
>          lock.release()
> 
> 
> if __name__ == "__main__":
> 
>  t1 = Thread(target=run,args=(5,))
>  t2 = Thread(target=run,args=(8,))
> 
>  t1.start()
>  t2.start()
> 
>  t1.join()
>  t2.join()
> 
>  #理论上，balance最终的结果为0
>  print(balance)
> ```
>
> ```Python
> from  threading import  Thread,Lock
> 
> balance = 0
> 
> #创建一个锁对象
> lock = Lock()
> 
> def change(n):
>  global balance
>  balance = balance + n
>  balance = balance - n
> 
> #子线程的任务
> def run(n):
>  for _ in range(1000000):
>      #同样表示获取锁，但是，不用手动释放，当临界资源的代码执行完毕之后，锁会被自动释放
>      with lock:
>          # 临界资源
>          change(n)
> 
> if __name__ == "__main__":
> 
>  t1 = Thread(target=run,args=(5,))
>  t2 = Thread(target=run,args=(8,))
> 
>  t1.start()
>  t2.start()
> 
>  t1.join()
>  t2.join()
> 
>  #理论上，balance最终的结果为0
>  print(balance)
> ```

# Day19

### 一、上堂回顾

> 1.进程和线程的概念
>
> ​	进程：启动一个应用程序【独立性，动态性，并发性】
>
> ​	线程：在一个进程中，处理不同的子任务，每个子任务可以开启一个线程【资源共享，并发性】
>
> ​	一个应用程序启动之后至少有一个进程，一个进程启动之后至少有一个线程
>
> ​	进程间是相互独立的，资源不共享的，线程之间是资源共享
>
> ​	系统创建进程比创建线程更加困难，需要系统重新分配系统资源
>
> 2.实现多任务的方式：
>
> ​	多进程模式，多线程模式，协程模式，多进程+多线程模式
>
> 3.使用
>
> ​	进程：multiprocessing模块，Process类
>
> ​	线程：threading模块，Thread类
>
> ​		启动：start()
>
> ​		执行顺序：join()

### 二、线程

#### 1.ThreadLocal

> 在多线程环境下，每个线程都有自己的数据，一个线程使用自己的局部变量比使用全局变量好，因为局部变量只能当前线程自己看到，其他的线程访问不了，如果一个线程修改自己的局部变量，不会影响其他的线程，而全局变量则需要添加锁
>
> 问题：局部变量在函数调用的时候，传递起来比较麻烦
>
> ```Python
> from  threading import  Thread,local
> 
> #全局变量
> num = 0
> 
> #创建一个全局的ThreadLocal对象
> #每个线程都有自己独立的存储空间，每个线程对ThreadLocal对象都可以读写，但是互不影响
> threadlocal = local()
> 
> def run(x,n):
>  x = x + n
>  x = x - n
> 
> def func(m):
>  """
>  全局变量threadlocal就是一个ThreadLocal对象，每个Thread都可以对他进行读写操作，但是互不影响
>  threadlocal.x对于每个线程而言，相当于是一个局部变量，
>  每个线程可以进行任意的读写而互不干扰，也不需要管理锁
> 
> 说明：threadlocal.x中的x可以是任意的，只要是一个合法的标识符即可，还可以绑定其他的变量，threadlocal.y,threadlocal.z。。。。。
>  """
>  threadlocal.x = num
> 
>  for _ in range(1000000):
>      run(threadlocal.x,m)
> 
> if __name__ == "__main__":
>  t1 = Thread(target=func,args=(6,))
>  t2 = Thread(target=func, args=(9,))
>  t1.start()
>  t2.start()
>  t1.join()
>  t2.join()
> 
>  print(num)
> 
> """
> 在多线程中处理临界资源【全局变量】，为了避免数据混乱，解决办法：
>  a.加锁【1手动加锁和释放锁  2.使用with自动加锁和释放锁】
>  b.使用ThreadLocal对象将全局变量修改为线程的局部变量
> 
> ThreadLocal的作用 ：解决了参数在一个线程中各个函数之间的传递问题
> """
> ```

#### 2.栅栏【屏障】

> ```Python
> from  threading import  Barrier,current_thread,Thread
> import  time
> 
> #Barrier:栅栏或者屏障
> 
> #Barrier类设置了一个线程数量的障碍，当等待的线程达到了这个数量则会唤醒所有的等待线程
> 
> #凑够一定的数量才执行
> 
> bar = Barrier(2)
> 
> def run():
>  print("%s---start" % (current_thread().name))
> 
>  time.sleep(2)
> 
>  #当前线程进入阻塞状态【等待状态】
>  bar.wait()
> 
>  print("%s---end" % (current_thread().name))
> 
> if __name__ == "__main__":
>  for _ in range(5):
>      Thread(target=run).start()
> 
> 
> #工作原理：每个线程进来就等待，不够num个则阻塞，直到够num个唤醒所有的线程，开闸放行
> ```

#### 3.定时线程

> ```Python
> import  threading
> 
> def run():
>  print("hfjahfahgj")
> 
> if __name__ == "__main__":
>  print("父线程启动")
> 
>  #创建定时线程【延时线程】并启动
>  #threading.Timer(time,target)
>  t = threading.Timer(5,run)
>  t.start()
> 
>  t.join()
> 
>  print("父线程结束")
> ```

#### 4.线程通信【生产者消费者设计模式】

> 为什么要使用生产者和消费者设计模式？
>
> ​	在线程的环境中，生产者就是生产数据的线程，消费者就是消费数据的线程，在实际的多线程开发中，如果生产者的处理速度快，但是消费者处理速度慢，那么生产者等待消费者处理完，才能继续生产数据，同样，生产者的处理速度慢，但是消费者处理速度快，消费者同样需要等待，这样引入生产者消费者设计模式
>
> 什么是生产者和消费者设计模式？【面试题】
>
> ​	生产者消费者设计模式是通过一个容器来解决生产者和消费者之间的强耦合问题，让生产者和消费者彼此之间不直接沟通，而是通过阻塞队列完成通讯，所以生产者生产完数据之后不用等待消费者处理完，直接扔给阻塞队列，消费者也不用找生产者要数据，直接从阻塞队列中获取，阻塞队列相当于是一个缓冲区，平衡了生产者和消费者之间的处理能力
>
> ​	阻塞队列就是用来给生产者和消费者进行解耦【符合大多数设计模式的设计思路】
>
> ```Python
> import  threading,time,random,queue
> 
> #需求：多个线程向队列中添加数据，多个线程从队列中获取数据
> 
> #生产者
> def product(id,queue):
>  while True:
>      num = random.randint(0,10000)
>      queue.put(num)
>      print("生产者%s向队列中添加了%s" % (id,num))
>      time.sleep(2)
>  #当任务完成，
>  queue.task_done()
> 
> #消费者
> def consumer(id,queue):
>  while True:
>      item = queue.get()
>      if item is None:
>          break
>      print("消费者%s从队列中获取%s" % (id, item))
>      time.sleep(2)
>  queue.task_done()
> 
> if __name__ == "__main__":
>  #阻塞队列
>  q = queue.Queue()
> 
>  #启动生产者
>  for i in range(4):
>      threading.Thread(target=product,args=(i,q)).start()
> 
>  # 启动消费者
>  for i in range(4):
>      threading.Thread(target=consumer, args=(i, q)).start()
> ```

### 三、协程

#### 1.概念

> 函数：在Python中，函数之间的调用一般都是层级调用，例如：A调用B，在B执行的过程中调用C,C执行完毕返回，B执行完毕返回，最后A执行完毕返回【函数的入栈和出栈】，是通过栈实现的，一个线程就是执行一个子程序，子程序调用总是一个入口，一次返回，调用的顺序是明确的
>
> 一个子程序在执行的过程中可以中断，然后转而去执行别的子程序，和函数的调用有区别
>
> 协程的好处：和线程相比，协程的执行效率较高，因为只有一个线程，也不会出现变量冲突的情况，在协程中的资源不需要加锁，只需要判断状态
>
> 协程最大的特点：控制函数的阶段性执行，节约线程或者进程的切换
>
> 协程其实就是特殊的线程，实际上就是一个函数生成器
>
> ```Python
> #函数调用
> def a():
>  print("aaaa")
>  b()
>  print("aaaa~~~~")
> def b():
>  print("bbbb")
>  c()
>  print("bbbb~~~~")
> def c():
>  print("cccccc")
> 
> a()
> 
> #执行顺序：aaaa---->bbbb--->cccc--->bbbb~~~~--->aaaaa~~~
> ```

#### 2.工作原理

> ```Python
> #yield关键字
> 
> """
> Python对协程的支持就是通过生成器实现的
> """
> 
> def run():
>  print(1)
>  yield 10
>  print(2)
>  yield 20
>  print(3)
>  yield 30
> 
> """
> 协程最大的特点：控制函数的阶段性执行，节约线程或者进程的切换
> 
> 协程其实就是特殊的线程，实际上就是一个函数生成器
> """
> m = run()
> print(m)
> print(next(m))
> print(next(m))
> print(next(m))
> 
> ```

#### 3.数据传输

> ```Python
> def run():
>  data = ""
> 
>  r = yield  data
>  #r = "11"
>  print(1,r,data)
>  r = yield "aa"
>  #r = "22"
>  print(2, r, data)
>  r = yield "bb"
>  print(3, r, data)
>  r = yield "cc"
> 
> #协程中的数据传输：从外加向生成器中传递数据，通过yield返回
> m = run()
> #启动协程
> print(m.send(None))
> print(m.send("11"))
> print(m.send("22"))
> print(m.send("33"))
> ```

#### 4.生产者消费者设计模式

> ```Python
> def product(c):
>  c.send(None)
>  for i in range(5):
>      print("生产者生成了%s" % (i))
>      r = c.send(str(i))
>      print("消费者消费了%s" % (r))
> 
>  #关闭
>  c.close()
> 
> def consumer():
>  data = ""
>  while True:
>     n =  yield  data
>     if not n:
>         return
>     print("消费者消费了%s" % (n))
>     data = 100
> 
> c = consumer()
> product(c)
> ```