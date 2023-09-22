# Intro to HTML - Level Up - Emmet

![Hero image](./assets/hero.png)

## What is Emmet in VS Code?

Emmet is a plugin in Visual Studio Code (VS Code) that enhances HTML, CSS, and JavaScript development by allowing you to write abbreviations that expand into complete code snippets. It employs a unique abbreviation syntax, influenced by CSS selectors, to produce code with minimal keystrokes.

### How Emmet Works

1. **Abbreviation**: Type an Emmet abbreviation. For example, `ul>li*5` is an abbreviation to create a list with five list items.

2. **Expansion**: Press the `Tab` key or another designated trigger to expand the abbreviation into full code. Using the previous example, `ul>li*5` will expand to:
```html
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

### Key Features
 - **Code Wrapping:** You can select code and use Emmet to wrap it with new elements.
 - **Lorem Ipsum Generator:** Use lorem to insert placeholder text.
 - **Attribute Generation:** You can include attributes within your Emmet abbreviation, like a[target=_blank].

### Enabling Emmet
In most cases, Emmet is enabled by default in VS Code for HTML, CSS, and certain JavaScript files. However, you can customize Emmet behavior through VS Code settings.

### Why Use Emmet?
 - **Speed:** Generate large blocks of code with fewer keystrokes.
 - **Consistency:** Helps maintain uniformity in code structure.
 - **Efficiency:** Reduces the chances of errors in repetitive coding tasks.