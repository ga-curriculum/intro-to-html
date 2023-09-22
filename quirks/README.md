# Intro to HTML - Quirks

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk


## Whitespace

Multiple spaces created using the `spacebar`, `tab` and `return` keys are rendered as a single space character between elements and text "words".

You can create extra space using CSS or by using the `&nbsp;` (non-breaking space) [HTML Entity](https://developer.mozilla.org/en-US/docs/Glossary/Entity).


## Malformed HTML

Proper structure and nesting of elements are important because the browser won’t complain - it just won’t necessarily display what you expect it to. One of the possible mistakes is to “overlap” tags instead of nesting them. Here’s an example of malformed HTML:

```html
<p>This is <strong>important text</p></strong>
```

Errors in complex HTML can be hard to find, so it’s not uncommon for Developers to use plugins or other tools to help them find errors, no matter what the language. [**Here is a website**](http://www.dirtymarkup.com/) that finds errors in HTML that you paste in.

[DirtyMarkup Formatter - HTML, CSS, & JavaScript Beautifier](https://www.10bestdesign.com/dirtymarkup/)