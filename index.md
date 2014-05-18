Markdown Syntax
===============

Introduction
-----------

Once upon a time, there used to way to edit text, Rich Text, and just Simple
Text.

People who used Rich Text had to use special editors(Microsoft Word, etc.),
they also had special formats, like .docx, that made it almost impossible to
use non-specialty editors.

But even though you had to use a specialty Rich Text editor, it was all fine,
because you could have specially formated text, images, colors, and all
different other thing to spruce up your Text, thing that Simple Text did not
have. 

Simple Text was just that, simple, there was no way to really display it
differently(at least without programming), nor could you add photos, or links. 

And then there was programming; you could definitely use something like HTML (a
web standard way to display text that had formating) and have all of the
formating and pictures of cats you'd ever want, while at the same time, you
could use any editor you wanted.

But HTML is bulky, and doesn't really work well with a lot of writing, I mean
whoever wants to write something like `<h2>` every time he wanted a header.

And then there is latex, now latex is the god of text formating; most
professors use it for mathematical formulas, that's the formulas that aleks
uses. 

You can take a latex paper and convert it into pdf, and more. The possibilities
are endless. And the good thing about latex is that it works on any text editor
(unlike Rich Text), the problem is that it is hard to use, after all it's
basically programming. Who want's to program at the same time as writing
a document, not many.

So someone thought, oh boy, why don't we really simplify things, and make
something that everyone could use iregardless of text editor(no need for Rich
Text editors, like Microsoft Word), or coding ability(latex, html).

So they saw that when people were texting or emailing each other, they were
sometimes using a simple syntax to enhance their text, an example would be
emphasising some text by surrounding it with times symbols (get it, it's times
impportant) like this: `*this is extra powerful*`.

They also noticed that HTML a perfect way to display formating, as it is global
and works on any machine.

HTML was already being used as a way to format pdf's, ebooks, and more.

if you ever look inside an ebook, you'd be surprised to find that it's
basically a collection of html files and pictures.

So they wrote a small script(specifically a perl script, don't worry if you
don't know what that is) that took a text file, looked for special symbols
(like a couple strong symbols surrounding some text), then converted that text
to html. 

You could then use some other tools to make that html into a pdf, ebook,
Microsoft Word document, or more specifically just use it in a website.

So that is the grand beginning of Markdown.

It is now ubiquitous, with a multitude of editors supporting Markdown.

Though you don't need any special editor to write markdown, a lot of editors
specifically made for markdown have their own html converters built in, they
also may have a way to immediately convert to a pdf, and other such goodies,
including Cloud sync.

If you are interested in Markdown, I recommend you check out these editor made
for markdown.

* [nvALT](http://brettterpstra.com/projects/nvalt/), it's free, and really cool
* [Byword](http://bywordapp.com/), this one is not free, but it's minimalistic,
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

You can also write header 1's like this
=======================================

And header 2's like this
------------------------
```

It will then be converted to:

```html
<h1>Header 1</h1>
<h2>Header 2</h2>
<h3>Header 3</h3>
<h4>Header 4</h4>
<h5>Header 5</h5>
<h6>Header 6</h6>
<h1>You can also write header 1's like this</h1>
<h2>And header 2's like this</h2>
```

Which will be displayed like this:

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
You can also write header 1's like this
=======================================

And header 2's like this
------------------------

hint: This is a start of a new section
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

Images are typed like this:

```markdown
![ImageCaption](path/to/image.png)
```

It will then be converted to this HTML:

```html
<img href="path/to/image.png" alt="My Alt Text"/>
```

Which Will be displayed in the browser like this:

![ImageCaption](path/to/image.png)


Emphasis
--------


Lists
-----

Lists are actually the easiest to understand, as they are actually written
exactly as they would normally be written.

This is an unorderd list:
```markdown
* I'm a list item
* I'm another list item

- I can actually also be written like this

+ Or like this
```

That in HTML would look like this:

```html
<ul>
  <li>I'm a list item</li>
  <li>I'm another list item</li>
  <li>I can actually also be written like this</li>
  <li>Or like this</li>
```

And would be displayed like this:

* I'm a list item
* I'm another list item

- I can actually also be written like this

+ Or like this

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

