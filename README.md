# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Flexbox

### What I learned

I am learning about overlaying image when hovering like this

```html
<div class="container">
  <img
    src="images/image-equilibrium.jpg"
    alt="image-equilibrium"
    width="100%"
  />
  <div class="overlay">
    <img src="images/icon-view.svg" alt="icon-view" width="50" />
  </div>
</div>
```

```css
.container {
  position: relative;
  margin-bottom: 10px;
}

.container img,
.container .overlay {
  border-radius: 10px;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 3px;
  left: 0;
  right: 0;
  opacity: 0;
  transition: 0.5s ease;
  background-color: var(--cyan-bg);
  display: flex;
  justify-content: center;
  align-items: center;
}

.container:hover .overlay {
  opacity: 1;
}
```

### Useful resources

- [W3School](https://www.w3schools.com/)

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)
