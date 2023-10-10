# Intro to HTML - Elements

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to differentiate between inline and block elements.

## Inline vs. block elements

Most elements are defined as either *block* or *inline* elements.

- Block elements display on their own line and take up the full width available to them.
- Inline elements are normally displayed without line breaks and occupy only enough space to contain their contents.

### Block elements

Examples of block elements include `<div>`, `<h1>`, and `<p>` elements.

The way we write code does not have any impact on how these appear in the browser. Here, on line 1, the `<div>` and `<h1>` are coded adjacent to one another. The same for the `<h2>` and `<p>` on line 3:

![HTML in Editor](./assets/html-in-editor-block.png)

Because they are block elements, they will render on their own line, taking up the full width available to them in the browser, as seen below:

![HTML in Browser](./assets/html-in-browser-block.png)

### Inline elements

Examples of inline elements include the `<span>`, `<td>`, `<img>`, and `<button>` elements.

Notice how, on line 1, the `<span>` and `<button>` are coded adjacent to one another, just as the elements above were:

![HTML in Editor](./assets/html-in-editor-inline.png)

The difference is because they are inline elements, they will share the line and do not take up the full width of the browser:

![HTML in Browser](./assets/html-in-browser-inline.png)

How we wrote the code for these doesn't matter. What matters is the built-in behavior of these different elements.

> 💡 Block elements will not share the line they occupy; inline elements will! 
> 
> Block elements can be styled to become inline elements. Conversely, inline elements can be styled to become block elements.

> 🧠 Inline elements generally cannot have their height and width set in CSS. However, using CSS like this, `display: inline-block;`, allows inline elements to be sized.
>
> Some inline elements (for example, the `<img>`) are [replaced inline elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Replaced_element) and can be given width and height without changing them into inline-block elements.
