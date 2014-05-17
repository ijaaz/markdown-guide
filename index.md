Markdown Syntax
===============

## Introduction

Once upon a time, there used to way to edit text, Rich Text, and just Simple
Text.

People who used Rich Text had to use special editors(Microsoft Word, etc.),
they also had special formats, like .docx, that made it almost impossible to
use non-specialty editors.

But even though you had to use a specialty Rich Text editor, it was all fine,
becuse you could have specially formated text, images, colors, and all
different other thing to spruce up your Text, thing that Simple Text did not
have. 

Simple Text was just that simple, there was no way to really display it
differently or make it look different then it really was, nor could you add
photos, or links. 

And then there was programming, you could definitely use something like html (a
web standard way to display text that had formating) and have all of the
formating and pictures of cats you'd ever want, while at the same time, you
could use any editor you wanted.

But HTML is bulky, and doesn't really work well with a lot of writing, I mean
whoever wants to write something like `<h2>` every time he wanted a header.

And then there is latex, now latex is the god of text formating; most
professors use it for mathimatical formulas, that's the formulas that aleks
uses. 

You can take a latex paper and convert it into pdf, and more. The possibilities
endless. And the good thing about latex is that it works on any text editor
(unlike Rich Text), but the problem is that it is hard to use, after all it's
basically programming. Who want's to program at the same time as writing
a document , not many.

So someone thought, oh boy, why dont we really simplify things, and make
something that everyone could use iregardless of text editor(no need for rich
text editors, like microsoft word), or coding ability(latex, html).

So they(this is all just from my imagination) saw that when people where text
or mailing each other, they where sometimes using a simple syntax to enhance
their text, an example would be empasizing some text by surrounding it with
times symbols (get it, it's times impportant) like this: `*this is extra
powerful*`.

They also noticed that HTML was perfect as a way to display formating, as it is
global and works on any machine.

HTML was already being used as a way to format pdf's, and ebooks.

if you ever look inside an ebook, you'd be surprised to find that it's
basically a collection of html files and a pictures.

So they wrote a small script (specifically a perl script, don't worry if you
don't know what that is) that took a text file, looked for special symbols
(like a couple strong symbols surrounding some text), then converted that text
to html. 

You could then use some other tools to make that html into a pdf, ebook, or
more specifically just use it in a website.

So this is the grand beginning of Markdown.

It is now ubiquitus, with a multitude of editors supporting Markdown, even
though you don't need any special editor to write markdown, a lot of editors
specifically made for markdown have their own html converters built in, they
also may have a way to imidiatly convert to a pdf, and other such goodies,
including Cloud sync.

If you are interested in Markdown, I recommend you check out these editor made
for markdown.

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



