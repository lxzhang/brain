# MathJax Basic

Tags: MathJax LaTeX

> [戳我的作业部落-本文][this]
>
> [戳我的作业部落-文档目录](https://github.com/district10/brain/tree/master/_data/zybuluo)

---

[TOC]

## **1. Symbols**

### **Operators**

| Operators | LaTeX |
| :-------: | :---: |
| $\pm\mp$ | \pm\mp |
| $\times\div$ | \times\div |
| $\cdot\ast$ | \cdot\ast |
| $\star\dagger\diamond$ | \star\dagger\diamond |
| $\vee\wedge$ | \vee\wedge |
| $\oplus\ominus\otimes\circ$ | \oplus\ominus\otimes\circ |
| $\setminus$ | \setminus |
| $\wr$ | \wr |
| $\sqrt{x}$ | \sqrt{x} |


### **Relations**

| Relations | LaTeX |
| :-------: | :---: |
| $\le\ge\neq$ | \le\ge\neq |
| $\sim\ll\gg\doteq\simeq$ | \sim\ll\gg\doteq\simeq |
| $\subset\supset\approx\asymp\subseteq\supseteq$ | \subset\supset\approx\asymp\subseteq\supseteq |
| $\in\ni$ | \in\ni |
| $\smile$ | \smile |
| $\propto$ | \propto |
| $\dashv\vdash$ | \dashv\vdash |
| $\mid\perp\parallel$ | \mid\prep\parallel |
| $\nmid$ | \nmid |


### **Greek Letters**

See Brain


### **Misc**

| Other Symbols | LaTeX |
| :-----: | :---: |
| $\ldots\vdots\cdots\ddots$ | \ldots\vdots\cdots\ddots |
| $\hat{x}\check{x}\dot{x}\breve{x}\acute{x}\ddot{x}\grave{x}\tilde{x}\mathring{x}\bar{x}\vec{x}$ | \hat{x}\check{x}\dot{x}\breve{x}\acute{x}\ddot{x}\grave{x}\tilde{x}\mathring{x}\bar{x}\vec{x} |
| $\vec{\jmath}\tilde{\jmath}$ | \vec{\jmath}\tilde{\imath} |
| $\widehat{3+x}\widetilde{abc}$ | \widehat{3+x}\widetilde{abc} |
| $\infty\triangle\angle$ | \infty\triangle\angle |
| $\aleph\hbar\imath$ | \aleph\hbar\imath |
| $\ell\wp$ | \ell\wp |
| $\Re\Im$ | \Re\Im |
| $\mho\prime$ | \mho\prime |
| $\flat\natural\sharp\$ | \flat\natural\sharp |
| $\surd\partial\top\bot\forall\neg$ | \surd\partial\top\bot\forall\neg |
| $\S$ | \S |



## **Exponents and Subscripts**

* `_` for subscript, `^` for exponents
* e.g. $2^a_i$


## **Fraction**

* `\frac`: $\frac{2}{x+2}$
* `dfrac`: $\dfrac{2}{x+2}$
* `cfrac`: $\cfrac{2}{1+\cfrac{2}{1+\cfrac{2}{1+\cfrac{2}{1}}}}$


## **Radicals**

* `\sqrt`: $\sqrt{2}$
* `\sqrt[n]{x}`: $\sqrt[n]{x}$


## **Sums, Products, Limits and Logarithms**

* `\sum`: $\sum_{i=1}^{\infty}\frac{1}{i}$
* `\prod`: $\prod_{n=1}^5\frac{n}{n-1}$
* `\lim`: $\lim_{x\to\infty}\frac{1}{x}$
* `\log`: $\log_n n^2$


## **Mods**

* `\bmod`: $9\equiv 3 \bmod{6}$
* `\pmod`: $9\equiv 3 \pmod{6}$
* `\mod`: $9\equiv 3 \mod{6}$
* `\pod`: $9\equiv 3 \pod{6}$


## **Combinations**

* `\binom`: $\binom{n-1}{r-1}$
* `\dbinom`(in display mode): $\dbinom{9}{3}$

## **Trigonometric Functions**

Symbols: 

* `\cos\sin\tan\sec\csc\cot`
* `\arccos\arcsin\arctan`
* `\cosh\sinh\tanh\coth`

Examples:

* $\cos^2 x +\sin^2 x = 1$
* $\cos 90\circ = 0$


## **Calculus**

* `\frac`: $\frac{d}{dx}\left(x^2\right) = 2x$
* `\int`, `\,dx`: $\int 2x\,dx = x^2+C$
* `\partial`: $\frac{\partial^2U}{\partial x^2} + \frac{\partial^2U}{\partial y^2}$
* `\oint`: $\frac{1}{4\pi}\oint_\Sigma\frac{1}{r}\frac{\partial U}{\partial n} ds$


## **Overline and Underline**

* `\overline`: $\overline{a+b\imath}$
* `\underline`: $\underline{431}$


## **Matrices**

**Example 01:**

The characteristic polynomial $f(\lambda)$ of the $3 \times 3$ matrix $$
\left(
\begin{array}{ccc}
a & b & c \\
d & e & f \\
g & h & i \end{array}
\right)
$$ is given by the equation $$ f(\lambda)$ = \left|
\begin{array}{ccc}
\lambda - a & -b & -c \\
-d & \lambda - e & -f \\
-g & -h & \lambda - i \end{array}
\right|.
$$

TeX Code: 

~~~
\begin{array}{ccc}
11 & 12 & 13 \\
21 & 22 & 23 \\
31 & 32 & 33
\end{array}
~~~

**Example 02:**

The characteristic polynomial $f(\lambda)$ of the $3 \times 3$ matrix $$
\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
$$ is given by the equation $$
f(\lambda)
= \begin{vmatrix}
\lambda - a & -b & -c \\
-d & \lambda - e & -f \\
-g & -h & \lambda - i
\end{vmatrix}.
$$

TeX Code:

~~~
\begin{pmatrix}
...
\end{pmatrix}
\begin{vmatrix}
...
~~~

**Example 03:**

$$
f(x) = \left\{ \begin{array}{ll}
x+7 & \mbox{if $5< x$};\\
x^2-3 & \mbox{if $-3 \le x \le 5$};\\
-x & \mbox{if $x < -3$}.\end{array} \right. 
$$

TeX Code:

~~~
\begin{array}{ll}
line 1
line 2
\end{array}
~~~

**Example 04:**

$$ 
f(x) = \begin{cases}
x+7 & \text{if $5< x$}; \\
x^2-3 & \text{if $-3 \le x \le 5$};\\
-x & \text{if $x < -3$}.
\end{cases}
$$

TeX Code:

~~~
f(x) = \begin{cases}
x+7 & \text{if $5< x$}; \\
x^2-3 & \text{if $-3 \le x \le 5$};\\
-x & \text{if $x < -3$}.
\end{cases}
~~~


**Text Styles in Math Mode**

MathBB

* `\mathbb`: $\mathbb{R}\mathbb{Z}\mathbb{Q}$
* `\mathbf`: $\mathbf{R}\mathbf{Z}\mathbf{Q}$
* `\mathcal`: $\mathcal{R}\mathcal{Z}\mathcal{Q}$
* `\mathfrak`: $\mathfrak{R}\mathfrak{Z}\mathfrak{Q}$





---

**See also**


**Refs**

* http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Symbols
* http://www.artofproblemsolving.com/Wiki/index.php/LaTeX:Commands
* http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference


[this]: https://www.zybuluo.com/gnat-xj/note/30681