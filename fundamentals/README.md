# Intro to HTML - Fundamentals

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

## Element Syntax

The basic syntax of HTML elements includes opening (`<div>`) and closing (`</div>`) tags, attributes (`id="my-id" class="my-class"`), and content (`This is a div!`).

Here is how that would look as HTML in your editor:

```html
<div id="my-id" class="my-class">This is a div!</div>
```

You will be learning plenty more about Elements in the next module! You can follow this link to [Elements](../elements/README.md).

## HTML Documents

HTML Documents consist of **elements** that define the structure and content of a web page.

|HTML in Editor|HTML in Browser|
|:-:|:-:|
|![HTML in Editor](./assets/originals/html-in-editor-page.png?h=750&w=1260)|![HTML in Browser](./assets/originals/html-in-browser-page.png?h=750&w=1260)|

The HTML spec does not specify how elements and their content should be displayed; instead, it’s left up to the specific browsers how to display a certain type of element. For example, some browsers may display an `<h1>` element with a differently sized font or varying amounts of padding.

## Comments

You can add comments to an HTML document using the following syntax:

```html
<!-- This is a comment -->
```

Comments can span multiple lines, and elements in a comment tag will not be rendered.


> 🧠 Note: VS Code can automatically comment line(s) of code for us by pressing **`Command ⌘ + /`**  in macOS or **`Ctrl + /`** in Linux and Windows.