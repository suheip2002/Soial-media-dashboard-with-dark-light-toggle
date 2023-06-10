# Frontend Mentor - Social media dashboard with theme switcher solution

This is a solution to the [Social media dashboard with theme switcher challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-media-dashboard-with-theme-switcher-6oY8ozp_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- SASS

### What I learned

I learned two things when i was building this project:
1. It was my first time to use SASS.
2. Also my first time to add a dark and light mode toggle switcher in a website

```html
 <fieldset class="header__toggle toggle" aria-label="theme toggle" role="radiogroup">

      <label for="dark">Dark mode<span class="visually-hidden">on</span></label>

      <div class="toggle__wrapper">
        <input type="radio" name="theme" id="dark">
        <input type="radio" name="theme" id="light">
        <span aria-hidden="true" class="toggle__background"></span>
        <span aria-hidden="true" class="toggle__button"></span>
      </div>

      <label for="light" class="visually-hidden">Dark mode off</label>

    </fieldset>
```
```css
@use "sass:math";

@function rem($pixels, $context: 16) {
    @return (math.div($pixels, $context)) * 1rem;
}
```
```js
window.matchMedia('(prefers-color-scheme: dark)')
    .addEventListener('change', (event) => {
    event.matches ? darkButton.click() : lightButton.click();    
});
```

### Continued development

It was my first time to use sass and it was a lot of fun and good exprience building with this project and i hope to use it in my future projects as well.

### Useful resources

- (https://www.youtube.com/watch?v=krfUjg0S2uI&t=22676s) - This helped me for building the project using SASS my first time.

## Author

- Frontend Mentor - [@suheip2002](https://www.frontendmentor.io/profile/suheip200)
