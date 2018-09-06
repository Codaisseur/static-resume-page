# Introduction to HTML
Remember? 

### 🌟 HTML is the language of the web, used for writing web pages.

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

Let's go through the code above **one tag at a time**:

* **`<!DOCTYPE html>`** tells the browser what type of information is getting (in this case HTML) to display your web page properly.

* **`<html>`** indicates that anything between it and the closing **`</html>`** tag is HTML code.

* **`<head>`** provides important information about your web page, like the title and the links to the CSS files.
  * **`<title>`** provides a title for the document, which will show on the tab of your browser.

* **`<body>`** contains everything that you will see in the browser.

In the previous example, we can see three main different elements within the body itself:

* **`<header>`** is where all the introductory content and navigation goes. It typically contains a `heading` element, a `nav` and the logo of the page.

* **`<main>`** specifies the main content of a document.

* **`<footer>`** defines a footer for your web page. It typically contains authorship and copyright information, links to your social media sites and contact information.

### 🌟 HTML tags are `keywords` (tag names) surrounded by `angle brackets`. Most HTML tags open and close.

[![](http://cd.sseu.re/20170208-4ri4d.png)](http://cd.sseu.re/20170208-4ri4d.png)

### 🌟 HTML tags can have attributes.

[![](http://cd.sseu.re/20170209-lsyri.png)](http://cd.sseu.re/20170209-lsyri.png)

### 🌟 Some HTML tags are self-closing. They don't need a closing tag.

[![](http://cd.sseu.re/20170209-c91ke.png)](http://cd.sseu.re/20170209-c91ke.png)

Now it's time for you to practice!

Now it's time for you to practice!

## ✏️ Exercise

> First you need to create a new project project in Atom (your text editor), following these steps:
>
> 1. Create a new folder somewhere in your computer called `static-portfolio-page`. **It is important that you can find this folder later ;-) .**
>
> 2. Open Atom and add a new project folder:
>
>   [![](http://cd.sseu.re/20170208-9cw7z.png)](http://cd.sseu.re/20170208-9cw7z.png)
>
> 3. A new window will open, where you can search for the `static-portfolio-page` folder in your computer. Select it and click `Open`:
>
>   [![](http://cd.sseu.re/20170208-3o9j6.png)](http://cd.sseu.re/20170208-3o9j6.png)
>
> 4. You should see a sidebar appearing on the left of your editor. Create a new file inside of this folder called `index.html` (you will be writing your first HTML in there):
>
>   [![](http://cd.sseu.re/20170208-vy91b.png)](http://cd.sseu.re/20170208-vy91b.png)
>
>   [![](http://cd.sseu.re/20170208-2ohp4.png)](http://cd.sseu.re/20170208-2ohp4.png)
>
>   [![](http://cd.sseu.re/20170208-pn3c0.png)](http://cd.sseu.re/20170208-pn3c0.png)
>
* In your index.html, copy the following code:
> ```html
> <!DOCTYPE html>
>
> <html>
>  
>   <head>
>
>     <title>This will show up in hour tab!</title>
>
>       <link rel="icon" type="image/png" href="https://cdn4.iconfinder.com/data/icons/business-1-3/512/checklist-512.png">
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
> * Open `index.html` in your browser. Check out the tab title! ![tab title](https://cd.sseu.re/This_will_show_up_in_hour_tab_2018-09-06_09-05-32.png)
> * Change the title from _'This will show up in your tab!'_ into your name. Make sure to **_save your changes_** and **_refresh the page in your browser_**! You should do this after each change you make!
> * Right click anywhere on your page and click inspect. Can you find your new title in the HTML part of your DevTools?
>
> Congrats! You created your first webpage!

## 💡 Tips & Tricks

> ### How to open an HTML file in Chrome
>
> You can open any HTML file in Chrome under the menu `File > Open File`:
>
> [![](http://cd.sseu.re/20170208-5g4jj.png)](http://cd.sseu.re/20170208-5g4jj.png)
>

---
## 🎯 Learning Goal Tracker
* [x] How to set up a basic HTML structure, useful for any website.
* [x] What elements and tags and attribtues are.
* [x] How to change the title in your tab
* [ ] How to connect your CSS to your HTML file.

---
