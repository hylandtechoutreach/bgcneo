# Go Bananas: Code-Along Activity
Add some styling to a website advertising bananas.

## Current Webpage
So far, there is a [simple website](https://Bananas.hylandoutreach.repl.co) that has a lot of information about a banana. All of the information is there, but the page doesn't really pop.

1. Go to the [existing Replit project](https://replit.com/@HylandOutreach/Bananas#index.html)
1. Fork the project by clicking the fork button
    - Make sure to log into your account!
1. Take a look at the code so far

There is an **index.html** file, and a **style.css** file. The CSS file is already properly linked, but there is nothing in it yet! The page could use a little CSS to make it pop.

## Adding the First Style
Bananas are often yellow, so it would make sense to make the background of the page a nice yellow-ish color. This is possible with the `background` property.

1. Open the **style.css** file for editing
1. In the CSS file, to select the entire page, use the body selector (`body`)
1. Use curly brackets (`{}`) to open the new block, also called a **ruleset**
1. Within the curly brackets, create a new **declaration** that sets the background color to yellow-ish
    - Start on a new line with the background property (`background`)
    - Insert a colon (`:`)
    - Provide the name of the yellow-ish color (`lightgoldenrodyellow`)
    - End it with a semi-colon (`;`)
1. Run the code, and verify that the background changes color!

The CSS should look something like this:

```css
body {
    background: lightgoldenrodyellow;
}
```

## Adding More `body` Styles
Any **declaration** within the `body` **ruleset** will apply by default to any element on the webpage.

1. Make the text color for the page a deep blue
	- Create a new declaration on its own line in the `body` ruleset
	- Property: `color`
	- Value: `darkblue`
1. Make the font for the page a nice sans-serif font
	- Create a new declaration on its own line in the `body` ruleset
	- Property: `font-family`
	- Value: `Tahoma`

At this point, the CSS should look like this:

```css
body {
    background: lightgoldenrodyellow;
    color: darkblue;
    font-family: Tahoma;
}
```

## Styling the Images
The images on the page are good, but they are a little too big. Use CSS to update their size.

1. In the CSS file, create a new ruleset for images
	- Start on a new line under the `body` ruleset (outside of the `{}`)
	- Create an image ruleset with `img` and opening/closing curly brackets (`{}`)
1. Within the `img` ruleset, add a declaration for height
	- Property: `height`
	- Value: `150px`

The new ruleset should look like this:

```css
img {
    height: 150px;
}
```

## Styling the Main Header
The top `h1` should have some special styling as the header for the whole page.

1. In the CSS file, create a new ruleset for `h1`
1. In the `h1` ruleset, create a declaration setting the color to goldenrod
	- Property: `color`
	- Value: `goldenrod`
1. In the `h1` ruleset, create a declaration setting the font to comic sans
	- Property: `font-family`
	- Value: `cursive`
1. In the `h1` ruleset, create a declaration setting the text size to 50 pixels
	- Property: `font-size`
	- Value: `50px`

The `h1` ruleset should look like this:

```css
h1 {
    color: goldenrod;
    font-family: cursive;
    font-size: 50px;
}
```

## Final CSS
By the end of the activity, the **style.css** file should look something like this:

```css
body {
    background: lightgoldenrodyellow;
    color: darkblue;
    font-family: Tahoma;
}

img {
    height: 150px;
}

h1 {
    color: goldenrod;
    font-family: cursive;
    font-size: 50px;
}
```