# Frontend Mentor - Clipboard landing page solution

This is a solution to the [Clipboard landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/clipboard-landing-page-5cc9bccd6c4c91111378ecb9). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- Solution URL: https://github.com/cosmonautkc/laughing-parakeet
- Live Site URL: https://cosmonautkc.github.io/laughing-parakeet/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (design tokens)
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project was mainly about strengthening my CSS fundamentals while intentionally using newer features to add them to my coding “vocabulary”.

I used `clamp()` for fluid typography instead of relying heavily on media queries. This helped keep responsiveness concise and easier to maintain. An example of a reusable class I created is below:

```css
.title {
  font-size: clamp(2rem, 3vw, 4rem);
  font-weight: var(--fw-600);
  line-height: 120%;
  color: var(--grey-700);
  padding-block: var(--sp-100);
}
```

I also used CSS Grid to create a full-bleed layout while constraining content width. This helped me better understand grid-based layout patterns, and centering techniques:

```css
.wrapper--snippets {
  display: grid;
  grid-template-columns: 1fr min(65ch, 100%) 1fr;
  padding-inline: var(--sp-150);
  justify-items: center;
}
```

Using these patterns helped reinforce how modern CSS can reduce the complexity while improving flexibility.

### Continued development

Going forward, I’ll continue using `clamp()` as it reduces the need for media queries, and keeps responsive logic on single lines of code.

I also want to improve consistency in spacing across layouts. This project had many sections, and several classes were used purely for margin/padding. Developing a clearer workflow for spacing utilities is something I want to keep refining in future projects.

## Author

- Frontend Mentor – https://www.frontendmentor.io/profile/cosmonautkc
- GitHub – https://github.com/cosmonautkc
