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

Between the `<title>` and `<head>`, type `link` then `[tab]`: 

```html
  ...
  <title>Document</title>
  <link rel="stylesheet" href="">
</head>
...
```

Now let's update the `href=""` 


```html
  ...
  <title>Intro to HTML & CSS</title>
  <link rel="stylesheet" href="style.css">
</head>
...
```

> The `<title>` element determines the text displayed in the browser tab for the page.
used to load the _style.css_ stylesheet, let's add it back using Emmet's help again...


## HTML5 Boilerplate
and `<title>` as follows: