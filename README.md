# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![Screenshot](./screenshot.jpg)

### Links

- Solution URL: [https://github.com/cybercoder-naj/social-proof-section-master.git](https://github.com/cybercoder-naj/social-proof-section-master.git)
- Live Site URL: [https://cybercoder-naj.github.io/social-proof-section-master/](https://cybercoder-naj.github.io/social-proof-section-master/)

## My process

### Built with

- Semantic HTML5 markup
- SASS 
- Flexbox
- CSS Grid
- Media Queries: Mobile-first workflow

### What I learned

I used the SASS language with proper implementation today, along with complex mixins and for-loops. I was able to structure my HTML DOM in a oraganised way.

```scss
@mixin shift-ratings {
  @for $i from 1 through 3 {
    .rating:nth-child(#{$i}) {
      margin-left: ($i - 1) * 5%;
    }
  }
}
```

This way, I did not have to individually use the `:nth-child` property for each element.

```scss
.rating {
  background: lighten(map-get($primary-colors, dark-magenta), 72%);
}
```

I used functions like `lighten`, `darken` and `map-get` to effectively structure my stylesheet in a readable way.

### Useful resources

- [Learn Sass in this Free Crash Course - Give your CSS Superpowers!](https://www.youtube.com/watch?v=roywYSEPSvc) - This gave a new insight on mixins and media queries. They become easier with the Sass annotation `@content`.
- [Sass Documentation](https://sass-lang.com/documentation) - This is an amazing documentation which helped me revise the concepts of Flow-Control, functions and mixins.
- [W3Schools](https://www.w3schools.com/howto/howto_css_star_rating.asp) - This gave me the code for a Star Rating in the HTML DOM.

## Author

- Frontend Mentor - [@cybercoder-naj](https://www.frontendmentor.io/profile/cybercoder-naj)
- LinkedIn - [Nishant Aanjaney Jalan](https://www.linkedin.com/in/nishant-aanjaney-jalan-3b7659191/)


---