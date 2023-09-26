# Intro to HTML - Boilerplate

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to create HTML boilerplate, and connect JS and CSS modules, if needed.

## HTML5 Boilerplate

Most websites and applications have a default HTML file named **index.html**.

**Boilerplate** is the markup that would exist in every web page, i.e., the starting point.

Use the `!` emmet abbreviation in index.html to create HTML boilerplate.

Type `!` then `[tab]` - voila!

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

## Linking a CSS Module

If we are going to include CSS we'll need to use the `<link>` element to load that module.

Between the `<title>` and `</head>`, type `link` then `[tab]`: 

```html
  ...
  <title>Document</title>
  <link rel="stylesheet" href="">
</head>
...
```

Now let's update the `href=""` with the relative path of your CSS module, including its extension. (e.g. *style.css*)

```html
<head>
  ...
  <title>Document</title>
  <link rel="stylesheet" href="style.css">
</head>
...
```

## Linking a JavaScript Module

If we are going to include JavaScript we'll need to use the `<script>` element to load that module.

Between the `<title>` and `</head>`, type `script` then `[tab]`:

```html
<head>
  ...
  <title>DOM Practice</title>
  <script></script>
</head>
```

Now let's add the `src=""` attribute with the relative path of your JS module, including its extension. (e.g. *main.js*)

```html
<head>
  ...
  <title>DOM Practice</title>
  <script src="js/main.js"></script>
</head>
```

Finally, add the `defer` attribute to ensure the DOM is ready before the script executes

```html
<head>
  ...
  <title>DOM Practice</title>
  <script defer src="js/main.js"></script>
</head>
```

## Updating the Title

The `<title>` element determines the text displayed in the browser tab for the page.

Updating the `<title>` is as simple as changing the text between the opening and closing `<title>` tags, (e.g. from *Document* to *HTML Boilerplate*) as follows:

```html
<head>
  ...
  <title>HTML Boilerplate</title>
</head>
```

