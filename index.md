Markdown Syntax
===============

## Introduction

Once upon a time, there used too be two types of text, rich text, and just
simple text.

People who used rich text had to use special editors, they also had special
formats, like .docx, that made it almost impossible to use non-specialty
editors.

But even though ypou had to use a specialyty rich text editor, it was all fine,
becuse you could have specially formated text, images, colors, and all
different other thing to spruce up typu text , thing that simple text did not
have. 

simple text was just that simple, there was no way to really display it
diffeerent ly ot r make it lok different that it really was, not could uoy add
photos. 

And then there was programming, you could definitely use something like html (a
web standard was of display text) and have all of the formating and pictures of
cats you'd ever want, while at the same time, you could us eanyeditor you
wanted. But HTML is bulky , and doesnt really work well  with
a lot of writing, I mean whoevet wants to write somnething like `<h2>` everey
time he wanted a heade.

And then there is latex, now latex is the god of text formating,; most
professors use it for math, that's the math that aleks uses. Yoy can teake
a latex paper and convert it into pdf, and more, the possibiltyis endless. And
the good thing about latex is that it works on anny text editor ( unlike Rich
text) , but the problem it s that it is hard to use, and it's basically
programming. Who want's to program at the same time as writing a dociument
(perhape me, pub thats a personal issue), not many.

So people thought oh boy , why dont we really simplify things, and amek
something that everyone could use iregardless of text editor(no need for rich
text editors, like microsoft word), or coding
ability(latex, html).

So thgey saw that when people wheere text or mailing each other, they where
sometimes using a simple syntax to enhanse thiere message, an example would be
empasising some text by surround ing it with times symbols (you get it, it;s
times impportant) like this: `*this is extra powerful*`.

They then noticed that HTML was perfect as a way to display formating, and that
html was already being used this was for pdf's, and for ebooks, if you ever
look inside a ebook, you's be surprised to find that it's bascically
a collection of html files, and amaypbe a couple pictures.

So they wrote a small script (specifically a perl script, don't worry if you
don't know what that is) that took a text file, looked for special symbols
(like a couple strong symbol surround somme text), and then converted that text
to html. 

You could then use some other tools to make that html into a pdf, or ebook, or
more specifically just use it in a website.

So this is the grand beginning of Markdown, the person who thougt this up is
[ name ].

It is now ubiquetuss , qwit a multitued of editors supporting Markdown, even
though you don't need any speciall editor to write markdown, a lot of editors
specifically made for markdown have there own converter builtin, anbd other
such goodies, including Cluoud sync.

If you are interestid in Markdown, I recomend you check out these editor made
for markdown

* (NVAlt)[http://brettterpstra.com/projects/nvalt/], it's free, and really cool
* (Byword)[http://bywordapp.com/], this one is not free, but it's minimalistic,
    and good for beginners




Headers
-------

You write headers like this:

```markdown
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

It will then be converted to:

```html
<h1>Header 1</h1>
<h2>Header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
```

Which will be displayed like this:

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6



Links
-----

You type links like this:

```markdown
[Text](http://link.com)
```

It will then be converted to this:

```html
<a href=http://link.com>Text</a>
```

Which will be displayed as: [Text](http://link.com)



Images
------


Emphasis
--------

Lists
-----

Code Spans
-----------

Blockquotes
----------

Blockquotes are a way to display blocks of code without the markdown enterpeter
interfering with it. Sometimes people use a special javascript library to
highlight different languages with specific colors, a good example of a js
library that does this is called [highlight.js](http://highlightjs.org/)


    ```function get (attr) {
      return function (object) { return object[attr]; }
    }

    var inventory = {
      apples: 0,
      oranges 144,
      eggs: 36
    };

    get('oranges')(inventory)
    ```

The output for this in html is:

```html
<blockquote>
function get (attr) {
  return function (object) { return object[attr]; }
}

var inventory = {
  apples: 0,
  oranges 144,
  eggs: 36
};

get('oranges')(inventory)
</blockquote>
```

And this is what it looks like in the browser:

```javascript
function get (attr) {
  return function (object) { return object[attr]; }
}

var inventory = {
  apples: 0,
  oranges 144,
  eggs: 36
};

get('oranges')(inventory)
```



