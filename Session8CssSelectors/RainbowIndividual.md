# Rainbow Coalition: Individual Exercises
The Rainbow Coalition page looks much more exciting than a simple HTML page, but it could look even better. Follow the instructions below to update the page with even more styles.

## Part 1 - Updating The Green
Start by updating the green color so that it pops a little more.

1. Open the **style.css** file for editing
1. Find the `.green` ruleset
1. Change the `lightgreen` to `lime`
1. Run the program, and verify that the green paragraph stands out!

## Part 2 - A New Paragraph
Add another paragraph to the home page, and make it cyan. For the text of the paragraph, use this:

```
Despite this loss, the spirit of the Rainbow Coalition lives on in various civil rights movements and groups even today.
```

### HTML
Start by adding the `<p></p>` in the HTML.

1. Open the **index.html** file for editing
1. Find the last informational paragraph
1. Under that, above the `<a>`, add a new `<p></p>` element
1. For the text content, use the sentence above
1. Add a `class` attribute to the `<p>` element
1. Set the value of the `class` to `cyan`

Run the code, and verify that the new paragraph appears!

### CSS
Next, add the ruleset in the CSS to to change the color.

1. Open the **style.css** file for editing
1. Make a new line at the bottom of the file (outside of any ruleset)
1. Create a new ruleset selecting elements with class `cyan`
    - Remember, this is `.cyan { }`
1. In the ruleset (between `{` and `}`), set the `color` to `cyan`
    - Remember, this is `color: cyan;`

Run the code, and verify that the new paragraph turns a bright blue color!

## Part 3 - Bigger Back Link
Next, embiggen the "Back" link on the gallery page so it is a little easier to see.

### HTML
Start by adding an `id` attribute to the `p` that contains the "Back" link.

1. Open the **gallery.html** page for editing
1. Find the `<p>` element that surrounds the `<a>` linking back
1. Add an `id` attribute to the `<p>` element
1. Set the value of the `id` to `back-link`

This should not change the appearance yet... we need CSS for that.

### CSS
Add some CSS to style the "Back" link based on its `id` attribute value.

1. Open the **style.css** file for editing
1. Make a new line at the bottom of the file (outside of any ruleset)
1. Create a new ruleset selecting the element with id `back-link`
    - Remember, this is `#back-link { }`
1. In the ruleset (between `{` and `}`), set the `font-size` to `24px`
    - Remember, this is `font-size: 24px;`

Run the code, and verify that the "Back" link on the gallery page is larger!

## (CHALLENGE) Part 4 - More Research
Try to find some more information about Fred Hampton and the Rainbow Coalition. Search google and try to find some more text and images to fill out the webpage. Add the information/images to the files in the proper places, and try to style them appropriately.