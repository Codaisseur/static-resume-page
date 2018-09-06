## How to include CSS in your site

By now you might be wondering where to write those CSS rules for any of the web pages that built today. There are two different ways in which you cad do it. Let's take a look at both.

### Placing the CSS into your HTML file

You can include CSS rules within your HTML pages right away. You should place a `<style>` element inside the `<head>` element of the page, like the following example:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Beginner Bootcamp</title>

    <style>
      body {
        font-family: Arial;
      }
      h1, h3 {
        font-family: "Comic Sans MS";
      }
      h1 {
        color: #D32F2F;
      }
      h3 {
        color: #00AA86;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Agenda</h1>
    </header>

    <main>
      <h3>On the menu today</h3>

      <ul>
        <li>Structure with HTML</li>
        <li>Styling with CSS</li>
      </ul>
    </main>

    <footer>
      <p>Made with ❤︎ at Beginner Bootcamp</p>
    </footer>
  </body>
</html>
```

The page would look like this after adding the styles above:

[![](http://cd.sseu.re/20161122-tah7d.png)](http://cd.sseu.re/20161122-tah7d.png)

#### 💡 Don't worry about the CSS itself, you'll learn how to write it yourself in the next chapters.

### Using an external CSS file

The option above is useful when you only want to add a couple of styles to your site. But normally you will be adding more than that. In that case, you want to use an external CSS file.

You will be using the `<link>` element, which lives inside the `<head>` element of your HTML file, to tell the browser where to find the CSS file that you want to use to style that page. Notice that it doesn't have a closing tag. This element should have 3 different attributes:

* `href` specifies the "path" to the CSS file. You will place your styles in a new folder called `css`, the same way you already did for `images`.

* `type` specifies the type of document, in this case `text/css`.

* `rel` specifies the relationship between your HTML page and the file that is linking to. In this case, `stylesheet`.

If we take the example used before, this would be the HTML file:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Beginner Bootcamp</title>
    <link href="css/styles.css" type="text/css" rel="stylesheet" />
  </head>
  <body>

    <!-- rest of the content -->

  </body>
</html>
```

And you will be creating a new file `css/styles.css` with the following content:

```css
body {
  font-family: Arial;
}
h1, h3 {
  font-family: "Comic Sans MS";
}
h1 {
  color: #D32F2F;
}
h3 {
  color: #00AA86;
}
```

Keep in mind that you can have different CSS files for one single HTML page. To do this, you should include a `<link>` element for every CSS file you use. You could for example use a file to write all the rules related to your fonts and another one for your colors.

## ✏️ Exercise
> * Add a new file to your project: `index.css`.
> * In your css file add the following code:
> ```
> body {
>  background-color: green;
> }
>```
> * Check your browser. Why didn't anything change yet?
> * **Spoiler alert!** - You still have to connect your css and your html files! In your HTML file, add the following code at the bottom of your `<head>`-section:
> ```
> <link href="index.css" type="text/css" rel="stylesheet" />
>```
> * Check your browser again. Right click on the page and click inspect to open your Dev Tools. Click at the end of the word 'green' and change the value to your favorite color. What happens?
> ![css in dev tools](https://cd.sseu.re/This_will_show_up_in_hour_tab_2018-09-06_09-34-49.png)
> * Refresh the page. What happens?
> * Change the value of `background-color` in your CSS file to your favorite color. **Save and refresh your browser!**

## 💡 Tips & Tricks

> ### Nothing Happening?
>
> * Check what your code should look like at this stage [here](). 
> * Still not sure? Make sure to ask!


---
## 🎯 Learning Goal Tracker
* [x] How to set up a basic HTML structure, useful for any website.
* [x] How to change the title in your tab
* [x] How to connect your CSS to your HTML file.
---
