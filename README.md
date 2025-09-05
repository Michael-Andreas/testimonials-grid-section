# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./images/Screenshot%20Desktop.png)

### Links

- Solution URL: [https://github.com/Michael-Andreas/testimonials-grid-section](https://github.com/Michael-Andreas/testimonials-grid-section)
- Live Site URL: [https://michael-andreas.github.io/testimonials-grid-section/](https://michael-andreas.github.io/testimonials-grid-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

How to tackle these kind of layouts with css grid. Also how to use the blockquote tag

```html
<blockquote>
  <p>
    “ I started as a total newbie with virtually no coding skills. I now work as
    a mobile engineer for a big company. This was one of the best investments
    I’ve made in myself. ”
  </p>
</blockquote>
```

```css
section {
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

article {
  grid-column: 2;
  grid-column-start: span 2;
  grid-column-end: auto;
}

article:nth-child(2),
article:nth-child(3) {
  grid-column: 1;
  grid-column-start: span 1;
  grid-column-end: auto;
}

article:nth-child(3) {
  grid-row-start: row2-start;
}

article:nth-child(5) {
  grid-row: 1 / 3;
  grid-column: 4 / 5;
}
```

### Useful resources

- [CSS Grid Layout Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) - This helped me to know which properties and values to use for the desktop grid.

## Author

- Website - [www.michaelandreas.de](https://michaelandreas.de)
- Frontend Mentor - [@Michael-Andreas](https://www.frontendmentor.io/profile/Michael-Andreas)
