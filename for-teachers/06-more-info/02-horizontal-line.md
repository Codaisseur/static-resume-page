# Horizontal Line



Last chapter we ended up with a page like this: ![page title-with-icon](https://cd.sseu.re/Monosnap_2018-09-06_16-50-43.png)

Did you see those nice little dividers? ![dividers](https://cd.sseu.re/FireShot_Capture_1_-_Jane_Doe__-_file____Users_mimi_Code_Codaisseur_.png_2018-09-06_17-10-57.png)

Let's add them to our page!

## ✏️ Exercise
> * Go to [ example page](https://serene-mcnulty-aa84b3.netlify.com/).
> * Inspect one of the divider elements. Which HTML elements do you see? Which styles are being applied?
> * Write a horizontal rule in your own code. Apply styling. Which of the styling you found in your Dev Tools is applied automitcally? Which one did you need to apply yourself?
>
><details>
>  <summary>
>     Can't figure it out? Check the Code!
>  </summary>
>
>   ```html
>   <!--index.html-->
>    <div class="work-experience">
>      <h1 class="section-title">
>        <span>
>          <img src="http://shopforclipart.com/images/open-suitcase-clipart/8.jpg" alt="red suitcase" class="title-icon" />
>        </span>
>        Work Experience
>      </h1>
>      <hr class="divider" />
>    </div>
>    <div class="education">
>      <h1 class="section-title">
>        <span>
>          <img src="https://delta.ncsu.edu/ar/2012-2013/image/infographic/degrees-certificates.png" alt="red suitcase" class="title-icon"
>      />
>        </span>
>        Education
>      </h1>
>      <hr class="divider" />
>    </div>
>   ```
>
>   ```css
>   /* index.css */
>    .divider {
>       margin: 2rem 0;
>    }
>
>    .work-experience {
>      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>      padding: 2rem;
>    }
>
>    .education {
>      box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
>      padding: 2rem;
>    }
>   ```
>
> </details>

## 😱 Sanity Check
Your page should now look something like this:
![page horizontal-line](https://cd.sseu.re/Monosnap_2018-09-06_20-25-01.png)
You can find the code [here]().

---
## 🎯 Learning Goal Tracker

* [x] Position an icon and title next to each other
* [x] Add a horizontal rule
* [ ] Easily add some fake text to your website.

---
