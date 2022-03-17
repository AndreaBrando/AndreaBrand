# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author))

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](Screenshot%202022-03-17%20at%2017-04-33%20Frontend%20Mentor%20QR%20code%20component.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://admiring-goodall-0b3d26.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

On my previous challenge, the nft card, i set the flex-direction: column property on main and I wondered why the box didn't scale down. I've found out that by adding column on .card (the box) it actually worked. I'm going to highlight the code:

```html
<main>
  <section class="card">
    <header>
      <img src="./images/image-qr-code.png" alt="qr code" />

      <h1>Improve your front-end skills by building projects</h1>
      <p>
        Scan the QR code to visit Frontend Mentor and take your coding skills to
        the next level
      </p>
    </header>
  </section>
</main>
```

```css
main {
  min-height: 98vh;
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  flex-wrap: wrap;
}
.card {
  flex-direction: column;
  box-shadow: 5px 5px 15px 1px hsl(213, 15%, 76%);
  padding: 1em;
  background-color: var(--box);
  border-radius: 1.5rem;
  width: 21em;
  display: flex;
}
```

### Continued development

I've found out some errors on the previous challenge and hopefully fix them here (probably gonna redo it cause I think it can be better). Still not perfect but better than the previous one. But during styling CSS I mistakenly went on styling html elements before setting general css properties.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

## Author

- Frontend Mentor - [@AndreaBrando](https://www.frontendmentor.io/profile/AndreaBrando)
