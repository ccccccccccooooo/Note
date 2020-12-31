# 1.html语法规范

## 1.1 基本语法概述

1.HTML标签是<font color=red>由尖括号包围的关键词</font>,例如<font color=red>\<html\>。</font>

2.HTML标签<font color=red>通常是成对出现的</font>，例如\<html\>和\</html\>，我们称为<font color=red>**双标签**。</font>标签对中的第一个标签是开始标签，第二个标签是结束标签。

3.有些特殊的标签必须是单个标签（极小情况），例如\<br/\>,我们称为<font color=red>**单标签**</font>

## 1.2标签关系

双标签关系可以分为两类：<font color=red>包含关系</font>和<font color=red>并列关系</font>

<font color=red size=5>**包含关系**</font>

```html	
<head>
    <title></title>
</head>
```

<font color=red size=5>**并列关系**</font>

```html
<head></head>
<body></body>
```

## 2.1第一个HTML网页

每个网页都会有一个基本结构标签（也称为骨架标签），页面内容也是在这些基本标签上书写。HTML页面也称为HTML文档

```html	
<html>
    <head>
        <title>我的第一个页面</title>
    </head>
    <body>
        Hello World!
    </body>
</html>
```



| 标签名          | 定义       | 说明                                                   |
| --------------- | ---------- | ------------------------------------------------------ |
| <html></html>   | HTML标签   | 页面中最大的标签，我们称为根标签                       |
| <head></head>   | 文档的头部 | 注意在head标签中我们必须要设置的标签是title            |
| <title></title> | 文档的标题 | 让页面拥有一个属于自己的网页标签                       |
| <body></body>   | 文档的主体 | 元素包含文档的说有内容，页面内容基本都是放到body里面的 |

### VSCode工具生成骨架标签新增代码

1. \<!DOCTYPE\> 标签

   \<!DOCTYPE\> 文档类型声明，作用就是告诉浏览器使用哪种HTML版本来显示网页

2. lang 语言

   用来定义当前文档显示的语言。

   2.1 en定义语言为英语

   2.2 zh-CN定义语言为中文

   简单来说，定义为en就是英文网页，定义为zh-CN就是中文网页

   其实对于文档显示来说，定义成en的文档也可以显示中文，定义成zh-CN的文档也可以显示英文

3. charset 字符集

字符集（Character set）是多个字符的集合。以计算机能够识别和存储各种文字。

在\<head\>标签内，可以通过<font color=red>\<meta></font>标签的<font color=red>charset</font>属性来规定HTML文档应该使用哪种字符编码。

```html
<meta charset="UTF-8"/>
```

charset常用的值有:GB2312、BIG5、GBK和UTF-8，其中<font color=red>UTF-8</font>也被称为<font color=red>万国码</font>，基本包含了全世界所有国家需要用到的字符。

# 3. HTML常用标签