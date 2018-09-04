# Main Structure

## Learning Goals
In this section, you will learn:

* What HTML and what CSS are used for
* How to set up a basic HTML Page
* How to set up a CSS rule
* How to connect your HTML to your CSS

# Introduction
In this lesson, you will start creating static web pages with HTML and CSS, which are the basics of web development. You will be using HTML, or Hypertext Markup Language, to tell the web browser how to structure the content of your web page. And you will use CSS, or Cascading Style Sheets, to tell the browser what the content should look like.

![html, javascript,  css](https://cd.sseu.re/2._Digitale_Werkplaats_-_Introductie_in_programmeren_-_Sessie_2_DRAFT_-_Google_Slides__2018-09-03_15-38-58.png)

Another important part of web development in JavaScript, which you use to make your pages interactive. We'll talk more about JavaScript later.

> 🎓 _DIY: Getting started_
> * Create a directory which is called `html-and-css`
> * In atom, click on `add new project folder` and select the `html-and-css` directory.
> * In Atom, create two new files. One should be called `index.html`, the other `index.css`
>
> Ready? Let's start with some HTML!

# HTML Structure

Think of any kind of document, like a newspaper, an application form, or a book... In all of them, structure is very important in helping readers to understand the messages they are trying to communicate and to navigate around the document. Web pages are no different, and in order to learn how to write them, it is very important to understand their structure.

## Using HTML to structure your pages

HTML is the language of the web, used for writing web pages. Any website you ever visited was made with html. Let's look at an example:

![WebPage](http://cd.sseu.re/20161122-k2yib.png)

You can see the HTML code for this page below:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Beginner Bootcamp</title>
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
      <p>Made with ❤︎ at Codaisseur</p>
    </footer>
  </body>
</html>
```

The HTML code (in red) is what we call **HTML elements**. Most of the times, these elements are made up of two **tags**: an **opening tag** and a **closing tag** (notice that the closing tag has an extra forward slash "`/`" in it). These elements tell the browser what kind of information lives between its opening and closing tags. You can think of tags like "containers".

Let's take a closer look at the code above and explain its different parts:

* **`<!DOCTYPE html>`** tells the browser what type of information is getting (in this case HTML) to display your web page properly.

* **`<html>`** indicates that anything between it and the closing **`</html>`** tag is HTML code.

* **`<head>`** provides important information about your web page, like the title and the links to the CSS files.
  * **`<title>`** provides a title for the document, which will show on the tab of your browser.

* **`<body>`** contains everything that you will see in the browser.

In the previous example, we can see three main different elements within the body itself:

* **`<header>`** is where all the introductory content and navigation goes. It typically contains a `heading` element, a `nav` and the logo of the page.

* **`<main>`** specifies the main content of a document.

* **`<footer>`** defines a footer for your web page. It typically contains authorship and copyright information, links to your social media sites and contact information.

> 🎓 _DIY: Setting up your basic framework_
> * In your index.html, copy the following code:
> ```html
> <!DOCTYPE html>
>
> <html>
>  
>   <head>
>
>     <title>This will show up in hour tab!</title>
>
>   </head>
>
>
>   <body>
>
>   </body>
>
> </html>
> ```
> * Open `index.html` in your browser. Check out the tab title! ![tab title](https://cd.sseu.re/This_will_show_up_in_hour_tab_2018-09-03_16-23-34.png)
> * Change the title from _'This will show up in your tab!'_ into your name. Make sure to **_save your changes_** and **_refresh the page in your browser_**! You should do this after each change you make!
>
> Congrats! You created your first webpage!

## Thinking Inside the Box

Did you notice that some parts of that HTML code are indented? This indicates that some tags are "nested" or placed inside of other tags. For example, if you look at `<main>`, you can see that there is a `<h3>` and a `<ul>` elements inside.

> You can think of any HTML code as a series of boxes that live inside one another. Each box is called an **element**.

Check out the diagram below and try to identify the different parts in the HTML code:

[![](http://cd.sseu.re/20161122-t9spb.png)](http://cd.sseu.re/20161122-t9spb.png)

> 🎓 _DIY: Adding some boxes_
> * In your index.html, we'll add two boxes inside  our 'body-box'. **_Don't forget to save and reload your browser_**!
> ```html
> <!DOCTYPE html>
>
> <html>
>  
>   <head>
>
>     <title>This will show up in hour tab!</title>
>
>   </head>
>
>
>   <body>
>
>     <div>I am a box!</div>
>     <div>I am another box!</div>
>
>   </body>
>
> </html>
> ```
> * In your browser, right-click on the text 'I am a box' and choose `inspect`. This opens your **DevTools**, which are going to be super helpful any time you need to do some development:
> ![Inspect & DevTools](https://cd.sseu.re/Jane_Doe_2018-09-03_16-33-28.png)
> Hover over the text in you DevTools. What happens?
>
> Cool, but boring. Let's add some style!

# Adding CSS

It's time to add some styles to our pages!

## Thinking Inside the Box

Do you remember when HTML was introduce that we talked about how to think in boxes will help you understand the structure of your pages? Well, good news! That way of thinking will also help you when writing CSS.

Back then we looked into this example:

[![](http://cd.sseu.re/20161122-t9spb.png)](http://cd.sseu.re/20161122-t9spb.png)

CSS associates style rules with HTML elements. With CSS you can create rules to control the way each of those boxes (and its content) is displayed in the browser. 

## How to include CSS in your site

### Using an external CSS file

We will use a `<link>` element, which lives inside the `<head>` element of your HTML file, to tell the browser where to find the CSS file that you want to use to style that page. Notice that it doesn't have a closing tag. This element should have 3 different attributes:

* `href` specifies the "path" to the CSS file. You will place your styles in a new folder called `css`, the same way you already did for `images`.

* `type` specifies the type of document, in this case `text/css`.

* `rel` specifies the relationship between your HTML page and the file that is linking to. In this case, `stylesheet`.

If we take the example used before, this would be the HTML file:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Beginner Bootcamp</title>
    <link href="index.css" type="text/css" rel="stylesheet" />
  </head>
  <body>

    <!-- rest of the content -->

  </body>
</html>
```

This will look for any styles in `index.css`.

> 🎓 _DIY: Connecting the dots..._
> * Add the following code under the title element in the head section of your html file: 
> ```html
> <link href="index.css" type="text/css" rel="stylesheet" />
> ```


## CSS Selectors

CSS associates style rules with HTML elements. With CSS you can create rules to control the way each of those boxes (and its content) is displayed in the browser. Like for example:

```css
p {
  font-family: Helvetica;
}

div {
  font-family: Arial;
  color: green;
}
```

CSS rules always contain two parts: a **selector** and a **declaration**, made up of a **property** and a **value**.

[![](http://cd.sseu.re/20161126-1xmve.png)](http://cd.sseu.re/20161126-1xmve.png)

> 🎓 _DIY: Color it up!_
> * Lets give your boxes some color! Inside your `index.css`  add a css rule with a `div`-selector, the property `color` and the value `red`. Your code should look like this: 
> ```css
>   div {
>     color: red;
>   }
> ```
> What happens when you safe your changes and refresh the page?
