About Pandoc Markdown {.title}
==============================

<title>About Pandoc Markdown</title>
<link rel="stylesheet" type="text/css" href="https://gist.githubusercontent.com/district10/ad8cdbf68052b70cddf0/raw/qiniu-css-pandoc-intro.css"></link> 


I. Normal Markdown {.h2 .section}
---------------------------------

### 1. Emphasis {.h3}

Use **bold**, or *italic (slanted)* to emphasis in Markdown. 
Or ***both*** if you want to.

### 2. Lists {.h3}

**Ordered List**

1. Stay hungry
2. Stay foolish

**Not Ordered List**

* All work and no play
* makes Jacky a dull boy

**Nested List**

1. one
2. two
    * two-one
	* two-two
3. three
    1. three-one
	2. three-two
	
### 3. Table {.h3}

| Key | Value | Notes |
| :---: | ---: | ---: |
| Foo | *fool* | * 第一列居中 |
| **Bar** | barbaric | 第二列右对齐 |
| Cup | cap cup c u ***dummy*** | 第三列左对齐 | 

似乎对齐有点问题

### 4. Quotes {.h3 #quotes}

Here is a quotation from [*Terminator 2*](http://www.imdb.com/character/ch0000933/quotes)

> The future has not been written. There is no fate but what we make for ourselves. I wish I could believe that. My name is John Connor, they tried to murder me before I was born, when I was 13 they tried again. Machines from the future. Terminators. All my life my mother told me the storm was coming, Judgment Day, the beginning of the war between man and machines. Three billion lives would vanish in an instant, and I would lead what was left of the human race to ultimate victory. It hasn't happened, no bombs fell, computers didn't take control, we stopped Judgment Day. I should feel safe, but I don't, so I live off the grid - no phone, no address, no one and nothing can find me. I've erased all connections to the past, but as hard as I try I can't erase my dreams, my nightmares. 


### 5. MISC {.h3}

**All Headers, H1-H6**

# Header 1 {.h1}
## Header 2 {.h2}
### Header 3 {.h3}
#### Header 4 {.h4}
##### Header 5 {.h5}
###### Header 6 {.h6}



II. Pandoc Markdown {.h2 .section}
----------------------------------

### 1. More Emphasis {.h3}

**上下标，删除线：**

* ~~2^^10^^ = 2014~~
* 2^^10^^ = 1024
* H~2~O 是生命之源


### 2. MathJax {.h3}

Do you know [**Euler $\Phi$-function**][euler-phi-function] ?

And, how about Einstein's $$E = mc^2$$

还可以是一个矩阵：

$$
\begin{bmatrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2 \\
\end{bmatrix}
$$

这个也不行。。。


### 3. Inline HTML（Markdown 中使用 HTML 标记） {.h3}

下面是一个 `<div style="background-color=violet">` 的 HTML 标记：

<div style="background-color:violet">
<p style="background-color:black;color:white;margin:10px;">
一个“黑纸白字”的段落</p>
<p>
你可以用 HTML 标记来<b>加粗</b>、<i>斜体</i>或者改变文字的
<font style="color:red">颜色</font>、
<font style="font-size:20px">字号</font>、
<font style="font-family:Impact,Georgia,Serif;">font</font> family
还可使用 Markdown，如下：
</p>

<div markdown="1" style="background-color:yellow;margin:10px;">
**注**：这些文字在一个 `<div markdown="1" style="background-color:yellow;margin:10px;">` 中用 Markdown 写成

可以 **加粗** 也可以 *斜体*

甚至可以使用 Pandoc Markdown 的上下标（以及列表）：
        
* ~~2^^10^^ = 2014~~
* 2^^10^^ = 1024
* H~2~O 是生命之源

| Key | Value | Notes |
| :------: | -------: | -------: |
| Foo | *fool* | * 第一列居中 |
| **Bar** | barbaric | 第二列右对齐 |
| Cup | cap cup c u ***dummy*** | 第三列左对齐 | 

</div>
</div>



### 4. MISC {.h3}

还可以设置页面内链接，点 [**我**](#quotes) 回到 Quotes 小节

And 

###### by the way, I like Gist {.i-like-gist}

这个标题通过在存在 Gist 上的一个 [CSS 文档][css] 来设置了颜色和字体。
事实上本文的 CSS 都放在了 Gist 上。Amazing!!!


III. 源码透析 {.h .section}
---------------------------


### 1. 本文的 Markdown 源码 {.h3}

<script src="https://gist.github.com/district10/caf9df9de0d41a97589e.js"></script>

### 2. 本文的 CSS 源码 {.h3}

<script src="https://gist.github.com/district10/ad8cdbf68052b70cddf0.js"></script>

### 3. Pandoc 转换后的 HTML 文档 {.h3}

<script src="https://gist.github.com/district10/d1f2fd07d4d95549b5fc.js"></script>



---

**Refs**

* [我的简书首页](http://www.jianshu.com/users/faa44ac9e895/latest_articles "因为不能交叉引用，那里有本文的Refs")


[css]: https://gist.github.com/district10/ad8cdbf68052b70cddf0
[euler-phi-function]: http://en.wikipedia.org/wiki/Euler%27s_totient_function