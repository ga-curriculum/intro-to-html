# ![Intro to HTML - Setup](./assets/hero.png)

Open your Terminal application and navigate to your `~/code/ga/lectures` directory:

```bash
cd ~/code/ga/lectures
```

Make a new directory called `html-intro`, then enter this directory:

```bash
mkdir html-intro
cd html-intro
```

Then, create an `index.html` file. These files will hold your work for this lecture:

```bash
touch index.html
```

With the files created, open the contents of the directory in VS Code:

```bash
code .
```

Open the `index.html` file and add HTML boilerplate by typing `!` and then hitting the `Tab` key. 

Open the `index.html` file in your browser.

# ![Intro to HTML - Concepts](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will have an understanding of what HTML is and what it does, its role in creating web content, and how it can benefit an application.

## What is HTML?

HyperText Markup Language or HTML is the standard markup language for documents designed to be displayed in a web browser. 

HyperText? Markup? HyperText is text displayed on a digital device with references to other text that can be navigated to using hyperlinks (commonly called links). Markup provides both structure and semantic meaning to content. For example, an `<h1>` indicates the main heading for a document, while `<p>` represents a paragraph of text.

In other words, HTML is a language for writing structured documents that link to one another.

When a web browser makes a request, it receives HTML documents from a web server and renders those documents into web pages.

HTML is one of the three main technologies used in creating web content in browsers, joined by CSS and JavaScript.

## Why use HTML?

Just like a house needs structural framing to stand, websites need structural content to style and assign behavior to. Fun and interactive sites are built on a base of HTML.

In addition to HTML providing the structure of web content, it can also play a key role in search engine optimization (SEO). Depending on how documents are structured, HTML can improve their chances of appearing in requested searches. This can lead to improved visibility and success from a marketing perspective.

# ![Intro to HTML - Comments and Elements](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand some details about comments and creating elements in HTML.

## Comments

You can add comments to an HTML document using the following syntax:

```html
<!-- This is a comment -->
```

Comments can span multiple lines. Nothing inside the `<!--` and `-->` comment tag will not be rendered.

> 🧠 VS Code can automatically comment line(s) of code for us by pressing `⌘ Command` + `/`  in macOS or `Ctrl` + `/` in Linux and Windows.

## Element syntax

We'll talk more about the HTML boilerplate you created soon; for now add everything between the `<body>` and `</body>`. Content here will show up in the browser!

HTML documents are made up of elements.

At their simplest, elements are a pair of tags with content between them.

![Element Syntax](./assets/element-syntax.png)

1. The opening tag. The tag itself starts with a `<` and ends with a `>`. Tags must also include the element name, like `h1` above. This indicates the start of an element.
2. The content of an element, `HTML Content!` here.
3. The closing tag. The tag starts with a `</` (note the addition of the slash) and ends with a `>`. The closing tag also includes the element name between. It matches the element name of the opening tag.

These things combined create an element.

Most elements have a semantic meaning, and some default styling implemented by the browser. For example, an `<h1>` element indicates the main topic of a webpage. Along with this, its text content is bold, and its default font size is larger than any other text element.

Element names are always lowercase.

There are many different types of elements. MDN maintains a [full reference here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

### Void elements

Some elements won't ever have text content. These are called void elements. Because they will not have text content, they do not have a closing tag. One such element is the `<hr>` element, which creates a horizontal rule.

```html
<hr>
```

You may see void elements written with a space and closing `/` added to the end of the tag. This is valid but not required.

```html
<hr />
```

# ![Intro to HTML - Element Attributes](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand how to apply attributes to HTML elements.

## Element attributes 

Elements have attributes that contain details about the element.

The available attributes will vary from element to element. However, many attributes work across every element, like the `id` attribute. The `id` attribute is used to uniquely identify an HTML element when necessary. It can also be used to help style elements. Here's the syntax to apply an `id` to our existing `<h1>` element.

![Element Attributes](./assets/element-attributes.png)

1. A space between the element name and the attribute name.
2. The attribute name.
3. An equal sign.
4. An attribute value wrapped in opening and closing quotes.
   
A few additional notes about attributes:

- Working with attributes will only ever alter the first tag or the only tag in the case of a void element.
- Attribute names are always written in `lower-camel-case`. In this convention, each word is written in lowercase and separated by a dash `-`.
- Multiple attributes can be used on a single element. A space should separate attributes.
- By convention, spaces aren't used to separate the equal sign from the attribute name or value, even though it would still be valid. The convention exists because spaces are the only thing separating different attributes. Adding extra spaces can make your HTML less readable.
- Double quotes are often used around the attribute value in HTML, but single quotes are also valid.

Attributes add a layer of powerful complexity to our HTML. MDN maintains a [list of attributes here](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes).

### Element and attribute indentation

At times, attribute values could be lengthy, or you may have many of them. To make your code easier to read, you should split the opening tag as in the examples below. You don't need to write this code or pay attention to these attributes. Just observe how indentation and line breaks are handled:

```html
<div
  class="my-class"
  id="my-id"
  draggable="false"
  hidden="false"
>
  My Content
</div>
```

```html
<img 
  src="https://super-bucket-extreme.s3.us-east-2.amazonaws.com/liam.jpg" 
  alt="Liam, a schnauzer, resting on a bed among his multi-color ducks."
>
```

In the course content, we will indent elements and tags in this way when an individual line of code is over 80 characters in length.

# 

![Intro to HTML - Nesting Elements](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand how to implement  nested elements, and discuss their relationships. 

## Nesting elements

Elements can also be placed inside one another, like how we placed the `<h1>` element inside the `<body>` element above. This is called nesting.

```html
<body>
  <h1 id="title">HTML Content!</h1>
</body>
```

We can continue nesting elements inside of one another.

```html
<body>
  <h1 id="title">HTML Content!</h1>
  <div>
    <h2>The big idea</h2>
    <p>HTML lets us structure content!</p>
  </div>
</body>
```

Here, we've nested a `<div>` inside the `<body>`. `<div>` is a generic container element used to group content together. Inside of the `<div>`, there is an `<h2>` and a `<p>` element. The `<p>` element represents a paragraph of text.

You ***must*** indent nested elements. Properly indenting elements makes the markup far more readable and less prone to errors.

Some elements, like the list item `<li>` element, must be nested inside another element, like the unordered list `<ul>` element. For example:

```html
<body>
  <h1 id="title">HTML Content!</h1>
  <div>
    <h2>The big idea</h2>
    <p>HTML lets us structure content!</p>
    <p>Elements can:</p>
    <ul>
      <li>Have attributes</li>
      <li>Be nested in other elements</li>
    </ul>
  </div>
</body>
```

> 🧠 Above, nested elements all have their own line, but this is not strictly required.
> Here's an example of a `<p>` element with text and a nested `<span>` element all on the same line:
> ```html
> <p>Have a <span>great</span> day!</p>
> ```

### Nested relationships

![HTML in the editor](./assets/nesting.png)

When elements are nested, they form relationships with one another.

- **Descendant / Ancestor:** An element is a descendant if it is nested anywhere within its ancestor.
- **Child / Parent:** An element is a child if it is a direct descendant of its parent.
- **Siblings:** Two or more elements are siblings if they have the same parent.

Visualizing this with a family tree-like view may help. 

![The DOM tree](./assets/tree.png)

Just like in real life, a child can also be a parent (the `<ul>` element is a child of the `<div>` element and simultaneously the parent of the `<li>` elements). Again, proper indentation of your HTML helps keep these relationships clear and organized.

This is more than an analogy - this is the ideal way to think about how dom elements are connected because it even applies to how elements are shown to users in the browser.

![HTML shown in the browser](./assets/html-in-the-browser.png)

# ![Intro to HTML - Boilerplate](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to build a basic HTML web page using HTML boilerplate.

## HTML boilerplate

HTML boilerplate is the markup that exists on every web page. In other words, it's the starting point for any work.

We've already discovered how to add this boilerplate - type a `!` in the `index.html` file and press `Tab` to create it. Below is the result of that. Note that our current HTML has a little more right now, but focus on these parts for now:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
    
</body>
</html>
```

The first line, `<!DOCTYPE html>` indicates to a browser that this will be an HTML file.

The second line, `<html lang="en">`, is the ***root*** element. Like the root of a family tree, this element is the ancestor of every other element. All other elements will be descendants of this element. `lang="en"` indicates that most of the content on this page will be written in English.

All elements inside of the `<head>` element hold information about the document (metadata) or are resources related to this document.

The first `<meta>` element informs the browser of the type of text that will appear on the page using the `charset` attribute. The second `<meta>` element will help mobile browsers display this content appropriately using the `name` and `content` attributes. Do not alter these elements.

The `<title>` element holds the text that will be shown in the tab for the page.

Anything we want to appear on the page goes into the `<body>` element. This is where we've written everything in this document so far.

## Updating the title

Update the `<title>`, change the text between the opening and closing `<title>` tags from `Document` to `Intro to HTML` as follows:

```html
<title>Intro to HTML</title>
```

# ![Intro to HTML - Block vs. Inline Elements](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to differentiate between inline and block elements.

## Inline vs. block elements

Most elements are defined as either *block* or *inline* elements.

- Block elements display on their own line and take up the full width available to them.
- Inline elements are normally displayed without line breaks and occupy only enough space to contain their contents.

### Block elements

Examples of block elements include `<div>`, `<h1>`, and `<p>` elements.

The way we write code does not have any impact on how these appear in the browser. Here, on line 1, the `<div>` and `<h1>` are coded adjacent to one another. The same for the `<h2>` and `<p>` on the next line:

```html
<div>This is a div!</div><h1>This is an h1!</h1>
<h2>This is an h2!</h2><p>This is a paragraph</p>
```

Because they are block elements, they will render on their own line, taking up the full width available to them in the browser, as seen below:

![HTML in Browser](./assets/html-in-browser-block.png)

### Inline elements

Examples of inline elements include the `<span>`, `<td>`, `<img>`, and `<button>` elements.

Notice how, on line 1, the `<span>` and `<button>` are coded adjacent to one another, just as the elements above were:

```html
<span>I'm a span!</span><button>I'm a button!</button>
```

The difference is because they are inline elements, they will share the line and do not take up the full width of the browser:

![HTML in Browser](./assets/html-in-browser-inline.png)

How we wrote the code for these doesn't matter. What matters is the built-in behavior of these different elements.

> 💡 Block elements will not share the line they occupy; inline elements will! 
> 
> Block elements can be styled to become inline elements. Conversely, inline elements can be styled to become block elements.

> 🧠 Inline elements generally cannot have their height and width set in CSS. However, using CSS like this, `display: inline-block;`, allows inline elements to be sized.
>
> Some inline elements (for example, the `<img>`) are [replaced inline elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Replaced_element) and can be given width and height without changing them into inline-block elements.
 
# ![Intro to HTML - Semantic HTML](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to identify the purpose of and use semantic elements.

## Semantic HTML

Semantic HTML helps express the meaning or purpose of the content in a webpage:

<img src="./assets/semantic.png" alt="semantic html" style="width:100vw;">

Semantic HTML clarifies the developer's intentions about what they are trying to accomplish and allows for more accurate web searches via better SEO (search engine optimization).

It also improves accessibility for the visually impaired enabling screen readers to do their job better.

## You Do

Take some time to research these semantic HTML tags. Replace the non-descriptive `<div>` element we've created already in our HTML with a more fitting element. We'll get back together and discuss

1. `<section>`
2. `<article>`
3. `<aside>`
4. `<figure>`
5. `<main>`
6. `<footer>`
7. `<header>`
8. `<nav>`

> ❓ Explain what semantic HTML is and the benefits it provides.

# ![Intro to HTML - Structural Pitfalls](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to understand some of the quirks involved in using HTML to provide a deeper understanding of formatting to help avoid common errors.


## Whitespace

Multiple spaces created using the `spacebar`, `tab` and, `return` keys are rendered as a single space character between elements and text.

```html
<p>
  You might think there would be a lot of              space here.



  Or here.



  But there's not!
</p>
```

Here is the result of the above HTML:

![The result of spacing in HTML](./assets/html-spacing.png)

When you want space between text and elements you should typically create it using CSS. As an additional option you can use the `&nbsp;` (non-breaking space) [HTML Entity](https://developer.mozilla.org/en-US/docs/Glossary/Entity) or the `<br>` or break element. 

## Malformed HTML

Proper structure and nesting of elements are important because the browser won't complain - it just won't necessarily display what you expect. One of the possible mistakes is to "overlap" tags instead of nesting them. Here's an example of malformed HTML:

```html
<p>This is <strong>important text</p></strong>
```

Errors in complex HTML can be hard to find, so it's not uncommon for Developers to use plugins or other tools to help them find errors. [Here is a tool](https://www.10bestdesign.com/dirtymarkup/) that finds errors in HTML that you provide.

> ⚠ Unlike JavaScript, our browsers will not complain if we make HTML or CSS mistakes. Instead, it just transparently does its best to correct our mistakes or fail.

# ![Intro to HTML - Level Up - Why `index.html`?](./assets/hero-why-index.png)

## Why Do We Name HTML Files `index`?

Most websites and applications have a default HTML file named `index.html`.

The practice of naming the main HTML file as `index.html` is rooted in web server standards. When a user navigates to a directory on a website, the web server searches for a default file to display. This file is most commonly `index.html`, but variations like `index.php` or `index.htm` also exist.

### Historical Context

In the early stages of the web, directories would often list files openly. To create a more user-friendly experience, web administrators began using an `index` file as a welcoming or landing page for each directory.

### Server Behavior

When a URL directs to a directory rather than a specific file, the web server will automatically look for a default file in that directory to display. `index.html` is widely recognized as that default file.

### Advantages

1. **User Experience**: Simplifies user access by allowing them to just type the domain or directory URL, without needing to remember a specific file name.
2. **Simplicity**: Makes server configuration easier, as most server software defaults to using `index.html` as the initial access point.
3. **SEO Benefits**: This standard practice is well-recognized by search engines, offering potential SEO advantages.

### Alternative Names

While `index.html` is the industry standard, some web servers allow for different default file names, configurable via server settings.

# ![Intro to HTML - Level Up - History of HTML](./assets/hero-history-of-html.png)

## History

HTML is a markup language used to create the basic structure of documents on the internet. It is the standard language for any web document displayed in your browser. HTML is used to designate the role of each element on a page and create connections to other web pages.

Sir Tim Berners-Lee developed HTML at the European Organization for Nuclear Research (CERN) in the early 1990s. Originally intended as a tool for building cross-references between academic papers, HTML quickly became the foundational tool of the modern internet thanks to its ability to structure and create links between web documents.

Today, the HTML spec is governed by the [Web Hypertext Application Technology Working Group (WHATWG)](https://whatwg.org/).

