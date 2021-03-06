# HTLM初识

HTLM(Hyper Text Markup Language)

- HTML 指的是超文本标记语言 (**H**yper **T**ext **M**arkup **L**anguage)
- HTML 不是一种编程语言，而是一种标记语言 (markup language)
- 标记语言是一套标记标签 (markup tag)

总结： HTML 作用就是用标记标签来描述网页，把网页内容在浏览器中展示出来。 

## HTML结构
```html
<html>
	<head>
        <title></title>
    </head>
    <body>
    </body>
</html>
```

## HTML标签关系

1.嵌套关系

```html
<head>
    <title></title>
</head>
```

2.标签分类

双标签

```html
<body></body>
```

单标签

```html
<br/>
```

3.并列关系

```html
<head></head>
<body></body>
```

## 文档类型

```html
<!DOCTYPE html>
```

## 字符集

```html
<mate charset="UTF-8" />
```

## HTML标签的语义化
所谓的语义化,就是指标签的含义.
为什么要有语义化标签?
1. 方便代码的阅读和维护
2. 同时让浏览器或是网络爬虫可以很好地解析，从而更好分析其中的内容 
3. 使用语义化标签会具有更好地搜索引擎优化 

核心：合适的地方给一个最为合理的标签。

语义是否良好： 当我们去掉CSS之后，网页结构依然组织有序，并且有良好的可读性。

白话，一眼看去，就知道那个是重点，结构是什么，知道每块的内容是干啥的。

遵循的原则：先确定语义的HTML ，再选合适的CSS。
## HTML常用标签
### 排版标签
排版标签主要和CSS搭配使用,显示网页结构的标签,是网页布局最常用的标签.
### 标题标签
为了使网页更具有语义化，我们经常会在页面中用到标题标签，HTML提供了6个等级的标题，即
h1-h6(heading)
```html
<h1>我是一级标题</h1>
<h2>我是二级标题</h2>
<h3>我是三级标题</h3>
<h4>我是四级标题</h4>
<h5>我是五级标题</h5>
<h6>我是六级标题</h6>
```
### 段落标签
(paragraph)
```html
<p>我是一个段落</p>
```
### 水平线标签
horizontal
```html
<hr/>
```
### 布局标签
div span 是没有语义的 是我们网页布局主要的2个盒子 
div就是division的缩写.
### 文本格式化标签
```html
<strong>粗体</strong>
<em>斜体</em>
<del>删除线</del>
<ins>下划线</ins>
```
## 标签属性
使用HTML制作网页时，如果想让HTML标签提供更多的信息，可以使用HTML标签的属性加以设置。其基本语法格式如下：
```html
<标签名 属性1="属性值1" 属性2="属性值2" …> 内容 </标签名>
```
在上面的语法中，

1.标签可以拥有多个属性，必须写在开始标签中，位于标签名后面。

2.属性之间不分先后顺序，标签名与属性、属性与属性之间均以空格分开。

3.任何标签的属性都有默认值，省略该属性则取默认值。

## 图像标签
image
该语法中src属性用于指定图像文件的路径和文件名，他是img标签的必需属性。
```html
<img src="图像URL" />
```
<img src="images/img.png">

## 链接标签
anchor
在HTML中创建超链接非常简单，只需用标签环绕需要被链接的对象即可，其基本语法格式如下：
```html
<a href="跳转目标" target="目标窗口的弹出方式">文本或图像</a>
```
href：用于指定链接目标的url地址，当为标签应用href属性时，它就具有了超链接的功能。  Hypertext Reference的缩写。意思是超文本引用
target：用于指定链接页面的打开方式，其取值有_self和_blank两种，其中_self为默认值，_blank为在新窗口中打开方式。

**注意:**

1.外部链接 需要添加 http:// www.baidu.com

2.内部链接 直接链接内部页面名称即可 比如 < a href="index.html"> 首页 </a >

3.如果当时没有确定链接目标时，通常将链接标签的href属性值定义为“#”(即href="#")，表示该链接暂时为一个空链接。

4.不仅可以创建文本超链接，在网页中各种网页元素，如图像、表格、音频、视频等都可以添加超链接。
### 锚点定位
通过创建锚点链接，用户能够快速定位到目标内容。
创建锚点链接分为两步：
```html
1.使用“a href=”#id名>“链接文本"</a>创建链接文本（被点击的）
  <a href="#two">   

2.使用相应的id名标注跳转目标的位置。
  <h3 id="two">第2集</h3> 
```
### base标签
base可以设置整体链接的打开状态<br/>
base写到```<head>  </head>```之间

把所有的连接 都默认添加 target="_blank"
### 特殊字符标签
<img src="images/zifu.png">

### 注释标签
在HTML中还有一种特殊的标签——注释标签。如果需要在HTML文档中添加一些便于阅读和理解但又不需要显示在页面中的注释文字，就需要使用注释标签。其基本语法格式如下：
```html
 <!-- 注释语句 -->   ctrl + /       或者 ctrl +shift + / 
```
