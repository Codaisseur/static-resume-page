In this section, you wil learn:

* How to add a background color
* How to style a specific part of your webpage
* How to create a paragraph
* How to style your text
* How to center something on your page
* How to add an image
* How to create a link

# Styling a specific part of your page
When you look at the final result of our page, you could point out all sorts of 'boxes' that we talked about in the chapter before. When you completely zoom out, you could distinguish to boxes: a 'main box', where all info is shown, and a 'footer box', with some additional information.
The code you wrote in the chapters so far, reflects this situation:

> ```html
> <!DOCTYPE html>
>
> <html>
>  
>   <head>
>
>     <title>This will show up in hour tab!</title>
>
>     <link href="index.css" type="text/css" rel="stylesheet" />
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

You also learned how to connect your css rules to your html elements, by linking an external style sheet and writing and using a selector and a declaration. Right now, your code looks like this:

```css
  div {
    color: red;
  }
```

You could add just another style right under your first declaration, this time using a [hex color code](https://htmlcolorcodes.com/):

```css
  div {
    color: red;
    background-color: #A60000;
  }
```
> 🎓 _DIY!_
> * Change the background color of your boxes to your favorite color! Use a hex color code or rgb() notation. (Check them [here](https://htmlcolorcodes.com/).)
> * Check your work in the browser, make sure to use your DevTools!

Your result will look something like this: ![](https://cd.sseu.re/This_will_show_up_in_hour_tab__2018-09-04_14-57-31.png)

However, we only want to color our footer. We'll have to make sure css recognizes the difference between those two boxes. To do so, we need to zoom in on the elements that HTML builds on.

## HTML Tags & Attributes

In this section, you will learn some of the tags that are available in HTML to create web pages.

## Looking Closer at Tags

Most HTML elements will **open** and **close**. This means that they will have an **opening tag** and a **closing tag**.

[![](http://cd.sseu.re/20161126-xrvqv.png)](http://cd.sseu.re/20161126-xrvqv.png)

HTML element can have **attributes**, which tell us more about them.

[![](http://cd.sseu.re/20161126-not5n.png)](http://cd.sseu.re/20161126-not5n.png)

Some HTML elements are **self-closing**. They don't need a closing tag.

[![](http://cd.sseu.re/20161126-nh6e8.png)](http://cd.sseu.re/20161126-nh6e8.png)

> 🎓 _DIY adding attributes_
> * Add an attribute to each of your `<div>`-opening tags. The names of both attributes should be 'class'. The value of the first should be 'main'. The value of the second should be 'footer'. Your code should now look like this:
> ```html
> <!DOCTYPE html>
>
> <html>
>
> <!-- Other Code -->
>
>   <body>
>
>     <div class="main">I am a box!</div>
>     <div class="footer">I am another box!</div>
>
>   </body>
>
> </html>
> ```
>
> Now select each box separately in our css file: 
>
> ```css
> .footer {
>   color: white;
>   background-color: #A60000;
> }
>```



