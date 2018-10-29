# Box Model



The chapter before, we ended up with this page:
![page box-model](https://cd.sseu.re/Jane_Doe_2018-09-06_15-27-16.png)
Nice, but it does not look very much like our website yet. Let's start positioning our components!

# Intro to flex box

With the box model, you can style any element anywhere. Most developers think it isn't intuitive. It needs some magic to let your footer always stick to the bottom of the page on each and every screen. 

## Flexible boxes

Flexboxes make it easier to style your content for multiple devices and screen sizes. It does this by identifying a containing element, called the `flex-container`. This container has no content of itself, but it holds your `flex-items`, the elements that hold the content intended for your user. 

Graphically that looks like this:
![flex-container-with-flex-items](http://cd.sseu.re/flex-container-with-flex-items.png)

### Navigation with a flexbox

Consider this example (without flexbox) for navigation:
```html
<nav>
  <li class="about">About</li>
  <li class="contact">Contact</li>
  <li class="home">Home</li>
</nav>
```
```css
nav {
  background: #333;
  list-style: none;
  padding: 5px;
}

li {
  padding: 20px;
  background: red;
  margin: 20px;
}

html {
  color: white;
  font-family: sans-serif;
}
```

This will render something like this:
![nav without flexbox](http://cd.sseu.re/A_Pen_by_Arno_Fleming_2017-06-21_12-00-05.png)
No surprises here. Let add flexboxing on the nav and see what looks different:
```css
nav {
  background: #333;
  list-style: none;
  padding: 5px;
  
  display: flex;
}

/* other styles omitted for brevity */
```
![nav with flexbox](http://cd.sseu.re/Example-flex-navigation_2017-06-21_11-25-00.png)

Hmm... That starts to look like a navbar to me! :)

It would be nice if these buttons would move to the right, or in flex terminology, to justify the content to the end of the flex container.

```css
nav {
  background: #333;
  list-style: none;
  padding: 5px;
  
  display: flex;
  justify-content: flex-end;
}
```
![nav with items at the end](http://cd.sseu.re/Example-flex-navigation_2017-06-21_11-31-09.png)

### Flexbox and screensizes

This is a nice layout of elements for a navigation in a browser, but the navigation isn't much help on a small screen like your users smartphones. This means that we want to see the layout from above on somewhat wide screens, but thumb-safe navigation on smaller displays. 

Here some CSS magic combines really well with Flexible Boxes.
```css
/* All previous styles omitted for brevity */

/* Too narrow to support three columns */

@media all and (max-width: 640px) {
  nav {
    flex-direction: column;
  }

  nav li {
    min-height: 50px;
    max-height: 50px;
  }
}
```
You force the size of the navigation items (`nav li`) to be exactly 50px, so your thumb won't inadvertently touch multiple items.
![small screen nav](http://cd.sseu.re/Example-flex-navigation_2017-06-21_11-54-28.png)

But wait, we can make more changes that make sense on a small screen. 

We will not `display` the navigation for contact, and re`order` home and about. Lets add some code to our css for small screens:

```css
@media all and (max-width: 640px) {
  nav {
    flex-direction: column;
  }

  nav li {
    min-height: 50px;
    max-height: 50px;
  }

  li.home {
    order: 0;
  }

  li.contact { 
    order: 1; 
  }

  li.about { 
    display: none;
  }
}
```
![altered small screen nav](http://cd.sseu.re/Example-flex-navigation_2017-06-21_11-57-07.png)

Sweet!

See [this codepen](https://codepen.io/ArnoFleming/pen/JJNeEd) for the end result.

## ✏️ Exercise
> * Change your the css code of your `main` container in such a way that the `sidebar` and the `more-info` component are placed next to each other.
><details>
>  <summary>
>     Check the code!
>  </summary>
>
>   ![](https://cd.sseu.re/Jane_Doe_2018-09-06_15-11-20.png)
> </details>
>
> * Add the following code to your `index.css`
>  ```css
>  .sidebar {
>    flex-grow: 1;
>  }
>  
>  .more-info {
>    flex-grow: 2;
>  }
>  ```

## 😱 Sanity Check
Your page should now look something like this:
![page styling-a-specific-element](https://cd.sseu.re/Monosnap_2018-09-06_15-42-47.png)
You can find the code [here]().

---
## 🎯 Learning Goal Tracker

In this section you will learn:

* [x] What the box model is
* [x] How to use flex-box to position components on your page.
* [ ] How to add a box shadow to a component

---
