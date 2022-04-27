# HTML Elements Cheatsheet
## HTML - `html`
Surrounds the entire HTML document

```html
<html>

</html>
```

## Body - `body`
Represents the **content** of an HTML document

```html
<html>
    <body>
    
    </body>
</html>
```

## Header - `h1`-`h6`
Represents different sizes of section headings

```html
<h1>I am the biggest header</h1>
<h6>I am the smallest header</h6>
```

## Paragraph - `p`
Represents a paragraph, usually blocks of text

```html
<p>Normal text</p>
```

## Link - `a`
Creates a hyperlink to another URL that will navigate when clicked

### Attributes
- `href`: The URL where the link will navigate

```html
<a href="https://google.com">Google</a>
```

## Image - `img`
Embeds an image into a webpage

### Attributes
- `src`: The URL of the image

### Notes
- Does not require a closing tag

```html
<img src="https://i.imgur.com/v4GLRqb.jpg">
```

## Lists - `ul`, `ol`, `li`
Represents a list of items, rendered as a bulletted or numbered list

```html
<p>Shopping List</p>
<ul>
    <li>Milk</li>
    <li>Eggs</li>
    <li>Cheese</li>
</ul>

<p>Recipe</p>
<ol>
    <li>Scramble Eggs</li>
    <li>Add Milk</li>
    <li>Add Cheese</li>
    <li>Fry</li>
</ol>
```