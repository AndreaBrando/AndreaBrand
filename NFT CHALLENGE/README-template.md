# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./Screenshot%202022-03-14%20at%2017-53-58%20Frontend%20Mentor%20NFT%20preview%20card%20component.png)

### Links

- Solution URL: [Add solution URL here](https://lucid-neumann-ece86f.netlify.app//)
- Live Site URL: [Add live site URL here](https://lucid-neumann-ece86f.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I'm pretty newbie when it comes to code autonomously (and for the first time in SASS) but I tried my best.
the 'hover' section is what I had problems with. I thought that by simply adding "img:hover" (for the main-image) and the cyan color it would've worked just fine. I learnt I had to add an overlay with the 'eye' icon on top of the image, so I'm happy with the result and glad that I figured it on my own. I apologize for the imperfections, there may be some, but overall I had fun with this challenge.
NOTE: I tried using 'display:none' for the overlay, but didn't work. I opted for the opacity interpolation.
Here's my code snippet (in SASS) for the overlay:

```html
<section class="image">
  <img src="./images/icon-view.svg" alt="" class="overlay" />
  <img
    src="images/image-equilibrium.jpg"
    alt="Equilibrium image"
    class="picture"
  />
</section>
```

```css
.image {
  position: relative;
}
.overlay {
  height: 296.06px;
  width: auto;
  border-radius: 1.5rem;
  position: absolute;
  background-color: rgba($color: $cyan, $alpha: 0.6);
  object-fit: scale-down;
  opacity: 0;
  transition: opacity 0.2s ease-in-out;
}

.picture {
  height: 296.06px;
  width: auto;
  border-radius: 1.5rem;
}
/*OVERLAY*/
.overlay:hover {
  cursor: pointer;
  opacity: 100;
}
```

### Continued development

I need to get better at coding and organizing my pages. Too often I had to stop to clean up some unecessary lines because of my 'Trial and error' approach. Resulting in taking too much time for a simple page. Secondly I'm wasnt' that confident when I started styling with CSS: I had to check 'Stack Overflow' or 'W3Schools' multiple times, i'd like to not rely too much on them and try to solve it on my own.

### Useful resources

- [Resource 1](https://www.w3schools.com/) - The well-known website W3schools was very helpful to me whenever I need it. Surely it's an useful resource.
- [Resource 2](https://stackoverflow.com/) - Stack Overflow is a goldmine of resources. usually there I was able to find solutions to most of my problems.
- [Resource 3](https://www.amazon.it/Progettare-costruire-Contenuto-digitale-download/dp/8850334044/ref=asc_df_8850334044/?tag=googshopit-21&linkCode=df0&hvadid=85509557663&hvpos=&hvnetw=g&hvrand=7605172766657923674&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1008588&hvtargid=pla-296660299438&psc=1) - I initially read this book when I started with HTML/CSS. Though some of the stuff in it is obsolete ( for instance there's a section about flash, now discontinued, and doesn't have a 'Flexbox' section) is graphically very well made and gives some insight about some deprecated codes, (the link directs to the italian version).

## Author

- Frontend Mentor - [@AndreaBrando](https://www.frontendmentor.io/profile/AndreaBrando)
