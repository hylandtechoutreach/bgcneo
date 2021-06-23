# Restaurant Website: Individual Exercises
The website for Alfredo's Pizza Cafe (or your own restaurant) is pretty solid, but there are some changes you can make to take it to the next level. Follow the instructions below to add some new features to your website!

## Part 1 - Expanding the Existing Options
Great news! Your restaurant is expanding its offerings. There is a new location, a new specialty item, and a new topping. The website should reflect those changes.

### Adding a New Location
First, add another location to the list of locations.

1. Open the **index.html** file for editing
1. Find the `<ul></ul>` element that lists restaurant locations
1. Under the existing `<li></li>` elements, above the `</ul>`, make a new line
1. Add a new `<li></li>` element with a new location, like "Cleveland, OH"
1. Run the site and make sure the new location appears in the list!

It should look something like this:

```html
<ul>
    <li>Scranton, PA</li>
    <li>Albany, NY</li>
    <li>Utica, NY</li>
    <li>Cleveland, OH</li>
</ul>
```

### Adding a New Specialty Item
Next, add another specialty item to the list of specialty items.

1. Open the **menu.html** file for editing
1. Find the `<ul></ul>` element that lists specialty items
1. Under the existing `<li></li>` elements, above the `</ul>`, make a new line
1. Add a new `<li></li>` element with a new specialty item, like "Margherita Pizza"
1. Run the site, open the menu, and make sure the new item appears in the list!

### Adding a New Topping
Finally, add another topping to the list of toppings.

1. Open the **menu.html** file for editing
1. Find the `<ul></ul>` element that lists toppings
1. Under the existing `<li></li>` elements, above the `</ul>`, make a new line
1. Add a new `<li></li>` element with a new topping, like "Olives"
1. Run the site, open the menu, and make sure the new item appears in the list!

## Part 2 - Size Options
For several types of food (including pizza), customers may want to decide what size portion they would like. For this restaurant, let's say we want two size options: Small and Large. List these options on the Menu page!

1. Open the **menu.html** file for editing
1. Under the `</ul>` for the toppings, but _above_ the `<a>` link, make a new line
1. Add an `<h2></h2>` header that says "Size Options"
1. Under that, create a `<ul></ul>` list
1. Between the `<ul>` and `</ul>`, add an `<li></li>` element with text "Small"
1. Under that, above the `</ul>`, add another `<li></li>` saying "Large"
1. Run the site, open the menu, and make sure the size options appear!

## Part 3 - Crust Options
Many pizza restaurants have different options for crusts. This could also be applied for other types of restaurants - for example, tacos could have hard or soft shells, sushi could have white or brown rice, etc. List these options on the Menu page!

1. Open the **menu.html** file for editing
1. Under the `</ul>` for the size options, but _above_ the `<a>` link, make a new line
1. Add an `<h2></h2>` header that says "Crust Options"
1. Under that, create a `<ul></ul>` list
1. Between the `<ul>` and `</ul>`, add an `<li></li>` element with text "Thin"
1. Under that, above the `</ul>`, add another `<li></li>` saying "Deep Dish"
1. Run the site, open the menu, and make sure the crust options appear!

## (CHALLENGE) Part 4 - An "About Us" Page
Sometimes customers want to learn more about a restaurant. This can be accomplished with an "About Us" Page! Create the new page, and link it from the home page.

### The New Page
Start by creating the new page.

1. Add a new file to the Replit project
1. Name the file **about.html**
1. Open the file for editing
1. Add some basic HTML to the file
    - The `<html></html>` and `<body></body>` tags
    - A `<h1></h1>` in the `body` that says "About Us"
    - A `<p></p>` under the `h1` with a short blurb about the restaurant
1. Under the `</p>`, add an `<a>`
1. Set the `href` for the `a` to be "index.html"
1. Make the text for the `a` say "Back"

### Linking to the New Page
Now the page exists, but it is not accessible yet! Add a link to the homepage.

1. Open the **index.html** file for editing
1. Find the `<a href="menu.html">Menu</a>` above the `</body>`
1. Right under that, add a new `<a>`
1. Set the `href` for the `a` to be "about.html"
1. Make the text for the `a` say "About Us"

Run the code, and verify that it is possible to open the "About Us" page!