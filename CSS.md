# CSS
## What is CSS?
CSS stands for Cascading Style Sheets. It is a stylesheet language used for describing the presentation and formatting of a document written in HTML (Hypertext Markup Language) or XML (eXtensible Markup Language). CSS allows web designers to control the appearance of web pages, including layout, colors, fonts, and other visual aspects.

By using CSS, you can define styles for different elements of a web page, such as headings, paragraphs, links, tables, and more. It provides a way to separate the content of a webpage from its presentation, allowing for greater flexibility and ease of maintenance.

CSS works by selecting HTML elements and applying specific styles to them. This is done through CSS rules, which consist of a selector and a declaration block. The selector targets the HTML elements to which the styles should be applied, and the declaration block contains one or more style declarations enclosed in curly braces. Each declaration consists of a property and a value, defining the specific aspect of the element's appearance.

## CSS rule
Here is the CSS rule including a selector and a declaration block. (illutrated as follows)
![CSS rule](fig/CSS%20rule.png)
![CSS rule](fig/CSS%20property%20and%20value.png)

CSS is linked to HTML by the link tag in the head tag:
![CSS link](fig/CSS%20link.png)

The styling is applyed to all tags if only use tags like h1. But what are CSS precedents and specificity? Basically the browser will use the most precise selector for an html element. CSS has a set of hierarchy rules which dictate which rule will apply to an element. In this example, the ID rule takes precedence over the html type selector rule. 
![CSS figure 1](fig/CSS%20f1.png)
