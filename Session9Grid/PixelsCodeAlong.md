# Pixels: Code-Along Activity
Create a CSS grid containing some pixel art.

![](https://i.imgur.com/k7Ahc1C.png)

## Pixel Art Examples
#### Original Mario
![](https://i.imgur.com/L1VJN5C.png)

All art for video games was once hand-coded, pixel-by-pixel!

#### Panda
(animated: https://i.imgur.com/ghillV4.gif)

![](https://i.imgur.com/ghillV4.gif)

Now, some developers copy this style for their own art

#### Landscape  
![](https://i.imgur.com/6YJEPEp.png)

Pixel art can be used for almost anything!

## Starting Point
Get started by forking the existing Repl.

1. Go to the [existing Replit project](https://replit.com/@HylandOutreach/GridStarter)
1. Fork the project by clicking the fork button
  - Make sure to log into your account!
1. Take a look at the code so far

There should be nothing on the page - not yet anyway.

## Main Div
First, add the main `<div>` element. This will contain all the cells for the pixels.

### HTML
Start by creating the `div` in the HTML.

1. Open the **index.html** file for editing
1. Make a new line between the `<body>` and `</body>`
1. There, add a new `<div></div>` element
1. Give the `div` an `id` of `main`

The HTML should look something like this:

```html
<div id="main">

</div>
```

It won't look like anything yet - it needs some CSS!

### CSS
Next, add some CSS to the `div`.

1. Open the **style.css** file for editing
1. Create a new ruleset for the main div
    - Remember, this is `#main { }`
1. Within the ruleset, set the `width` to `400px`
1. Under that, still within the ruleset, add a border
    - It should be `2px` thick
    - It should be `solid`
    - It should be `black`

The CSS should look something like this:

```css
#main {
    width: 400px;
    border: 2px solid black;
}
```

Run the code, and verify that something appears! It should be the right width, but it still has no content...

## First Cell
It's time to add a cell to the container!

### HTML
Start by creating another `div` in the HTML.

1. Open the **index.html** file for editing
1. Make a new line between the `<div id="main">` and `</div>`
1. There, add a new `<div></div>` element
1. Give the `div` a `class` of `cell`

The HTML should look something like this:

```html
<div id="main">
    <div class="cell"></div>
</div>
```

It won't look like anything yet - it needs some CSS!

### CSS
Next, add some CSS to the cell `div`.

1. Open the **style.css** file for editing
1. Create a new ruleset for elements with class `cell`
    - Remember, this is `.cell { }`
1. Within the ruleset, set the `height` to `100px`

The CSS should look something like this:

```css
.cell {
    height: 100px;
}
```

Run the code, and verify that the whole container changes height! That's because it contains a cell.

## First Row
Now there is one cell, but the grid needs _four_ cells for each row. Start by putting together the first row.

### HTML
First, add some more `div` elements to the HTML.

1. Open the **index.html** file for editing
1. Make a new line under the existing cell `div`
    - This should still be within `<div id="main"></div>`
1. There, add a new `<div class="cell"></div>` element
1. Add two more cell `div` elements, all children of the main div

The HTML should look something like this:

```html
<div id="main">
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
    <div class="cell"></div>
</div>
```

The website should not look different yet.

### CSS
Now that the cells exist, they need to take up the proper amount of space.

1. Open the **style.css** file for editing
1. Find the `#main` ruleset
1. Within the ruleset, set the `display` to `grid`
1. Under that, set the `grid-template-columns` property
    - There should be _four_ equal columns
    - This can be accomplished with `1fr 1fr 1fr 1fr`

The CSS should look something like this:

```css
#main {
    width: 400px;
    border: 2px solid black;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
}
```

The website should not look different yet - but now the cells are in place, and they can be styled!

## Yellow
Now it's time to actually style these cells! Start by styling the two yellow cells in PAC-MAN's head.

### HTML
Start by updating the HTML - telling it which cells should be yellow.

1. Open the **index.html** file for editing
1. Find the second cell `div`
1. Add `yellow` to its `class` attribute list
    - Make a space after `cell`, within the `""`, and put `yellow`
1. Add a `class` of `yellow` to the fourth cell `div` as well

The HTML should look something like this:

```html
<div id="main">
    <div class="cell"></div>
    <div class="cell yellow"></div>
    <div class="cell"></div>
    <div class="cell yellow"></div>
</div>
```

The cells still won't be yellow yet - they need some CSS.

### CSS
Select the proper cells with CSS, and make them yellow!

1. Create a new ruleset for elements with class `yellow`
    - Remember, this is `.yellow { }`
2. Within the ruleset, set the `background` to `gold`

The CSS should look something like this:

```css
.yellow {
    background: gold;
}
```

Run the code, and verify that two yellow pixels appear in the top row!

## The Eye
To complete the top row, we need one black pixel in between the two yellow ones.

### HTML
Start by updating the HTML - telling it which cell should be black.

1. Open the **index.html** file for editing
1. Find the third cell `div`
1. Add `black` to its `class` attribute list
    - Make a space after `cell`, within the `""`, and put `black`

The HTML should look something like this:

```html
<div id="main">
    <div class="cell"></div>
    <div class="cell yellow"></div>
    <div class="cell black"></div>
    <div class="cell yellow"></div>
</div>
```

The cells still won't be black yet - they need some CSS.

### CSS
Select the proper cells with CSS, and make them black!

1. Create a new ruleset for elements with class `black`
    - Remember, this is `.black { }`
1. Within the ruleset, set the `background` to `black`

The CSS should look something like this:

```css
.black {
    background: black;
}
```

Run the code, and verify that the whole top row is what it should be! It should have a white square, a yellow square, a black square, and another yellow square.

## The Rest
Now, all the CSS is done. The only thing that's left is to add more cell `div` elements within the main `div`. The cells will continue on to the next row, so just add `<div>` elements with the proper classes. Each `div` should have a class of `cell`. Some should have a class of `yellow`, and some should have a class of `black` - each cell in the PAC-MAN corresponds to one of the cell `div` elements.

![](https://i.imgur.com/NxRAlzz.png)

For example, the next cell to add is the fifth one - it should be yellow.

```html
<div id="main">
    <div class="cell"></div>
    <div class="cell yellow"></div>
    <div class="cell black"></div>
    <div class="cell yellow"></div>

    <div class="cell yellow"></div>
</div>
```

This should add a new row. Continue adding each cell until the entire picture is complete!

## Final Code
By the end of the activity, the code should look something like this:

**index.html**
```html
<html>
    <head>
        <link href="style.css" rel="stylesheet" type="text/css">
    </head>
    <body>
        <div id="main">
            <div class="cell"></div>
            <div class="cell yellow"></div>
            <div class="cell black"></div>
            <div class="cell yellow"></div>

            <div class="cell yellow"></div>
            <div class="cell yellow"></div>
            <div class="cell yellow"></div>
            <div class="cell yellow"></div>

            <div class="cell yellow"></div>
            <div class="cell yellow"></div>
            <div class="cell"></div>
            <div class="cell"></div>

            <div class="cell"></div>
            <div class="cell yellow"></div>
            <div class="cell yellow"></div>
            <div class="cell yellow"></div>
        </div>
    </body>
</html>
```

**style.css**
```css
#main {
    width: 400px;
    border: 2px solid black;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
}

.cell {
    height: 100px;
}

.yellow {
    background: gold;
}

.black {
    background: black;
}
```