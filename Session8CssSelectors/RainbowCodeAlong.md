# Rainbow Coalition: Code-Along Activity
Add some styling to a website with information about the First Rainbow Coalition.

## Current Webpage
So far, there is a [website](https://rainbowcoalition.hylandoutreach.repl.co/) about the Rainbow Coalition with a couple of pages. The information is good, but the site could definitely use some styling.

1. Go to the [existing Replit project](https://replit.com/@HylandOutreach/RainbowCoalition)
1. Fork the project by clicking the fork button
  - Make sure to log into your account!
1. Take a look at the code so far

There is an **index.html** file, a **gallery.html**, and a **style.css** file. The CSS file is already properly linked to both the home page and the gallery page.

## Basic Changes
Start by making some basic changes that will apply to the entire website.

### Body Changes
Set the whole page to dark mode (white text on black background) using the `body` selector.

1. Open the **style.css** file for editing
1. At the top of the file, create a new ruleset for the `body`
    - `body { }`
1. Within the `body` ruleset, set the `background` to `black`
    - `background: black;`
1. Under that, set the `color` to `white`
    - `color: white;`
1. Run the code, and verify that the page is now in dark mode!

The code should look something like this:

```css
body {
    background: black;
    color: white;
}
```

### Image Changes
Resize all of the images using the `img` selector.

1. Outside of the `body` ruleset (under `}`), make a new line
1. Add a ruleset for `img`
1. In the `img` ruleset, set `height` to `200px`
1. Run the code, go to the gallery, and verify that each image is smaller

The code should look something like this:

```css
img {
    height: 200px;
}
```

### Link Changes
Currently, the hyperlinks on the page are difficult to see. Change the color of all hyperlinks using the `a` selector.

1. Outside of that ruleset (under `}`), make a new line
1. Add a ruleset for `a`
1. In the `a` ruleset, set `color` to `lightblue`
1. Run the code, and verify that each link is light blue.

The code should look something like this:

```css
a {
    color: lightblue;
}
```

## Changing the Main Header Color
Next, it's time to change the main header color. This should not apply to all headers, so it will be necessary to use a **class**! Update the HTML to add a `class` attribute to the `h1`, and then update the CSS to style it.

### Updating the HTML
First, make the changes in the HTML.

1. Open the **index.html** file for editing
1. Find the top `<h1>` element
1. Make a space after the `h1` (before `>`) and add the `class` attribute
    - `class`
    - `=`
    - `""`
1. Between the quotes, put `red`

The header should look like this:

```html
<h1 class="red">The Rainbow Coalition</h1>
```

Nothing will happen yet, though!

### Updating the CSS
Now that the HTML has been modified, it will be possible to _select_ the specific header using the `class` attribute value.

1. Open the **style.css** file for editing
1. Under the existing rulesets, make a new line
1. Create a new ruleset selecting all elements with a `class` of `red`
    - `.red { }`
1. In the `.red` ruleset, set the `color` to `salmon`
    - `color: salmon;`
1. Run the code, and verify that only the main header changes to light red!

The new ruleset should look something like this:

```css
.red {
    color: salmon;
}
```

## Rainbow Paragraphs
The goal is to have each paragraph on the page be a different color of the rainbow. These updates will be very similar to updating the header - just with different elements and colors!

### The First Paragraph
For the first paragraph, we can reuse the existing `.red` style.

1. Open the **index.html** file for editing
1. Find the first `<p>` element on the page
1. Add a `class` attribute to the `<p>` with a value of `red`
1. Run the code, and verify that the top paragraph turns light red!

The paragraph should look something like this:

```html
<p class="red">The Original Rainbow Coalition, formed in Chicago in the late 1960s, was the alliance between the Chicago Black Panther Party, Puerto Rican Young Lords, and Poor White Young Patriots Organization.</p>
```

Note that no CSS changes are required - it applies the same `.red` style to any HTML element with `class="red"`!

### The Second Paragraph
For the second paragraph, it will be necessary to create some new CSS. The goal is to make this paragraph orange.

1. Open the **index.html** file for editing
1. Find the second `<p>` element
1. Add a `class` attribute to the `<p>` with a value of `orange`
1. Open the **style.css** file for editing
1. At the bottom, create a new ruleset to select by `class="orange"`
1. In the `.orange` ruleset, set the `color` to `orange`
1. Run the code, and verify that the second paragraph turns orange!

The paragraph should look like this:

```html
<p class="orange">It was one of the moments in the history of this country where the working class came together across racial lines to build power, support each other, and fight for their shared interests.</p>
```

The ruleset should look like this:

```css
.orange {
    color: orange;
}
```

### The Third and Fourth Paragraphs
The third and fourth paragraphs should be updated in a very similar way. The third paragraph should be yellow, and the fourth paragraph should be green (using `lightgreen` as the actual color). Follow the same steps:

1. Find the proper `<p>` element in the **index.html** file
1. Set the `class` attribute to the color name
1. Make a new ruleset for the color in the **style.css** file
1. Set the `color` property to the proper color

The HTML code should look like this:

```html
<p class="yellow">The Original Rainbow Coalition represented a real threat to the established powers both locally in Chicago and nationally.</p>
<p class="green">The Chicago police conspired with the FBI to assassinate Fred Hampton, one of the key figures from the Black Panther Party, in his bed and to seriously undermine the Rainbow Coalition effort.</p>
```

The CSS should look like this:

```css
.yellow {
    color: yellow;
}

.green {
    color: lightgreen;
}
```

By this point, the paragraphs should form a nice rainbow of color!

## Reusing the Yellow Class
One of the good things about creating class styles is that they can be reused. Reuse the `.yellow` ruleset to style the header on the gallery page.

1. Open the **gallery.html** file for editing
1. Find the `<h1>` element on the page
1. Add a `class` attribute to the `<h1>` with a value of `yellow`
1. Run the code, and verify that the header turns yellow!

The header should look something like this:

```html
<h1 class="yellow">Gallery</h1>
```

## Italic Source
The next thing to do is italicize the source `<p>` element. Since there is only one of these, we can use an `id` attribute/selector.

### Updating the HTML
First, make the changes in the HTML.

1. Open the **index.html** file for editing
1. Find the `<p>` element at the bottom with the source information
1. Make a space after the `p` (before `>`) and add the `id` attribute
    - `id`
    - `=`
    - `""`
1. Between the quotes, put `footnote`

The header should look like this:

```html
<p id="footnote">Source: Kairos Center</p>
```

Nothing will happen yet, though!

### Updating the CSS
Now that the HTML has been modified, it will be possible to _select_ the specific paragraph using the `id` attribute value.

1. Open the **style.css** file for editing
1. Under the existing rulesets, make a new line
1. Create a new ruleset selecting all elements with a `id` of `footnote`
    - `#footnote { }`
1. In the `#footnote` ruleset, set the `font-style` to `italic`
    - `font-style: italic;`
1. Run the code, and verify that only the source paragraph becomes italic!

The new ruleset should look something like this:

```css
#footnote {
    font-style: italic;
}
```

## Highlighted Image
Next, it's time to add a border to one of the images (but only the main one). This will be similar to the process of selecting the one `<p>` by its `id`, but it will be with an `img` instead, and the style property will be different.

### Updating the HTML
First, make the changes in the HTML.

1. Open the **gallery.html** file for editing
1. Find the third `<img>` element
1. Make a space after the `img` (before `src=""`) and add the `id` attribute
    - `id`
    - `=`
    - `""`
1. Between the quotes, put `main-img`

The image should look like this:

```html
<img id="main-img" src="https://assets.teenvogue.com/photos/5d3719fac85d530008fb5322/16:9/w_2560%2Cc_limit/00-story-fred-hampton.jpg">
```

Nothing will happen yet, though!

### Updating the CSS
Now that the HTML has been modified, it will be possible to _select_ the specific image using the `id` attribute value.

1. Open the **style.css** file for editing
1. Under the existing rulesets, make a new line
1. Create a new ruleset selecting all elements with a `id` of `main-img`
    - `#main-img { }`
1. In the `#main-img` ruleset, set the `border` to `2px solid yellow`
    - `border: 2px solid yellow;`
1. Run the code, and verify that only the main image has a yellow border!

The new ruleset should look something like this:

```css
#main-img {
    border: 2px solid yellow;
}
```

## Final Code
The website looks much more interesting now! The files at the end should look something like this:

**index.html**
```html
<html>
  <head>
    <link href="style.css" type="text/css" rel="stylesheet">
  </head>
  <body>
    <h1 class="red">The Rainbow Coalition</h1>

    <p class="red">The Original Rainbow Coalition, formed in Chicago in the late 1960s, was the alliance between the Chicago Black Panther Party, Puerto Rican Young Lords, and Poor White Young Patriots Organization.</p>
    <p class="orange">It was one of the moments in the history of this country where the working class came together across racial lines to build power, support each other, and fight for their shared interests.</p>
    <p class="yellow">The Original Rainbow Coalition represented a real threat to the established powers both locally in Chicago and nationally.</p>
    <p class="green">The Chicago police conspired with the FBI to assassinate Fred Hampton, one of the key figures from the Black Panther Party, in his bed and to seriously undermine the Rainbow Coalition effort.</p>

    <a href="gallery.html">Gallery</a>

    <p id="footnote">Source: Kairos Center</p>
  </body>
</html>
```

**gallery.html**
```html
<html>
  <head>
    <link href="style.css" type="text/css" rel="stylesheet">
  </head>
  <body>
    <h1 class="yellow">Gallery</h1>
    <p>
      <a href="index.html">Back</a>
    </p>

    <img src="https://southsideweekly.com/wp-content/uploads/2019/09/83192385_10212858707620808_5722822335967264768_o.jpg">
    <img src="https://kpbs.media.clients.ellingtoncms.com/img/croppedphotos/2020/01/22/FIRSTRAINBOW_Publicity_02.jpg">
    <img id="main-img" src="https://assets.teenvogue.com/photos/5d3719fac85d530008fb5322/16:9/w_2560%2Cc_limit/00-story-fred-hampton.jpg">
    <img src="https://redanthropology.files.wordpress.com/2015/07/rainbown-coalition-wttw2-2.jpg">
  </body>
</html>
```

**style.css**
```css
body {
  background: black;
  color: white;
}

img {
  height: 200px;
}

a {
  color: lightblue;
}

.red {
  color: salmon;
}

.orange {
  color: orange;
}

.yellow {
  color: yellow;
}

.green {
  color: lightgreen;
}

#footnote {
  font-style: italic;
}

#main-img {
  border: 2px solid yellow;
}
```