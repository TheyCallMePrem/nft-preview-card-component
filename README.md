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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](images\screenshot.JPG)

### Links

- Live Site URL: [Add live site URL here](https://theycallmeprem.github.io/nft-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Hover effects, with adjescent sibling selector

```html
<div class="equi">
	<img class="img_eqi" src="images\image-equilibrium.jpg" alt="equilibrium" />

	<div class="hidden_img"></div>
	<img src="images\icon-view.svg" alt="" class="hidden-icon" />
</div>
```

```css
.hidden_img {
	position: absolute;
	top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	height: 100%;
	width: 100%;
	opacity: 0;
	background-color: hsl(178, 100%, 50%);
	border-radius: 10px;
}

.hidden-icon {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	text-align: center;
	display: none;
}

.equi:hover .hidden_img {
	opacity: 0.5;
	cursor: pointer;
}

.equi:hover .hidden_img + .hidden-icon {
	display: block;
}
```

### Continued development

I would like to study about hover effets and apply them in future projects.

### Useful resources

- [w3schools](https://www.w3schools.com/howto/howto_css_image_overlay_icon.asp) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.

## Author

- Github - [TheyCallMePrem](https://github.com/TheyCallMePrem)
- Frontend Mentor - [@TheyCallMePrem](https://www.frontendmentor.io/profile/TheyCallMePrem)
- Twitter - [@TheyCallMe_Prem](https://twitter.com/TheyCallMe_Prem)
