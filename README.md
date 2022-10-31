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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Screenshot](https://github.com/Fqthom/Testimonials/blob/f72a9d1657312a35c520f3a0656ca4ba84793ef5/images/Testimonials_Screenshot.png)

### Links

- Solution URL: [Github](https://github.com/Fqthom/Testimonials)
- Live Site URL: [Github Pages](https://fqthom.github.io/Testimonials/)

## My process
My process started with a desktop first approach. 
At first attempt, I attempted to flex mulitiple divs to achieve the grid style layout, before discovering the grid system in CSS. Grid is new to me and it was an interesting challenge diving into this mid-project with no priot knowledge. This approach was a bit half-hazard, but eventually arrived at the finished project.

I originally had created simple hover actions when hovering over each card *as you'll see in the stylesheet*, but in the end opted away from those, due to feedback of it being a bit overwhelming for the simplicity of the page.

I'm self taught as a hobby, and I imagine alot of my CSS isn't streamlined, so any feedback is more than welcome.
### Built with

- Semantic HTML5 markup *(kind-of)*
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Grid was a stuggle to get the div's to behave properly according to the sizing.
Learning template areas as well as setting column widths with 'fr' measurements ended up tying the entire project together.

## *The code that tied it together*
```css
.main{
    margin: 0 0;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: auto auto;
    grid-template-areas: 
        'card1 card1 card2 card3'
        'card4 card5 card5 card3';
    gap: 30px;
}
```

### Continued development

- Grid system
- HTML semantics
- IDs

I find myself creating nested divs and classes for almost each individual items instead of minimizing my code and utilizing IDs for specific changes within repeating divs.

### Useful resources

- ['fr' measurement CSS'](https://css-tricks.com/introduction-fr-css-unit/)

The key article that helped me understand the 'fr' measurement to keep my grid's in order. If you're having overflow issues within your columns, reference this great article!

## Author

- Website - [Fqthom](https://www.github.com/Fqthom)
- Frontend Mentor - [@Fqthom](https://www.frontendmentor.io/profile/Fqthom)
