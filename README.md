# Frontend Mentor - Product Preview Card Component 👋🏾

![Desktop View](design/desktop-preview.jpg)

This the [Product preview card component](design/desktop-preview.jpg). Thanks for checking it out

## Table of contents 🧳

- [Overview](#overview)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

This is a product preview card component that is used in online shops to showcase products. Built mainly with flexbox.

### The objective

Users are be able to:

- View the optimal layout for the card depending on their device's screen size.
- See an active state when they click on the 'Add to cart' button.

### Screenshots

#### Mobile View

![Mobile View](design/mobile-design.png)

### Links

- Solution URL: [https://github.com/franco2ke/product-preview-card](https://github.com/franco2ke/product-preview-card)
- Live Site URL: [https://franco2ke.github.io/product-preview-card/](https://franco2ke.github.io/product-preview-card/)

## My process

I started by examining the design images and listing the key visible html elements required for the component. Once I had this list of elements, I proceeded to assign class names via the BEM methodology.

My development approach was to split the parent container into two child containers, one for the image and another for the product info, both positioned via flexbox. The product info layout was also done via flex box using the 'column' flex-direction.

Flexbox was the more practical choice for me because the component did not need much 2 dimensional positioning.Started with desktop view, then proceeded to mobile view. 

Effort was made to space elements using the 'gap' flex-box property, minimizing usage of margins where possible, with an aim of reducing work and also increasing the maintainability and resuability of the component.

The breakpoint chosen was 600px/ 37.5em. Looking good at all sizes between 1440px to 300px. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Desktop first workflow
- [SASS](https://sass-guidelin.es) - Sassy Sass
- [BEM](http://getbem.com/introduction/) - BEM methodology

### What I learned

Setting up the Art Direction; allowing the page to serve different images depending on screen width was something new for me.
From this problem, I see the need to brush up on loading and sizing images via html or css and the pros/cons of the various approaches.

```html
<!-- Art Direction; Different images for different screen widths -->
<picture class="product-card__img">
  <source srcset="./img/image-product-mobile.jpg" media="(max-width: 37.5em)" />
  <img src="./img/image-product-desktop.jpg" class="product-card__img" alt="" />
</picture>
```

### Useful resources

- [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML) - On the different options to load images.

## Author

- Website - [https://www.paon.co.ke](https://www.paon.co.ke)
- Frontend Mentor - [@franco2ke](https://www.frontendmentor.io/profile/franco2ke)
- Twitter - [@franco2ke](https://twitter.com/franco2ke)

Happy Coding 🎯
