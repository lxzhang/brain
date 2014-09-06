Pro Pandoc Markdown
===================

<link rel="stylesheet" href="../../_hl/v1/default.css">
<script src="../../_hl/v1/highlight.pack.js"></script>
<script>hljs.initHighlightingOnLoad();</script>




~~~ {.bash}
echo "# Hello Pandoc" | pandoc.exe
pandoc.exe < README > README.html
pandoc.exe README -o README.pdf
~~~

On some inline code `echo bash code`{.bash}
`echo `{.bash}


`<h1 id="hello-pandoc">Hello Pandoc</h1>`


### Test Codes

~~~~~~ {#codetag .python .numberLines .startFrom="20"}
import ogr 
driver = ogr.GetDriverByName('PDF') 
dataSource = driver.Open('test.shp', 0) 
layer = dataSource.GetLayer() 
layer.GetFeatureConut(), layer.GetExtent() 
feature = layer.GetFeature(0)
dataSource.Destroy()
~~~~~~

random text with tag {#texttag}


**Auto numbered list**

#. one
#. two


 9)  Ninth
10)  Tenth
11)  Eleventh
       i. subone
      ii. subtwo
     iii. subthree




Term 1

:   Definition 1

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.



(@)  My first example will be numbered (1).
(@)  My second example will be numbered (2).

Explanation of examples.

(@逗你玩)  My third example will be numbered (3).
Numbered examples can be labeled and referred to elsewhere in the document:

(@)  This is a good example.

As (@逗你玩) illustrates, ...






  Right     Left     Center     Default
-------     ------ ----------   -------
     12     12        12            12
    123     123       123          123
      1     1          1             1

Table:  Demonstration of simple table syntax.



-------     ------ ----------   -------
     12     12        12             12
    123     123       123           123
      1     1          1              1
-------     ------ ----------   -------

### Title with hash(good) {#good}

-------------------------------------------------------------
 Centered   Default           Right Left
  Header    Aligned         Aligned Aligned
----------- ------- --------------- -------------------------
   First    row                12.0 Example of a row that
                                    spans multiple lines.

  Second    row                 5.0 Here's another one. Note
                                    the blank line between
                                    rows.
-------------------------------------------------------------

Table: Here's the caption. It, too, may span
multiple lines. {#table}


elipses...




1--8
that is --- fabulous

_good underscore_


<span style="font-variant:small-caps;">Small caps</span>

$$x^y=z$$

$$E=mc^2$$


**four kinds of titles**

[one][my label 1], and [two][my label 2] and [three][my label 3] and [four][my label 4]

[my label 1]: /foo/bar.html  "My title, optional"
[my label 2]: /foo
[my label 3]: http://fsf.org (The free software foundation)
[my label 4]: /bar#special  'A title in single quotes'

[my website][]  is good, even [my website] is good, even [this]. 

### Hashe

* See [above]
* See [table](#table)
* See [codetag](#codetag)


[my website]: /shit
[good]: /bar/baz <good>
[this]: /baz
[above]: #good



Image in a paragraph ![inline-pic-without-showing-this-text]


![standalone-pic-displayed-with-this-text]



Here is a footnote[^1], or this kind of footnote[^footnote]



Here is an inline note.^[Inlines notes are easier to write, since
you don't have to pick an identifier and move down to type the
note.]



[^1]: good, you are smart
[^footnote]: this foot note...



[inline-pic]: http://gnat-tang-shared-image.qiniudn.com/emoji/11.gif
[standalone-pic]: http://gnat-tang-shared-image.qiniudn.com/emoji/33.gif




---

**Refs**

* [Pandoc Markdown Official Site](http://johnmacfarlane.net/pandoc/demo/example9/pandocs-markdown.html)
* [The pandoc-siteproc package](http://hackage.haskell.org/package/pandoc-citeproc)

