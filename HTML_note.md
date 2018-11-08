# HTML笔记

--------
## HTML元素

-HTML 元素以开始标签起始
-HTML 元素以结束标签终止
-元素的内容是开始标签与结束标签之间的内容
-某些 HTML 元素具有空内容（empty content）
-空元素在开始标签中进行关闭（以开始标签的结束而结束）
-大多数 HTML 元素可拥有属性

-------

## HTML属性

类似于`<a href="http://www.runoob.com">这是一个链接</a>`
其中`href="http://www.runoob.com"`就是一个属性

-HTML 元素可以设置属性
-属性可以在元素中添加附加信息
-属性一般描述于开始标签
-属性总是以名称/值对的形式出现，比如：name="value"。

### 常用属性
属性|描述
---------|----------
class	|为html元素定义一个或多个类名（classname）(类名从样式文件引入)
id	|定义元素的唯一id
style	|规定元素的行内样式（inline style）
title	|描述了元素的额外信息 (作为工具条使用)

--------

## HTML标题

### HTML标题
`标题（Heading）是通过 <h1> - <h6> 标签进行定义的.`

### HTML水平线

`<hr> 标签在 HTML 页面中创建水平线。`

### HTML注释

`<!-- 这是一个注释 -->`

## HTML文本格式化
### HTML文本格式化标签

标签|描述
-----|-------
<b>	|定义粗体文本
<em>|	定义着重文字
<i>	|定义斜体字
<small>|	定义小号字
<strong>|	定义加重语气
<sub>	|定义下标字
<sup>	|定义上标字
<ins>	|定义插入字
<del>	|定义删除字

### HTML"计算机输出" 标签
标签|描述
-----|-------
<code>	|定义计算机代码
<kbd>	|定义键盘码
<samp>	|定义计算机代码样本
<var>	|定义变量
<pre>	|定义预格式文本


### HTML 引文, 引用, 及标签定义
标签|描述
-----|-------
<abbr>	|定义缩写
<address>|	定义地址
<bdo>	|定义文字方向
<blockquote>|	定义长的引用
<q>	|定义短的引用语
<cite>	|定义引用、引证
<dfn>	|定义一个定义项目。

## HTML链接
### HTML超链接
`<a href="url">链接文本</a>`
图片链接
```
<p>创建图片链接:
<a href="//www.runoob.com/html/html-tutorial.html">
<img  border="10" src="smiley.gif" alt="HTML 教程" width="32" height="32"/></a></p>
```
### HTML链接 - target 属性

使用 target 属性，你可以定义被链接的文档在何处显示。
`<a href="http://www.runoob.com/" target="_blank">访问菜鸟教程!</a>`

### HTML 链接- id 属性
id属性可用于创建在一个HTML文档书签标记。
在HTML文档中插入ID:

`<a id="tips">有用的提示部分</a>`
在HTML文档中创建一个链接到"有用的提示部分(id="tips"）"：

`<a href="#tips">访问有用的提示部分</a>`
或者，从另一个页面创建一个链接到"有用的提示部分(id="tips"）"：

`<a href="http://www.runoob.com/html/html-links.html#tips">
访问有用的提示部分</a>`

### HTML电邮链接
在进行邮件内容发送时，需要使用关键字：mailto<br>

示例如下：
`<a href="mailto:zhangrr601@163.com?subject=这是邮件的主题&body=这是邮件的内容" rel="nofollow">发送邮件</a>`
关于创建电子邮件链接时如何进行抄送，密送.<br>

在进行抄送时，需要使用关键字：cc<br>

在进行密送时，需要使用关键字：bcc<br>

示例如下：
`<a href="mailto:zhangrr601@163.com?cc=someone@163.com&bcc=somebody@163.com" rel="nofollow">发送邮件</a>`
参数说明：
参数|描述
-----|------
mailto:name@email.com|	邮件接收地址
cc=name@email.com	|抄送地址
bcc=name@email.com	|密件抄送地址
subject=subject text|	邮件主题
body=body text	|邮件内容
?	|第一个参数分隔符
&	|其他参数分隔符

注：多个邮件地址用 ; 隔开，空格用 %20 代替。

抄送：

英文名称：Carbon Copy，又简称为 CC。在网络术语中，抄送就是将邮件同时发送给收信人以外的人，用户所写的邮件抄送一份给别人，对方可以看见该用户的 E-mail。同收件人地址栏一样，不可以超过 1024 个字符。一般来说，使用"抄送"服务时，多人抄送的电子邮件地址使用 ; 分隔。

密件抄送：

英文名称：Blind Carbon Copy ，又称“盲抄送”，和抄送的唯一区别就是它能够让各个收件人无法查看到这封邮件同时还发送给了哪些人。密件抄送是个很实用的功能，假如一次向成百上千位收件人发送邮件，最好采用密件抄送方式，这样一来可以保护各个收件人的地址不被其他人轻易获得，二来可以使收件人节省下收取大量抄送的 E-mail 地址的时间。

## HTML头部
```
<head> 元素包含了所有的头部标签元素。在 <head>元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种meta信息。
可以添加在头部区域的元素标签为: <title>, <style>, <meta>, <link>, <script>, <noscript>, and <base>.
```
### HTML <title> 元素
<title> 元素:

定义了浏览器工具栏的标题
当网页添加到收藏夹时，显示在收藏夹中的标题
显示在搜索引擎结果页面的标题

### HTML <base> 元素
<base> 标签描述了基本的链接地址/链接目标，该标签作为HTML文档中所有的链接标签的默认链接:
```
<head>
<base href="http://www.runoob.com/images/" target="_blank">
</head>
```

### HTML <link> 元素
<link> 标签定义了文档与外部资源之间的关系。

<link> 标签通常用于链接到样式表:
```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```

### HTML <style> 元素

<style> 标签定义了HTML文档的样式文件引用地址.

在<style> 元素中你也可以直接添加样式来渲染 HTML 文档:
```
<head>
<style type="text/css">
body {background-color:yellow}
p {color:blue}
</style>
</head>
```

### HTML <meta> 元素
```
meta标签描述了一些基本的元数据。

<meta> 标签提供了元数据.元数据也不显示在页面上，但会被浏览器解析。

META 元素通常用于指定网页的描述，关键词，文件的最后修改时间，作者，和其他元数据。

元数据可以使用于浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他Web服务。

<meta> 一般放置于 <head> 区域

为搜索引擎定义关键词:
```

`<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript">`
为网页定义描述内容:

`<meta name="description" content="免费 Web & 编程 教程">`
定义网页作者:

`<meta name="author" content="Runoob">`
每30秒钟刷新当前页面:

`<meta http-equiv="refresh" content="30">`

### HTML <script> 元素

`<script>标签用于加载脚本文件，如： JavaScript。`