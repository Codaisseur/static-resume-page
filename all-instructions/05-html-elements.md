# HTML Elements

### 💡 Not going through this chapter step by step? Find the starter code  for this section [here]().

Remember?

### 🌟 HTML tags are `keywords` (tag names) surrounded by `angle brackets`. Most HTML tags open and close.

[![](http://cd.sseu.re/20170208-4ri4d.png)](http://cd.sseu.re/20170208-4ri4d.png)

Tags show you the function of certain content on a page. Let's have a closer look at some tags used for text!

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

## ✏️ Exercise

> * Go to the [example page](https://serene-mcnulty-aa84b3.netlify.com/) and inspect the text _Find me online!_ in the footer:
> ![inspect the footer](https://cd.sseu.re/Jane_Doe_2018-09-06_10-23-11.png)
> * Which tag names do you recognize?
> * Inside the body section of your `index.html`. Add the following code:
>  ```html
> <!DOCTYPE html>
>
> <html>
>  <!--some more code...-->
>   <body>
>
>     <h3>Find me online!</h3>
>
>   </body>
>
> </html>
> ```
> * Check your page in your browser. Does it show up?
> * Under your h3 element, add a paragraph element where you say something nice to your future employer.
> * When you inspect the footer section more closely, you'll see three span elements:
> ![spans](https://cd.sseu.re/Monosnap_2018-09-06_10-32-09.png)
> * Add three `<span>` elements to your page, in between your `<h3>` and `<p>` elements. In each `<span>`element, add the name of one of your favorite online presence. Your code should look like this:
>  ```html
> <!DOCTYPE html>
>
> <html>
>  <!--some more code...-->
>   <body>
>
>     <h3>Find me online!</h3>
>     <span>Medium</span>
>     <span>GitHub</span>
>     <span>LinkedIn</span>
>     <p>Have any questions? Get in touch!</p>
>   </body>
>
> </html>
> ```
> * What do you notice?

## Inline vs block elements
Congrats! You have discovered the difference between block and inline elements. By default, block-level elements begin on new lines, but inline elements can start anywhere in a line.

## 😱 Sanity Check
Your page should now look like this:
![page html-elements](https://cd.sseu.re/Jane_Doe_2018-09-06_10-46-59.png)

## 💡 Tips & Tricks

> **NOTE** This is an introduction to a couple of common HTML tags. You do not have to remember them all — the most important thing is that you know how HTML elements work and how to use different attributes.

Here is a list of resources that will help you learn more about HTML tags:

+ [Htmldog](http://htmldog.com/guides/html/beginner/tags/)
+ [MDN](https://developer.mozilla.org/nl/docs/Web/HTML/HTML_Tags)

---
## 🎯 Learning Goal Tracker

* [x] How to add different sorts of text elements to your page.
* [x] The difference between a block and an inline element.
* [ ] How to add a link to another page.
* [ ] How to add an image element to your page.
* [ ] How to style a specific element.
---
