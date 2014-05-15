Markdown Syntax
===============

Markdown a way to have the best of both world's. Markdown is just text, than
it's compiled to HTML.

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

Which will be displayed as:

[Text](http://link.com)



Images
------


Emphasis
--------

Lists
-----

Blockquotes
-----------

Code Spans
----------

Blockquotes are a way to display blocks of code without the markdown enterpeter
interfering with it.  Sometimes people use a special javascript library to
highlight different languages with specific colors, a good example of a js
library that does this is called [highlight.js](http://highlightjs.org/)

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
