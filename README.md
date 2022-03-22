# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Four card feature section solution](#frontend-mentor---four-card-feature-section-solution)
  - [Table of contents](#table-of-contents)
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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./public/assets/designs/desktop-design.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- SCSS Architecture
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

There were some hurdles to overcome with this project. One of those was trying to get use to working with the calc() function and clamp() to create a more fluid typography. Also learned how to better use grid-template areas to easily layout the cards.

To see how you can add code snippets, see below:

```css
.title__primary {
  @extend %text-modules;
  @extend %ctr-txt;
  @include text-prop(
    $size: clamp(1.13rem, 6vw, 1.9rem),
    $f-weight: $font-weight-light,
    $color: $color-text-base
  );
  font-weight: $font-weight-light;
  color: $color-text-base;
  padding-top: px-to-rems(75px);
}

.main__grid--container {
  @include grid_layout_container();
  margin-top: px-to-rems(40px);
  @include mq("md") {
    margin-top: px-to-rems(55px);
  }
}

// Grid Area Items
.supervisor {
  grid-area: supervisor;
}

.team-builder {
  grid-area: team-builder;
}

.karma {
  grid-area: karma;
}

.calculator {
  grid-area: calculator;
}
```

### Continued development

I will continue to work with using CSS Grid Template areas to layout content and to better understand using css clamp and calc to build layouts faster

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Brian Johnson](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**
