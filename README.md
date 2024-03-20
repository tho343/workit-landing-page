# Frontend Mentor - Workit landing page solution

This is a solution to the [Workit landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/workit-landing-page-2fYnyle5lu). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](../assets/images/Screenshot%202024-03-19%20at%2010.37.15%20PM.png)


### Links

- Solution URL: (https://github.com/tho343/workit-landing-page)
- Live Site URL: (https://tho343.github.io/workit-landing-page/)

## My process

- Started with HTML structure and meta links
- Applied styles from top to bottom
- Lastly, added responsiveness

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Boostrap5


### What I learned

From this project I learned:

- Limit the elements size to avoid it from growing when expanding the browser window. 
- Apply wrapper to some elements if needed
- color text changing CSS effect on links
```html
<div class=wrapper>
<a href=#><span data-content = "Click here" aria-hidden="true"></span>Click here</a>
<div>
```
```css
.wrapper {
  position: relative;
}

span {
  position: absolute;
  overflow: hidden;
  top:0;
  left: 0;
  transform: translateX(-100%);
  transition: transform 275ms ease;
}

span::before{
  display: inline-block;
    content: attr(data-content);
    color:var(--secondary-color1--);
    z-index: 10000;
    transform: translateX(100%);
    transition: transform 275ms ease;
}
a:hover span{
    transform: translateX(0);
}

a:hover span::before{
    transform: translateX(0);
}


```

### Continued development

- Continuue to learn clip-path to create the curve border


## Author

- Website - [Tran Ho](https://tho343.github.io/tran-website/)
