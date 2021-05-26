# Restaurant Website: Code-Along Activity
Congratulations, you just won $250,000 in a prestigious cooking competition! The only catch is that all of that money has to go toward starting a restaurant. You can serve any type of food you'd like, but you _also_ have to make a website for your new endeavor. Follow the instructions below!

## Setup
Make sure to log into your Repl account before proceeding!

1. Open and fork the [empty Repl project](https://replit.com/@HylandOutreach/EmptyWeb) to begin
1. In your new project, open up the **index.html** file
1. Add the `html` tags (opening and closing)
1. Add the `body` tags within the `html` tags

It should look something like this:

```html
<html>
    <body>
    </body>
</html>
```

## Adding the Basics
Add a header, image, and paragraph to the site. For this example, we will be making a Pizza restaurant - but feel free to choose a different food, and a different restaurant name.

1. Add an `h1` header that says "Alfredo's Pizza Cafe" between the `<body>` and `</body>`
1. Under the `h1`, add an `<img >` of the pizza (set the `src` attribute to "https://i.imgur.com/v4GLRqb.jpg")
    - Feel free to use a different image for a different restaurant
1. Under the `img`, add a `p` that says "WE'RE NOT FINE DINING; WE'RE JUST FINE FOOD!"
    - Note that this is the actual slogan of the actual Alfredo's Pizza Cafe
1. Open your webpage in a browser and make sure it appears as expected!

At the end of this section, your code should look like this:

```html
<html>
    <body>
        <h1>Alfredo's Pizza Cafe</h1>
        <img src="https://i.imgur.com/v4GLRqb.jpg">
        <p>WE'RE NOT FINE DINING; WE'RE JUST FINE FOOD!</p>
    </body>
</html>
```

## Adding a YouTube Video
One fun way to attract customers is to add a video to the site! This is possible using YouTube's built-in embedding feature.

1. Go to [YouTube](https://youtube.com)
1. Find a video that would make sense on your website (like [this one](https://www.youtube.com/watch?v=wusGIl3v044) for a pizza restaurant)
1. From the YouTube video, click on the "SHARE" button
1. In the pop-up, click on the "Embed" button
1. In the lower right corner, click "COPY" to copy the code
1. Go back into Replit, and paste the code into the **index.html** file, under the `<p></p>` element
1. Run the program, and verify that the video appears on the page!

It should look something like this:

```html
<html>
    <body>
        <h1>Alfredo's Pizza Cafe</h1>
        <img src="https://i.imgur.com/v4GLRqb.jpg">
        <p>WE'RE NOT FINE DINING; WE'RE JUST FINE FOOD!</p>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/wusGIl3v044" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

    </body>
</html>
```

## Adding a List of Locations
Next, it's important to list the locations for the restaurant.

1. Add an `h2` header that says "Locations" under the `</iframe>`
1. Under the `h2`, add a new `ul` (unordered list)
1. Within the `ul`, add some locations within `li` elements
    - Note that the `li` elements are _children_ of the `ul` element
    - There should be at least _three_ locations
1. Open your webpage in a browser and make sure it appears as expected!

At the end of this section, your code should look something like this:

```html
<html>
    <body>
        <h1>Alfredo's Pizza Cafe</h1>
        <img src="https://i.imgur.com/v4GLRqb.jpg">
        <p>WE'RE NOT FINE DINING; WE'RE JUST FINE FOOD!</p>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/wusGIl3v044" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        
        <h2>Locations</h2>
        <ul>
            <li>Scranton, PA</li>
            <li>Albany, NY</li>
            <li>Utica, NY</li>
        </ul>
    </body>
</html>
```

## Adding the Menu - A New Page
The website has information now, but we still need to add in a menu! The menu can be another page on the website - this way, it can stay separate from the main page. Start by adding a new file, filling out some basic HTML, and linking it from the **index.html** file.

1. In the Replit project, add a new file by clicking the "Add file" button
1. Enter the name **menu.html** for the new file
1. Open the new file, and add the basic elements: `html` and `body`
1. Within the `body`, add an `h1` header that says "Menu"
1. Under that, add a `p` that says "No substitutions please"

The code in the **menu.html** file should look something like this:

```html
<html>
    <body>
        <h1>Menu</h1>
        <p>No substitutions please</p>
    </body>
</html>
```

### Linking to the New File
In order to actually see the new page, it will be necessary to link to it from the main page!

1. Open the **index.html** file for editing
1. Under the `</ul>` element, create an `a` element
1. Set the `src` of the `a` element to be "menu.html"
1. Set the text of the `a` element to say "Menu

The `a` element should look something like this:

```html
<a href="menu.html">Menu</a>
```

Run the program, and verify that it is possible to open the new Menu page!

## Adding Specialty Pizzas
Now that the Menu page has been created, we need to add some food to it.

1. Open the **menu.html** file for editing
1. Make a new line under the `</p>` in the `body`
1. Add an `h3` that says "Top Specialty Pizzas"
1. Under the `</h3>`, create a `<ol></ol>` element
    - This is an _unordered_ list because these are ranked in order
1. Between the `<ol>` and `</ol>`, add an `<li></li>` element
1. Between the `<li>` and `</li>`, add the text "Hawaiian Pizza"
1. Continue this process and add two more `<li></li>` elements under the first one within the `ol`

The code for this part should look something like this:

```html
<h3>Top Specialty Pizzas</h3>
<ol>
    <li>Hawaiian Pizza</li>
    <li>Meat Lovers Pizza</li>
    <li>Meat Haters Pizza</li>
</ol>
```

Run the program, and verify that the specialty pizzas appear on the menu!

## Adding Toppings
Next, add a section that lists all the toppings a customer can add.

1. Under the `</ol>` in the `body`, make a new line
1. Add an `h3` that says "Toppings"
1. Under the `</h3>`, create a `<ul></ul>` element
1. Between the `<ul>` and `</ul>`, add an `<li></li>` element
1. Between the `<li>` and `</li>`, add the text "Pepperoni"
1. Continue this process and add two more `<li></li>` elements under the first one within the `ul`

The code for this part should look something like this:

```html
<h3>Toppings</h3>
<ul>
    <li>Pepperoni</li>
    <li>Mushroom</li>
    <li>Extra Cheese</li>
</ul>
```

Run the program, and verify that the toppings list appears on the menu!

## Linking Back
Currently, after a customer visits the menu, they cannot get back to the main page. We can fix this with another `a` element on the Menu page.

1. Under the final `</ul>`, make a new line
1. Add an `a` element
    - Set its `href` attribute to `index.html`
    - Set its text content to `Back`

It should look something like this:

```html
<a href="index.html">Back</a>
```

Run the program, and verify that it is possible to go to the Menu page and go back!

## Final HTML
By the end, the two files should look something like this:

**index.html**
```html
<html>
    <body>
        <h1>Alfredo's Pizza Cafe</h1>
        <img src="https://i.imgur.com/v4GLRqb.jpg">
        <p>WE'RE NOT FINE DINING; WE'RE JUST FINE FOOD!</p>

        <iframe width="560" height="315" src="https://www.youtube.com/embed/wusGIl3v044" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        
        <h2>Locations</h2>
        <ul>
            <li>Scranton, PA</li>
            <li>Albany, NY</li>
            <li>Utica, NY</li>
        </ul>
        <a href="menu.html">Menu</a>
    </body>
</html>
```

**menu.html**
```html
<html>
    <body>
        <h1>Menu</h1>
        <p>No substitutions please</p>

        <h3>Top Specialty Pizzas</h3>
        <ol>
            <li>Hawaiian Pizza</li>
            <li>Meat Lovers Pizza</li>
            <li>Meat Haters Pizza</li>
        </ol>

        <h3>Toppings</h3>
        <ul>
            <li>Pepperoni</li>
            <li>Mushroom</li>
            <li>Extra Cheese</li>
        </ul>

        <a href="index.html">Back</a>
    </body>
</html>
```