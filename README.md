# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Links

- Solution URL: [Add solution URL here](https://www.frontendmentor.io/solutions/responsive-layout-using-grid-and-flex-1LtBBv5eAs)
- Live Site URL: [Add live site URL here](https://sen-nyin.github.io/FEM-stats-preview/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- Mix-blend-modes for image overlays

### What I learned

At first I set the images up with a linear-gradient overlay, but noticed the colouring didn't perfectly match the example. I had to go away and learn about mix-blend-mode to get the job done, setting a background colour to the main image container and set the image as a background to an ::after.

To see how you can add code snippets, see below:

```css
.stats__image::after {
  content: "";
  width: 100%;
  height: 100%;
  background: url(../images/image-header-mobile.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  position: absolute;
  top: 0;
  left: 0;
  mix-blend-mode: multiply;
  opacity: 0.75;
}
```

### Continued development

I think this project highlighted my need to do some additional research on image backgrounds. I had originally planned to use the picture element with media sources to switch between the mobile and desktop images, but found this approach problematic with the sizing, so switched to CSS backgrounds.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Sen-Nyin)
- Twitter - [@LeonLonsdale](https://www.twitter.com/LeonLonsdale)

