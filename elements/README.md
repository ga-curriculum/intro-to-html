# Intro to HTML - Elements

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk


## Tags

Most **Tags** have an opening and closing tag name inside angle brackets like this:

```html
<p></p>
```

Note the slash in the closing tag.

Some tags such as `<img>` and `<br>` are called *empty tags* because they **never have content** and thus do not have a closing tag. Before HTML5, empty tags typically had a slash before the last angle bracket like this `<br/>`; however, since the introduction of HTML5, it is preferable to omit the slash.

```html
  <img 
    src="https://super-bucket-extreme.s3.us-east-2.amazonaws.com/liam.jpg" 
    alt="Liam, a schnauzer, resting on a bed among his multi-color ducks"
  >
```

Lowercase is used for both tags and attribute names.


## Elements

An **Element** consists of a *Tag* and its contents (if any), which may include other tags as well. For example:

```html
<p>Have a <span>great</span> day!</p>
```

Some elements, such as a table cell `<td>`, would be pointless unless nested inside a `<tr>` row element.


> ‼️ Unlike JavaScript, our browsers will not complain if we make HTML or CSS mistakes. Instead, it just transparently does its best to correct our mistakes or fail.


Most elements are defined as either *block* or *inline* elements.

- **Block** elements display on their own line and take up the full width available to them (they don’t allow other elements next to them unless they are styled to do so).
    
    Examples: `<div>`, `<h1>`, `<p>`
    
- **Inline** elements are normally displayed without line breaks and occupy only enough space to contain their contents.
    
    Examples: `<span>`, `<td>`, `<img>`
    
    <aside>
    🧠 Inline elements generally cannot have their height and width set in CSS. However, using CSS like this, display: inline-block;, allows inline elements to be sized.
    
    </aside>
    
    <aside>
    ⚠️ Some inline elements (for example, the `<img>` tag) are [replaced inline elements](https://developer.mozilla.org/en-US/docs/Web/CSS/Replaced_element) and can be given width and height without changing them into inline-block elements.
    
    </aside>

### Attributes

An element may contain **attributes** that provide additional information about that element. Attributes are placed within the opening tag and are typically *name/value* pairs separated by an equals sign (`=`).

The *value* should always be put in double-quotes (not single quotes). For example:

```html
<div class="my-class">My Content</div>
```

The most common attribute is `class` for assigning CSS class(es) to an element.

The `id` attribute is used to target a specific element (or its contents) more easily for styling or JS access. The value of an `id` attribute should be unique in the document. The `id` attribute is optional and should be used *only when necessary* - the less we clutter our code, the better.

A few attributes, such as `required`, `checked`, `novalidate`, and `disabled`, stand alone without a value called *boolean attributes*.

You can add custom attributes of your own too! The HTML5 spec recommends that you prefix them with `data-`. Developers can use custom attributes to add additional information to the markup. They are commonly used by front-end frameworks such as AngularJS.

# HTML Nesting

!https://i.imgur.com/4W1snYp.png

When an element contains another element, the contained element is considered to be *nested* inside the outer element. The HTML graphic above has colored boxes drawn around elements to help visualize the relationship between parent and child elements.

You *must* indent nested elements. Properly indenting elements makes the markup more readable and **much** less prone to errors.


> 🧠 Properly indenting all code (HTML, CSS & JS) is mandatory if you want to get a job!


Describing Nested Relationships:

- **Descendant / Ancestor**: An element is considered a *descendant* if it is nested anywhere within its *ancestor*.
- **Child / Parent**: An element is considered a *child* if it is a direct descendant of its *parent*.
- **Siblings**: Two or more elements are considered *siblings* if they have the same *parent*.