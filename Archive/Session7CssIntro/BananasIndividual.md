# Go Bananas: Individual Exercises
The banana product page looks much more exciting than a simple HTML page, but it could look even better. Follow the instructions below to update the page with even more styles.

## Part 1 - Updating Existing Rulesets
Start by updating some of the existing properties.

### Changing the Text Color
The `darkblue` color is a little too strong. Change it to a lighter blue color that still maintains a contrast with the yellow background.

1. In the **style.css** file, find the `body` ruleset
1. In the `body` ruleset, find the declaration for the `color` property
1. Update the value of the `color` property from `darkblue` to `steelblue`

Run the code, and verify that the text changes color!

### Changing the Main Header Font
Update the main header font so it looks even more fun.

1. In the **style.css** file, find the `h1` ruleset
1. In the `h1` ruleset, find the declaration for the `font-family` property
1. Update the value of the `font-family` property from `cursive` to `jokerman`

Run the code, and verify that the font changes!

### Making the Images Larger
The images on the page are a little small. Make them bigger!

1. In the **style.css** file, find the `img` ruleset
1. In the `img` ruleset, find the declaration for the `height` property
1. Update the value of the `height` property from `150px` to `200px`

Run the code, and verify that the images get bigger!

## Part 2 - Creating Additional Rulesets
Next, add some _new_ rulesets to change other parts of the HTML page.

### Updating the Color of the Section Headers
The section headers should match the background more effectively. Update the CSS so that the headers are a dark gold color.

1. In the **style.css** file, create a new **ruleset** for `h2`
    - Place the new ruleset beneath the existing rulesets (under `}`)
    - Use the `h2` selector and curly brackets (`{}`) to open the new block
2. Within the curly brackets, create a new **declaration** that sets the text color
    - Property: `color`
    - Value: `darkgoldenrod`

It should look something like this:

```css
h2 {
    color: darkgoldenrod;
}
```

### Updating the Font of the Reviewer Names
The reviewer names should have a different font to differentiate them from the rest of the text on the page.

1. In the **style.css** file, create a new **ruleset** for `h3` (reviewer names are in these headers)
2. Within the ruleset, create a new **declaration** that sets the font
    - Property: `font-family`
    - Value: `cursive`

## (CHALLENGE) Part 3 - New Product
Update the HTML on the page so that it is about a different product! Change the text, images, and anything else. The same styles should apply to any new HTML!

## (CHALLENGE) Part 4 - Adding Style to Other Projects
Find some of the previous HTML projects you have created. Try to figure out how to add some CSS to make them more fun.

- Start by creating a new **style.css** file in the Replit project
- Then, link the file from the HTML
    - It should look something like `<link href="style.css" type="text/css" rel="stylesheet">`
- Finally, add some CSS styles! Feel free to copy and paste from the Banana website.