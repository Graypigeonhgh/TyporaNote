#  markdown语法快速入门（Typora为例）



## 一.markdown简介

​		Markdown 是一种轻量级标记语言，创始人为约翰·格鲁伯（John Gruber）。 它允许人们使用易读易写的纯文本格式编写文档，然后转换成有效的 XHTML（或者HTML）文档。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。由于 Markdown 的轻量化、易读易写特性，并且对于图片，图表、数学式都有支持，许多网站都广泛使用 Markdown 来撰写帮助文档或是用于论坛上发表消息。 如 GitHub、Reddit、Diaspora、Stack Exchange、OpenStreetMap 、SourceForge、简书等，甚至还能被使用来撰写电子书。(来自百度百科)



## 二.markdown语法



###  1.代码块：

~~~java
~~~语言类型
//~：为1键左边的键（语言类型可写可不写）
~~~

~~~java
//例：java代码块
public static void main(String[] args){
    System.out.println("hello world");
}
~~~



###  2.标题：

~~~java
# 一级标题	
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

分别对应Typora快捷键：
Ctrl + 1
Ctrl + 2
......
Ctrl + 6

// 标题共有6级（#后记得加空格！！！）
//以下举例为 引用 + 标题 的格式
~~~

> # 一级标题

> > ## 二级标题

> > > ### 三级标题

> > > > #### 四级标题

> > > > > ##### 五级标题

> > > > > > ###### 六级标题



### 3.字体：

~~~java
*斜体*
**加粗**
***粗斜体***

或者如下：
_斜体_
__加粗__
___粗斜体___

==代码高亮显示==
~~删除线~~
<u>下划线</U>		(类似html写法)
脚注[^脚注]
~~~

*斜体*
**加粗**
***粗斜体***

或者如下：
_斜体_
__加粗__
___粗斜体___

==代码高亮显示==
~~删除线~~

<u>下划线</u>

脚注[^脚注]



###  4.区块引用:

~~~java
>Hey GrayPigeonHGH!
>>Hey GrayPigeonHGH!
>>Hey GrayPigeonHGH!
>>>Hey GrayPigeonHGH!
>>>Hey GrayPigeonHGH!
~~~

>Hey GrayPigeonHGH!
>>Hey GrayPigeonHGH!
>>Hey GrayPigeonHGH!
>>
>>>Hey GrayPigeonHGH!
>>>Hey GrayPigeonHGH!



### 5.列表:

#### 5.1  有序列表

~~~java
//数字.空格  （按回车键自动添加序号，类似于Word的排版）
1. 有序列表1
2. 有序列表2
3. 有序列表3
~~~

1. 有序列表1
2. 有序列表2
3. 有序列表3

#### 5.2 无序列表

~~~java
// -空格 或 *空格
- 无序列表1
- 无序列表2
* 无序列表3
* 无序列表4
~~~

- 无序列表1
- 无序列表2
* 无序列表3
* 无序列表4

5.3 列表嵌套

~~~java
1. 列表1
	- 列表2
		- 列表3
			- 列表4
- 列表2
	- 列表3
		- 列表4 
~~~

1. 列表1
   - 列表2
     	- 列表3
     		- 列表4

- 列表2
	- 列表3
		- 列表4



### 6.表格:

~~~java
|  表头   | 表头  | 表头 | 表头 |
| --- | :---:  | --: | :---- |
| 单元格  | 单元格 |单元格|单元格|
| 单元格  | 单元格 |单元格|单元格|

：分别实现了以上的左对齐，居中，左对齐，右对齐（默认为左对齐）
快捷键：鼠标右键+插入+表格
~~~

| 表头   |  表头  |   表头 | 表头   |
| ------ | :----: | -----: | :----- |
| 单元格 | 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 | 单元格 |



### 7.分割线:

~~~java
//以下都为分割线语法：
***
****
___	(三个减号)
_ _ _
~~~

***

___

_ _ _

****



### 8.图片插入:

~~~java
方式一： ![图片描述，可写可不行](图片地址)    快捷键：Ctrl+K
//在线图片填链接(不建议)，本地图片填地址，无双引号，也可直接托入或复制粘贴
//图片描述：可以方便搜索引擎根据图片描述里面的关键词搜索到图片

方式二： ![图片](图片地址"optional tital")
//optional tital:鼠标悬置于图片上会出现的标题文字，可以不写
(注意斜杠方向)

例1：![个人主页]（D:\TyporaNote\image\1.png)
例2：![个人主页]（\TyporaNote\image\1.png"optional tital")
~~~

例1：![个人主页](\TyporaNote\image\1.png)

例2：![个人主页](\TyporaNote\image\1.png "optional tital")



### 9.超链接插入:

~~~java
[超链接名称](超链接地址)
[CSDN](https://www.csdn.net/)
~~~

[CSDN](https://www.csdn.net/)



### 10.插入单选框（待办事项）

~~~java
- [ ] 待办事项1
- [ ] 待办事项1
- [ ] 待办事项1
- [x] 待办事项1
- [x]待办事项1
// []中间，[]与文本间都要加空格，加x表示已完成
~~~

- [ ] 待办事项1
- [ ] 待办事项1
- [ ] 待办事项1
- [x] 待办事项1
- [x] 待办事项1



### 11.转义

~~~java
可以在符号前面加上反斜杠" \ "来帮助插入普通的符号
**GrayPigeonHGH**
\**GrayPigeonHGH**
***
\***
~~~

**GrayPigeonHGH**
\**GrayPigeonHGH**
***
\***

### 12.公式

~~~java
// $...$ 中的数学表达式将会在行内显示。
// $$...$$ 中的数学表达式将会在块内显示。
f(x) = sing(x+4) + 12
$f(x) = sing(x+4) + 12$
$$f(x) = sing(x+4) + 12$$
$\sum_{n=1}^{100} n$
$$\sum_{n=1}^{100} n$$

//表达式在块内显示:$$(+回车键)
$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$
~~~





$f(x) = sing(x+4) + 12$

$$f(x) = sing(x+4) + 12$$

$\sum_{n=1}^{100} n$
$$\sum_{n=1}^{100} n$$


$$
\begin{Bmatrix}
   a & b \\
   c & d 
\end{Bmatrix}
$$


### 13.支持HTML

~~~html
<font type="黑体" color=#ffffff size=10> GrayPigeonHGH </font>
~~~

<font type="黑体" color=#g0b6cf size=10> GrayPigeonHGH </font>



## 三.总结

> 本文简单总结了markdown语言的语法使用，希望能对广大读者有所帮助。

参考网站：[菜鸟教程](https://www.runoob.com/markdown/md-tutorial.html)

