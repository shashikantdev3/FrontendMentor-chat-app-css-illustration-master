# Frontend Mentor - Chat app CSS illustration solution

This is a solution to the [Chat app CSS illustration challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/chat-app-css-illustration-O5auMkFqY). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- **Bonus**: See the chat interface animate on the initial load

### Screenshot

![](./screenshot.jpg)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

In this project I have learned and implemented styling of input box:

1. Revome border from input box
2. Remove outline/border when input box is clicked
3. Add a svg inside input box
4. Style the placeholder

See below code snippets:

```html
<div class="type-msg">
            <label class="input-msg">
              <input type="text" placeholder="Type a message…">
            </label>
            
          </div>
```
```css
.input-msg>input{
    height: 2.5rem;
    min-width: 5rem;
    border: 0;
    border-radius: 1rem;
}

.input-msg>input:is(:active,:focus)
{
    border: 0;
    outline: none;
}

::placeholder{
    padding-left: 0.5rem;
    font-size: 0.75rem;
    color: #999;
}

.input-msg{
    background-color: var(--clr-white);
    border-radius: 1rem;
}

label.input-msg{
    position: relative;
}

label.input-msg::before{
    content: '\f138';
    display: inline-block;
    font-style: normal;
    font-variant: normal;
    text-rendering: auto;
    -webkit-font-smoothing: antialiased;
    font-family: "Font Awesome 5 Free"; 
    font-weight: 900; 
    position: absolute;
    top: -20%;
    left: 85%;
    font-size: 1.5rem;
    color: var(--clr-very-dark-desaturated-violet);;
}

```


### Continued development

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)


