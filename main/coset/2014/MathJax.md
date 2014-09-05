MathJax Notes
=============

### What is MathJax?

* Open-source JS display engine
* Modular, load components only when necessary
* Rich API


### Getting Started

* Using the MathJax Content Delivery Network (CDN)
* Add these to your src code (.html or .md)

	<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

* MathJax hosted on GitHub: [mathjax | MathJax](https://github.com/mathjax/MathJax/)
* TeX and LaTeX input
    * display: `$$...$$` or `\[...\]`
	* inline: `\(...\)` (default) or `$...$`
* MathML, etc.


### Installing and Testing MathJax

For later reading


### Loading and Configuring MathJax

For later reading


### Common Configurations

Use `default.js` or use this request:

    <script type="text/javascript" src="path-to-MathJax/MathJax.js?config=default"></script>

	
### Using MathJax in popular web platforms

For later reading


### MathJax TeX and LaTeX Support

Note that the TeX input processor implements only the **math-mode** macros of TeX and LaTeX, not the **text-mode** macros.

In Markdown, the back-tick (`) is used to mark **verbatim text**

And sometime you may double backslashs to escape
    
	\\begin{array}{cc}
      a & b \\\\
      c & c
    \\end{array}

You can use the `\def`, `\newcommand`, `\renewcommand`, `\newenvironment`, `\renewenvironment`, and `\let` commands to **create your own macros and environments**.



### Some Examples I Tried

First, new a .md file, see `try-mathjax.md`, and add these lines:

~~~
Try MathJax
===========

<title>About Pandoc Markdown</title>
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
~~~

**Define Macros**

on the page

~~~
We'll define our own macros and use them, $$
   \def\RR{\bf R}
   \def\bold#1{\bf #1}
   \bold{``bold\ face"}$$
And do that again: \(\bold{``bold\ face"}\)
And do that again: $$\bold{``bold\ face"}$$
And do that again: $$\bold{``bold  face"}$$
~~~

And you could create a file in `MathJax/config/local` called `local.js`
that contains your macro definitions:

~~~
MathJax.Hub.Config({
  TeX: {
    Macros: {
      RR: "{\\bf R}",
      bold: ["{\\bf #1}",1]
    }
  }
});

MathJax.Ajax.loadComplete("[MathJax]/config/local/local.js");
~~~

and then load it along with your main configuration file on the script that loads MathJax.js:

    <script src="/MathJax/MathJax.js?config=TeX-AMS_HTML,local/local.js"></script>

	
**Automatic Equation Numbering**

~~~
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  TeX: { equationNumbers: { autoNumber: "AMS" } }
});
</script>

$E=mc^2$

Numbered Eqns:

$$
   \begin{equation}
   E = mc^2 
   \end{equation}$$

Not Numbered Eqns:

$$
\begin{equation*}
   e^{\pi i} + 1 = 0
\end{equation*}$$	
~~~	
	
~~~
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  TeX: {
    Macros: {
      RR: "{\\bf R}",
      bold: ["{\\bf #1}",1]
    }
  }
});
</script>

Displayed: $$\RR$$ and $$\bold{bold}$$

Inline: \(\RR\) and $\bold{bold}$
~~~	


~~~
* Use `\(...\)`: \(x^y=z\) (now work, both cases)
* Use `\[...\]`: \[x^y=z\] (not work, both cases)
* Use `$...$`: $x^y=z$ (without `--mathjax`, works; with `--mathjax`, works better)
~~~


http://alexgorbatchev.com/SyntaxHighlighter/




---

**Refs**

* [MathJax Document](http://docs.mathjax.org/en/latest/mathjax.html)
