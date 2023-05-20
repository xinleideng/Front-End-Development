# HTML
## What is HTML?
HTML stands for Hypertext Markup Language. Hypertext is text which contains links to other text. Markup refers to tags and elements used within a document. HTML is simply a text file with a specific structure that consists of elements and tags. Also take note that HTML files usually have a dot HTML suffix. For instance, when you visit a website, the first page that is returned to the browser is often called index.html. 

The rules and structure for elements and tags are known as the HTML specification. The HTML specification is maintained by the World Wide Web Consortium, or W3C, as it is commonly known. Whenever the HTML specification changes, a new version of HTML is standardized, the current version is HTML 5. 

HTML elements with their opening and closing tags, and angle brackets build up an HTML document. These elements form the structure of a web page and describe to the web browser what to display.

## HTML declaration
Now you know that HTML documents are made up of elements and tags. But before adding elements or tags, we first need to create a standard HTML structure which starts with the DOCTYPE declaration. This notifies the web browser that is a HTML documents. 

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Little Lemon</title>
    </head>
    <body>
        <h1>Our Menu</h1>
        <h2>Falafel</h2>
        <p>Chickpea, herbs, and spices</p>
        <h2>Pasta Salad</h2>
        <p>Lettuce, vegetables, and mozzarella</p>
    </body>

</html>
```
<!DOCTYPE html>
<html>
    <head>
        <title>Little Lemon</title>
    </head>
    <body>
        <h1>Our Menu</h1>
        <h2>Falafel</h2>
        <p>Chickpea, herbs, and spices</p>
        <h2>Pasta Salad</h2>
        <p>Lettuce, vegetables, and mozzarella</p>
    </body>

</html>


## Simple HTML tags
- Headings
```html
<body>
  <h1>Heading 1</h1>
  <h2>Heading 2</h2>
  <h3>Heading 3</h3>
  <h4>Heading 4</h4>
  <h5>Heading 5</h5>
  <h6>Heading 6</h6>
</body>
```
- Paragraphs

```html
<p>
   This paragraph
   contains a lot of lines
   but they are ignored.
</p>
```
Note that putting content on a new line is ignored by the web browser.

- Line Breaks

As you've learned, line breaks in the paragraph tag line are ignored by HTML. Instead, they must be specified using the &lt;br&gt; tag. The &lt;br&gt; tag does not need a closing tag.

```html
<p>
   This paragraph<br>
   contains a lot of lines<br>
   and they are displayed.
</p>
```

- Strong

Strong tags can be used to indicate that a range of text has importance.
```html
<p>
   No matter how much the dog barks: <strong>don't feed him chocolate</strong>.
</p>
```

- Bold

Bold tags can be used to draw the reader's attention to a range of text.

```html
<p>
   The primary colors are <b>red</b>, <b>yellow</b> and <b>blue</b>.
</p>
```
Bold tags should be used to draw attention but not to indicate that something is more important. Consider the following example:

```html
The three core technologies of the Internet are <b>HTML</b>, <b>CSS</b> and <b>Javascript</b>.
The following displays in the web browser: 
```

- Emphasis

Emphasis tags can be used to add emphasis to text.

```html
<p>
   Wake up <em>now</em>!
</p>
```

- Italics

Italics tags can be used to offset a range of text.

```html
<p>
   The term <i>HTML</i> stands for HyperText Markup Language.
</p>
```

**Emphasis vs. Italics**

By default both tags will have the same visual effect in the web browser. The only difference is the meaning.

Emphasis tags stress the text contained in them. Let's explore the following example:

```html
I <em>really</em> want ice cream.
```

Italics represent off-set text and should be used for technical terms, titles, a thought or a phrase from another language, for example:

```html
My favourite book is <i>Dracula</i>.
```

Screen readers will not announce any difference if an italics tag is used.

- Lists

You can add lists to your web pages. There are two types of lists in HTML.

Lists can be unordered using the &lt;ul&gt; tag. List items are specified using the &lt;li&gt; tag, for example:

```html
<ul>
   <li>Tea</li>
   <li>Sugar</li>
   <li>Milk</li>
</ul>
```

Lists can also be ordered using the &lt;ol&gt; tag. Again, list items are specified using the &lt;li&gt; tag.

```html
<ol>
   <li>Rocky</li>
   <li>Rocky II</li>
   <li>Rocky III</li>
</ol>
```

- Div tags

A &lt;div&gt; tag defines a content division in a HTML document. It acts as a generic container and has no effect on the content unless it is styled by CSS.

The following example shows a &lt;div&gt; element that contains a paragraph element:

```html
<div>
   <p>This is a paragraph inside a div</p>
</div>
```

It can be nested inside other elements, for example:

```html
<div>
   <div>
      <p>This is a paragraph inside a div that’s inside another div</p>
   </div>
</div>
```

Div inside a dive displayed in browser 
As mentioned, the div has no impact on content unless it is styled by CSS. Let’s add a small CSS rule that styles all divs on the page.

```html
<style>
   div {
      border: 1px solid black;
      padding: 2px;
   }
</style>
<div>
   <div>
      <p>This is a paragraph inside stylized divs</p>
   </div>
```

- Comments

If you want to leave a comment in the code for other developers, it can be added as:
```html
<!-- This is a comment --> 
```
The comment will not be displayed in the web browser.
