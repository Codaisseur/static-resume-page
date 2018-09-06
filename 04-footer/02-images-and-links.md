# Links and Images

### 💡 Not going through this chapter step by step? Find the starter code  for this section [here]().

Right now, our page looks like this: ![page html-elements](https://cd.sseu.re/Jane_Doe_2018-09-06_10-46-59.png)

Next, you will change the social medium titles into links, so they will link to your profiles!

## Links

I know you were looking forward to this part, since links are the most important feature of the web, since thanks to them you can navigate from page to another.

### Linking to other sites

You can create links using the `<a>` element. You should always specify which page you want to link to using the `href` attribute.

```html
<a href="https://reader.codaisseur.com">Codaisseur Reader</a>
```

### Linking to other pages on the same site

If you want to link to other pages within your site, there is no need to specify the domain name in the URL. This is what it's called a **relative URL**.

Remember that, if you are placing all the pages of your site in the same folder, the value of the `href` attribute is just the name of the file.

```html
<nav>
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
  <a href="contact.html">Contact</a>
</nav>
```

### Opening links in a new window

You can add an extra attribute `<target>` to the `<a>` element to open any link in a new window.

```html
<a href="https://reader.codaisseur.com" target="_blank">Codaisseur Reader</a>
```
## ✏️ Exercise
> * Add a link element inside each of your span elements:
> ```html
> <!--index.html-->
><body>
>  <h3>Find me online!</h3>
>
>  <span>
>     <a href="https://medium.com/">Medium</a>
>  </span>
>  <span>
>    <a href="https://github.com">GitHub</a>
>  </span>
>  <span>
>    <a href="https://linkedin.com/">LinkedIn</a>
>  </span>
>
>  <p>Have any questions? Get in touch!</p>
></body>
>```
> * Check your page in the browser. What happens when you click one of the links?

So far so good! However, it would be even cooler if we could replace the boring text by some images:
![Social Media Buttons](https://cd.sseu.re/Jane_Doe_2018-09-06_11-07-30.png)

## Images

### Adding images

To add images to your site, you will use the `<img>` element. Notice that there is no closing tag for this case. It should have the following two attributes:

* `src` tells the browser where to find the image file. It accepts a link to the image on the internet, or if your images are stored on your site, the "path" to the folder where it's stored.

* `alt` provides a text description of the image. If for some reason the image doesn't show, this text will be displayed instead.

```html
<!-- Image loaded from the internet -->
<img src="https://goo.gl/F6SGlE" alt="Abrictosaurus" />

<!-- Image stored on your site or locally -->
<img src="images/abrictosaurus_dinosaur.png" alt="Abrictosaurus" />
```

It is considered to be good practice to create a folder for all of the images that you will use in your site. You can call this folder `images`.

## ✏️ Exercise
> * Add an image element inside each of your link elements:
> ```html
> <!--index.html-->
><body>
>  <h3>Find me online!</h3>
>
>  <span>
>     <a href="https://medium.com/">
>       <img src="https://medium.com/icons/monogram-mask.svg" alt="medium"/>
>     </a>
>  </span>
>  <span>
>    <a href="https://github.com">
>     <img src="https://cdn4.iconfinder.com/data/icons/iconsimple-logotypes/512/github-512.png" alt="github"/>
>    </a>
>  </span>
>  <span>
>    <a href="https://linkedin.com/">
>     <img src="https://png.icons8.com/metro/1600/linkedin.png" alt="linkedin" />
>    </a>
>  </span>
>
>  <p>Have any questions? Get in touch!</p>
></body>
>```
> * Check your page in the browser. Click on the images. Do they still work?

## 😱 Sanity Check
Your page might now look something like this:
![page images-and-links](https://cd.sseu.re/FireShot_Capture_2_-_Jane_Doe__-_file____Users_mimi_Code_Codaisseur_.png_2018-09-06_11-16-42.png)

Clearly, it is time to do some styling!

---
## 🎯 Learning Goal Tracker

* [x] How to add different sorts of text elements to your page.
* [x] The difference between a block and an inline element.
* [x] How to add a link to another page.
* [x] How to add an image element to your page.
* [ ] How to style a specific element.
---
