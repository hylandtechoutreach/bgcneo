# CSS Cheatsheet
## Ruleset
A **ruleset** is how CSS applies styles to specific elements. To define a ruleset, use:
- A _selector_
- Opening curly bracket (`{`)
- A set of _declarations_
- Closing curly bracket (`}`)

#### Example
```css
p {
    color: red;
    font-size: 20px;
}
```

## Declaration
A **declaration** is a specific CSS _property_ set to a property _value_. To define a declaration, use:
- Property name
- Colon (`:`)
- Property value
- Semi-colon (`;`)

#### Example
```css
color: red;
```

## Selector
A **selector** specifies which part of the HTML to style.

### Element selector
The **element selector** selects all elements of the given type. Use the tag type that appears in the HTML.

#### Examples
```css
p {
    /* styles all paragraphs */
}

a {
    /* styles all hyperlinks */
}
```

### ID selector
The **ID selector** selects one specific HTML element based on its `id` attribute value. Use the hashtag (`#`) followed by the value of the `id` attribute for the element.

#### HTML
```html
<h1 id="header1">Header1</h1>
```

#### CSS
```css
#header1 {
    /* styles the specific h1 */
}
```

### Class selector
The **class selector** selects HTML elements based on the value of their `class` attribute. Use the dot (`.`) followed by the value of the `class` attribute.

#### HTML
```html
<h2 class="dark-mode">Title</h2>
<p class="dark-mode">Subtitle</p>
```

#### CSS
```css
.dark-mode {
    /* styles the h2 and p and any other element with "dark-mode" as a class */
}
```

## Property/Value
A **property** is an identifier that defines which feature to style. A **value** describes the specific style for the property. Refer to https://htmldog.com/references/css/properties/ to see a complete list of available properties.

### Examples
```css
body {
    background: black; /* changes the background color */
    border: 1px solid red; /* adds a solid red border with 1px width */
    box-shadow: -2px 2px 5px black; /* adds a black shadow with 5px blur, 2px to the left and 2px down */
    cursor: pointer; /* makes the cursor into a hand */
    font-family: cursive; /* sets the font to comic sans */
    font-size: 20px; /* sets the size of the text to 20px */
    height: 500px; /* sets the height to 500px */
    width: 500px; /* sets the width to 500px */
}
```