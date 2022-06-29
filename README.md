# DOM Editing Lab

## Learning Goals

- Identify that DOM nodes are written as HTML

## Introduction

We've started looking at the DOM and how it's created. Now it's time to see its
structure.

If you haven't already, fork and clone this lab into your local environment.
Navigate into its directory in the terminal, then run `code .` to open the files
in Visual Studio Code.

## Identify That DOM Nodes Are Written As HTML

In the previous lesson, we learned that, when we load a web page in a browser,
the content we see in the DOM is a representation of the underlying HTML, CSS
and JavaScript. If we were to view the DOM in Chrome Dev Tools (we'll learn how
to do that shortly), we would see HTML that is a clone of the HTML found in the
source HTML file. As we learned earlier in the course, that HTML consists of
_elements_ that in turn consist of HTML _tags_ and their content.

When we're working in the DOM, the structure is the same. We can access objects
in the DOM (called _nodes_) that consist of tags, just like the HTML elements
that make up the base HTML. Nodes and elements are not the same thing —
all elements in the DOM are nodes but not all nodes are HTML elements. However,
when we're working in the DOM, the nodes we access and modify are virtually
always HTML elements.

### The Structure of DOM Content

We'll start by going over how content in the DOM is structured using nodes. The
information below should be familiar from what you've learned about HTML
elements.

DOM nodes most often have a starting tag and an ending tag. Examples include a
paragraph:

```html
<p>I am a paragraph.</p>
```

or a `main` section:

```html
<main></main>
```

Because they have both starting and ending tags, we can nest other nodes inside
them. The inner node is called a child node, and the outer node is called a
parent node. To nest items, we simply add the child node and its content between
its parent's starting and ending tags:

```html
<body>
  <main>
    <p>I am a nested paragraph, inside the main element, inside the body!</p>
  </main>
</body>
```

Some nodes only have a starting tag. Those are called _self-closing elements_ or
_void elements_. Void elements do not have any content nested inside of them and
cannot be parent nodes.

An example of a self-closing tag is an image:

```html
<img
  src="https://media.giphy.com/media/3o6MbkZSYy4mI3gLYc/giphy.gif"
  alt="A cartoon gif"
/>
```

In self-closing tags, the trailing `/` is optional. This is valid too:

```html
<img
  src="https://media.giphy.com/media/3o6MbkZSYy4mI3gLYc/giphy.gif"
  alt="A cartoon gif"
>
```

Enough review, let's write some HTML!

## Instructions

Start by running the tests and taking a look through the errors. You'll see that
the tests are looking for certain content to be present in the HTML file.

Next, open the `index.html` file in the browser using the instructions in the
previous lesson for your development environment.

Just to speed things up a bit, paste the following code into `index.html`:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Introduction to the DOM Lab</title>
  </head>
  <body>
    <!--All our work for this lesson will go here-->
  </body>
</html>
```

