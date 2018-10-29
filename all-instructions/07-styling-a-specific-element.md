# Styling a specific element

last chapter, we ended up with page looking something like this:
![page images-and-links](https://cd.sseu.re/FireShot_Capture_2_-_Jane_Doe__-_file____Users_mimi_Code_Codaisseur_.png_2018-09-06_11-16-42.png)

Let's go and fix the styling of those images!

## CSS Selectors

CSS associates style rules with HTML elements. With CSS you can create rules to control the way each of those boxes (and its content) is displayed in the browser. Like for example:

```css
p {
  font-family: Helvetica;
}

h1, h2, h3 {
  font-family: Arial;
  color: green;
}
```

CSS rules always contain two parts: a **selector** and a **declaration**, made up of a **property** and a **value**.

[![](http://cd.sseu.re/20161126-1xmve.png)](http://cd.sseu.re/20161126-1xmve.png)

Here, we are selecting HTML Elements by their tags tags. But imagine that you have multiple paragraphs in your web page, and you want to style them different. What now? That's where **classes** come in.

Let's look at an example. First you should be adding some classes to your HTML elements:

```html
<h2 class="valley-name">Valley of Geysers</h2>
<h2 class="dinosaur-name">Abrictosaurus</h2>
```

After that, you can target those elements by using their class names like this in your `css/styles.css` file:

```css
.valley-name {
  color: #D32F2F;
}
.valley-name {
  color: #00AA86;
}
```

The color of the first `<h2>` will be red, while the second one will be green.

## Naming Your Classes

You should try to name your classes "semantically" - thinking of the role the targeted class has on the page and NOT how does it look like. Let's look at an example:

```css
/* Bad */
.red-background {
  background: red;
  height: 300px;
  text-align: center;
}

/* Good */
.main-banner {
  background: red;
  height: 300px;
  text-align: center;
}
```

If you apply this rule, it will make your css better, more flexible, maintainable and understandable.

## ✏️ Exercise
> * Check your `index.css`. What selector are we using? What is the property? What is the value?

## Images
### Size

The `width` and the `height` properties allow you to control the size of an image.

```html
<!-- index.html -->

<img src="https://goo.gl/F6SGlE" alt="Abrictosaurus" class="large" />
<img src="https://goo.gl/F6SGlE" alt="Abrictosaurus" class="medium" />
<img src="https://goo.gl/F6SGlE" alt="Abrictosaurus" class="small" />
```

```css
/* css/styles.css */

img.large {
  width: 500px;
  height: 300px;
}
img.medium {
  width: 250px;
  height: 150px;
}
img.small {
  width: 100px;
  height: 60px;
}
```

[![](http://cd.sseu.re/20161123-6de1x.png)](http://cd.sseu.re/20161123-6de1x.png)

### Centering Images

One of the ways to center an image is by using the `display` property, setting its value to `block`. You also need to use the `margin` property, setting the values of the left and right margins to `auto`.

```html
<!-- index.html -->

<img src="https://goo.gl/F6SGlE" class="medium align-center"  alt="Abrictosaurus" />
```

```css
/* css/styles.css */

img.align-center {
  margin: 0px auto;
}
```

[![](http://cd.sseu.re/20161123-pe97j.png)](http://cd.sseu.re/20161123-pe97j.png)

## ✏️ Exercise
> * In your `index.html` add an attribute to the opening tags of your images with the name `class` and the value `social-media-button`. Your code should look something like this:
> ```html
> <!--index.html-->
><body>
>  <h3>Find me online!</h3>
>
>  <span>
>     <a href="https://medium.com/">
>       <img src="https://medium.com/icons/monogram-mask.svg" alt="medium" class="social-media-button"/>
>     </a>
>  </span>
>  <span>
>    <a href="https://github.com">
>     <img src="https://cdn4.iconfinder.com/data/icons/iconsimple-logotypes/512/github-512.png" alt="github" class="social-media-button"/>
>    </a>
>  </span>
>  <span>
>    <a href="https://linkedin.com/">
>     <img src="https://png.icons8.com/metro/1600/linkedin.png" alt="linkedin" class="social-media-button"/>
>    </a>
>  </span>
>
>  <p>Have any questions? Get in touch!</p>
></body>
>```
> * In your `index.css`, add the following code: 
> ```css
> /*index.css*/
>
> .social-media-button {
>   height: 2rem;
> }
>```
> Check your page. It should look way better!
> ![page smaller pictures](https://cd.sseu.re/Jane_Doe_2018-09-06_12-13-13.png)

Next up, styling text!

## Text

### Specifying Typefaces

You can specify the typeface to be used by any text inside an element using the `font-family` property.

```css
body {
  font-family: Georgia, Times, serif;
}
h3 {
  font-family: "Courier New", Courier, monospace;
}
p {
  font-family: Arial, Verdana, sans-serif;
}
```

It is considered to be best practice to define a list of fonts for each of the elements and not only one. If the user does not have the first font installed, the browser will try to use any other from the list.

You should also end with a generic font name, like `serif`, `sans-serif` or `monospace`. These typefaces are installed on most computers.

### Size of Type

You will use the `font-size` property to specify the size of your font. You can use different units to do so:

#### Pixels

The number of pixels is followed by the letters `px`.

#### Percentages

Browsers have a default size of text of **16px** (100%). A size of 75% would be the equivalent of 12px, and 200% would be 32px.

#### EMS

An `em` is equivalent to the width of a letter `m`.

```css
body {
  font-family: Georgia, Times, serif;
  font-size: 14px;
}
h3 {
  font-size: 150%;
}
p {
  font-size: 1.2em;
}
```

### Bold and Italic

You can specify any text to be bold using the `font-weight` property. This property commonly take two values: `normal` or `bold`.

```css
.info {
  font-weight: bold;
}
```

You can use the `font-style` property to make text appear italic. This property commonly takes three values: `normal`, `italic` or `oblique`.

```css
.copy {
  font-style: italic;
}
```
## ✏️ Exercise
> * Add a font-family to the `body`-selector in `index.css`. 
> * Add a a rule to your `.footer`-selector in `index.css` with a property `text-align`, and a value `center`. Check the page in your browser!

## 😱 Sanity Check
Your page might now look something like this:
![page styling-a-specific-element](https://cd.sseu.re/Jane_Doe_2018-09-06_12-22-46.png)
You can find the code [here](https://github.com/Codaisseur/static-resume-page/tree/master/04-footer/03-styling-a-specific-element).

### 💡 Tips & Tricks
* colors can be defined by a [name, hex-color or rgb values](https://htmlcolorcodes.com/color-names/). Use a [color picker](https://htmlcolorcodes.com/color-picker/) to find the colors you like!
*  There are other ways in which you can "target" or select any element in your page and add styles to it. Check out [this article](http://www.w3schools.com/cssref/css_selectors.asp) for a full list of CSS selectors.

---
## 🎯 Learning Goal Tracker

* [x] How to add different sorts of text elements to your page.
* [x] The difference between a block and an inline element.
* [x] How to add a link to another page.
* [x] How to add an image element to your page.
* [x] How to style a specific element.
---
