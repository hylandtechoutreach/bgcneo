# About Me: Follow-Along
With this exercise, you will create a webpage that shows some information about yourself.

## Making a Repl Account
Before beginning, make sure you have a Repl account. You can follow [these instructions](../ReplSetup.md) to set one up if you do not have one.

## Getting Started
Start by creating a **fork** of an empty project to get started, and sharing a **Multiplayer Link** to the project.

1. Go to [this empty Project](https://replit.com/@HylandOutreach/EmptyWeb#index.html)
1. Click the "Fork" button in the upper right  
    ![](https://i.imgur.com/RR31b6X.png)
1. On the next page, click the "Share" button in the upper right  
    ![](https://i.imgur.com/FfGzMHe.png)
1. In the window that appears, click the "Copy" button next to the link  
    ![](https://i.imgur.com/LGfBIUE.png)

Once the **Multiplayer Link** has been copied, you can open [this google form](https://forms.gle/tw1bQoptj9M8Jts68). Fill in your name, paste the link, and submit the form.

## HTML Setup
Now everything should be ready to go. Start by creating a simple HTML document containing a header.

1. In the **index.html** file, add the `<html></html>` opening and closing tag
1. Inside of the `<html>` and `</html>`, add the `<body></body>` opening and closing tag
1. Inside of the `<body>` and `</body>`, add a `<h1></h1>` header tag that says "About Me"
1. Click the **Run** button to make sure your page is working!

At the end of the **Setup**, your code should look like this (try to match the spacing):
```html
<html>
    <body>
        <h1>About Me</h1>
    </body>
</html>
```

## Greeting and Basic Information
Next, add some additional information to the webpage.

1. Under the `h1` header tag, add in a `<p></p>` paragraph tag welcoming the user to your page
1. Add another paragraph containing your name
1. Add another paragraph containing your grade level
1. Add another paragraph containing your favorite thing to do

At the end of this section, your code should look something like this:
```html
<html>
    <body>
        <h1>About Me</h1>

        <p>Welcome to my page!</p>
        <p>My name is Arthur Read</p>
        <p>I am in 3rd grade</p>
        <p>I like to play with my dog</p>
    </body>
</html>
```

## Favorite Animal
Add in a picture of your favorite animal.

1. Under the last `p` paragraph tag, add a smaller `h3` header that says "Favorite Animal"
1. Add an image of your favorite animal
    1. Find an image somewhere online, and copy the **image URL**
    1. Add an `<img>` image tag under the `h3` header
    1. Set the `src` of the image to the URL, in quotes

## Final HTML
The code should look something like this:

```html
<html>
    <body>
        <h1>About Me</h1>

        <p>Welcome to my page!</p>
        <p>My name is Arthur Read</p>
        <p>I am in 3rd grade</p>
        <p>I like to play with my dog</p>

        <h3>Favorite Animal</h3>
        <img src="https://i.imgur.com/GfT5Z9R.png">
    </body>
</html>
```