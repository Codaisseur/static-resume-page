# Box Model



The chapter before, we ended up with this page:
![page styling-a-specific-element](https://cd.sseu.re/Monosnap_2018-09-06_15-42-47.png)

Do you also think those black borders are a little boring? Let's add some 3D effects, using box shadow!

## ✏️ Exercise
> * There is a `box-shadow` property. Can you find out how it works?
>
><details>
>  <summary>
>     Hint
>  </summary>
>
>   [Check out MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)
> </details>
>
> * Add the `box-shadow` property to the `sidebar`, `work-experience` and `education` selectors in `index.css`. To make it even more fancy, you could add a shadow on top of the first shadow! That would look like this:
> ```css
> .sidebar {
>  flex-grow: 1;
>  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>}
> ```
>
> * Remove the border property from the `<div>` selector.
>
><details>
>  <summary>
>     Code not working? Check the CSS!
>  </summary>
>
>  ```css
>  .sidebar {
>    flex-grow: 1;
>    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>  }
>  
>  .work-experience {
>    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>  }
>
>  .education {
>    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>  }
>  ```
> </details>

## 😱 Sanity Check
Your page should now look something like this:
![page box-shadow](https://cd.sseu.re/Monosnap_2018-09-06_16-12-05.png)
You can find the code [here]().


---
## 🎯 Learning Goal Tracker

In this section you will learn:

* [x] What the box model is
* [x] How to use flex-box to position components on your page.
* [x] How to add a box shadow to a component

---
