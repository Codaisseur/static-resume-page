# 🎯 Learning Goals
In this section, you wil learn:

* [ ] How to add a background color
* [ ] How to style a specific part of your webpage
* [ ] How to create a paragraph
* [ ] How to style your text
* [ ] How to center something on your page
* [ ] How to add an image
* [ ] How to create a link

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

---
#### 🎯 Learning Goal Tracker
* [x] How to add a background color
---

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
> * Now select each box separately in our css file: 
>
> ```css
> .footer {
>   color: white;
>   background-color: #A60000;
> }
>```
> The result should look something like this:
> ![result](https://cd.sseu.re/This_will_show_up_in_hour_tab__2018-09-04_15-11-49.png)

---
#### 🎯 Learning Goal Tracker
* [x] How to add a background color
* [x] How to style a specific part of your webpage
---

Time to add some content to our footer! Let's check on how to add text to our HTML...

## Text

### Headings

HTML has six "levels" of headings:

```html
<h1>This is used for main headings</h1>
<h2>This is used for a level 2 heading</h2>
<h3>This is used for a level 3 heading</h3>
<h4>This is used for a level 4 heading</h4>
<h5>This is used for a level 5 heading</h5>
<h6>This is used for a level 6 heading</h6>
```

By default browsers display the contents of headings at different sizes. The content of an `<h1>` element is that largest, and the content of an `<h6>` element is the smallest.

[![](http://cd.sseu.re/20161119-90oh8.png)](http://cd.sseu.re/20161119-90oh8.png)

### Paragraphs

You can create a paragraph by surrounding the words with an opening `<p>` tag and a closing `</p>` tag.

```html
<p>Code is everywhere. People in all industries can benefit from learning code to boost their productivity and e-skills.</p>

<p>We offer you a kickstart into the world of modern day software engineering for the web with immersive and results-driven boot camps.</p>

<p>Learn to build web applications from industry experts. Choose from entry level beginner courses all the way up to advanced courses that prepare you for a new career.</p>
```

By default browsers will show each paragraph on a new line with a bit of space in between.

[![](http://cd.sseu.re/20161119-cwhpw.png)](http://cd.sseu.re/20161119-cwhpw.png)

### Span
A span is an **inline element**, meaning it can be on a line with other elements:

```html
<p>We</p>
<p>are</p>
<p>on</p>
<p>a</p>
<p>new</p>
<p>line</p>

<span>We</span>
<span>are</span>
<span>on</span>
<span>one</span>
<span>line</span>
```
Which will look like this:

![](https://cd.sseu.re/Page_Title__2018-09-04_15-28-14.png)

> 🎓 _DIY Add some text!_
> * Add a heading to your footer, saying 'Find me online!'
> * Add a couple of spans with social media names (facebook, github, medium, etc)
> * Add a paragraph inviting the reader to ask for more information.
> Your code will look something like this:
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
>     <div class="footer">      
>       <h4>Find me online!</h4>
>       <span>facebook</span>
>       <span>github</span>
>       <span>medium</span>
>       <p>Have any questions? Get in touch!</p>
>     </div>
>
>   </body>
>
> </html>
> ```
> * finally update your style sheet and add a css declaration with a property `text-align` and a value `center`. Explore with some other properties, such as [font-family](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family) and [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)
> By now, your page should look something like this:
> ![](https://cd.sseu.re/Jane_Doe__2018-09-04_15-40-26.png)

---
#### 🎯 Learning Goal Tracker
* [x] How to add a background color
* [x] How to style a specific part of your webpage
*  [x] How to create a paragraph
*  [x] How to style your text
*  [x] How to center something on your page

---

