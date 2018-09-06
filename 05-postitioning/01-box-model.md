# Box Model

### 💡 Not going through this chapter step by step? Find the starter code  for this chapter [here]().

### 🌟 A screen consists of `pixels`. Any HTML element in your page will have a `width` and `height`, that you can define in `pixels`.

[![](http://cd.sseu.re/20170208-aqays.png)](http://cd.sseu.re/20170208-aqays.png)

### 🌟 Any HTML element in your page will have a `margin`'s and `padding`'s, that you can also define in `pixels`.

[![](http://cd.sseu.re/20170208-dckoh.png)](http://cd.sseu.re/20170208-dckoh.png)

Let's look at some examples of how you can define these CSS properties:

```css
p {
  padding: 30px;
  margin: 10px;
}

.main-title {
 padding: 10px;
}

#taste-of-code {
   margin: 25px;
}
```

### Inspecting Elements in Chrome

Using Chrome DevTools, you can see and edit each element's properties very easily until you find the right dimensions for each of the areas listed above.

To open Crome DevTools press `CTRL + Shift + i` (Windows or Ubuntu) or `CMD + Option + i` (Mac), and the following panel will open:

[![](http://cd.sseu.re/20161125-cmgw8.png)](http://cd.sseu.re/20161125-cmgw8.png)

Let's not select any element of the page and inspect the current values for its margins, paddings and border. Scroll to the bottom of the section in the right, and you will see the following diagram:

[![](http://cd.sseu.re/20161125-92i74.png)](http://cd.sseu.re/20161125-92i74.png)

You can click in those values and edit them directly in the browser until you are happy with the results. After that, you can transfer those values into your stylesheet.

Let's now have a look at the most common CSS properties related to boxes.

### Box Dimensions

You can define the dimensions of any "box" or element in your HTML using the `width` and `height` properties.

```css
div {
  height: 300px;
  width: 400px;
}
```

You can also limit its width and height using the `min-width`, `max-width`, `min-height` and `max-height` properties.

### Borders

The `border` property allows you to specify the width, style and color of a border.

```css
p {
  width: 250px;
  border: 3px dotted #00AA86;
}
```

### Margin & Padding

You can specify the padding of an element with the `padding` property. This property will apply the same value to each side of the box.

```css
p {
  padding: 10px;
}
```

You can also specify different values for each side of the box using the properties `padding-top`, `padding-right`, `padding-bottom` and `padding-left`.

Or you can use the short form (where values would be in clockwise order: top, right, bottom, left).

```css
p {
  padding: 10px 5px 3px 6px;
}
```

You can use the `margin` property in a similar way as you do with the `padding` property.

## ✏️ Exercise
> * Remember the structure of our page?
> ![](https://cd.sseu.re/FireShot_Capture_1_-_Jane_Doe__-_file____Users_mimi_Code_Codaisseur_.png_2018-09-06_14-12-49.png)
>
>   * Our `body` (blue) consists of a `footer` and a `main` box (red)
>   * Inside our `main` box, there is a `side-bar` and a `more-info` box (orange)
>   * Inside our `more-info` box, there are a `work-experience` and a `education` box (yellow).
>   * Inside these boxes, there are even smaller boxes: the elements that we just learned about, such as `<h1>`, `<img>` and `spans`
> * Reflect this structure in your code. We'll use `div` elements to distinguish different components, and class attributes to distinguish them for styling. First wrap your footer in a `div` with the class `footer`:
> ```html
> <!--index.html-->
><body>
>   <div class="footer">
>     <h3>Find me online!</h3>
>     <!--Your spans-->
>     <p>Have any questions? Get in touch!</p>
>   </div>
></body>
>```
> * Now add the rest of the structure using the explanation above, `div` elements and classes.
><details>
>  <summary>
>     Try yourself first, click here to see the code!
>  </summary>
>
> ```html
> <!--index.html-->
><body>
>   <div class="main">
>     <div class="sidebar"></div>
>     <div class="more-info">
>       <div class="work-experience"></div>
>       <div class="education"></div>
>     </div>
>   </div>
>   <div class="footer">
>     <h3>Find me online!</h3>
>     <!--Your spans-->
>     <p>Have any questions? Get in touch!</p>
>   </div>
></body>
>```
> </p></details>



---
## 🎯 Learning Goal Tracker

In this section you will learn:

* [x] What the box model is
* [ ] How to use flex-box to position components on your page.
* [ ] How to add a box shadow to a component

---
