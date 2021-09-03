# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

![Screenshot 2021-09-02 at 21-15-06 Frontend Mentor 3-column preview card component](https://user-images.githubusercontent.com/32622980/131935795-f3c1e852-e321-4754-8064-2a876d422ea4.png)
![cropped-Screenshot 2021-09-02 at 21-36-57 Frontend Mentor 3-column preview card component](https://user-images.githubusercontent.com/32622980/131937864-357da5d9-7af4-4cff-bde0-432d21fc3ae3.png)


### Links

- Solution URL: https://github.com/JonMStevens/frontend-mentor-3-column-preview-card-component/
- Live Site URL: https://jonmstevens.github.io/frontend-mentor-3-column-preview-card-component/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid

### What I learned

Got more comfortable with grid...
Grid
minmax function
clamp function
```css
#main {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  width: clamp(350px, 66vw, 80vw);
  margin: 4rem auto 4rem auto;
}
```

Got to make good use of transparent (alpha) colors. On hover the buttons will show the color of the card they are on.
```css
.card button:hover {
  color: var(--transparent-white);
  cursor: pointer;
  background: rgba(0 0 0 / 0);
  box-shadow: 0 0 0 2px currentColor;
}
```

### Continued development

- I still need to practice with grid more before I am fully comfortable with it.
- Also, I would like to understand better how to center things vertically on a page and keep them visible when the page is larger than the screen size.


### Useful resources
- [10 modern layouts in 1 line of CSS](https://youtu.be/qm0IfG1GyZU?t=715) - I stole the responsive grid layout from Una Kravets video. She calls is the RAM (Repeat, Auto, Minmax) layout.
- [css-tricks forum: border radius for outline](https://css-tricks.com/forums/topic/border-radius-for-outline/) - This is where I learned I should use box shadow for a round outline. At first, my outlines were shaped like rectangles on chrome.

## Author

- Frontend Mentor - [@JonMStevens](https://www.frontendmentor.io/profile/JonMStevens)
