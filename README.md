# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Reference](#reference)
  - [Color](#color)
  - [Typography](#typography)
  - [Font](#font)
- [Run Locally](#run-locally)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![Profile card component desktop screenshot](https://devshaunb.github.io/fem-profile-card-component/screenshots/desktop.png)

![Profile card component mobile screenshot](https://devshaunb.github.io/fem-profile-card-component/screenshots/mobile.png)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/profile-card-component-with-flexbox-4akI1GuwqV](https://www.frontendmentor.io/solutions/profile-card-component-with-flexbox-4akI1GuwqV)

- Live Site URL: [https://devshaunb.github.io/fem-profile-card-component/](https://devshaunb.github.io/fem-profile-card-component/)

## Reference

### Color

#### Primary

- ![hsl(185, 75%, 39%)](https://via.placeholder.com/10/19a2ae?text=+) `Dark cyan: hsl(185, 75%, 39%)`
- ![hsl(229, 23%, 23%)](https://via.placeholder.com/10/2d3248?text=+) `Very dark desaturated blue: hsl(229, 23%, 23%)`
- ![hsl(227, 10%, 46%)](https://via.placeholder.com/10/6a6f81?text=+) `Dark grayish blue: hsl(227, 10%, 46%)`

#### Neutral

- ![hsl(0, 0%, 59%)](https://via.placeholder.com/10/969696?text=+) `Dark gray: hsl(0, 0%, 59%)`

### Typography

#### Body Copy

- Font size (paragraph): 18px

### Font

- Family: [Kumbh Sans](https://fonts.google.com/specimen/Kumbh+Sans)
- Weights: 400, 700

## Run Locally

Clone the project

```bash
  git clone https://github.com/DevShaunB/fem-profile-card-component.git
```

Go to the project directory

```bash
  cd fem-profile-card-component/
```

Run `index.html`

```bash
  <browsername> index.html
```

E.g.

```bash
  firefox index.html
```

```bash
  google-chrome index.html
```

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS custom utility classes
- Flexbox
- Mobile-first workflow

### What I learned

- add background patterns with pseudo-elements

```css
main {
  min-height: 100vh;
  position: relative;
  z-index: 0;
  overflow: hidden;
}

main::before,
main::after {
  content: '';
  width: 100%;
  height: 100%;
  position: absolute;
  transform: translate(-50%, -50%);
  z-index: -1;
}

main::before {
  top: 0;
  left: 0;
  background: url('./images/bg-pattern-top.svg') no-repeat bottom right / cover;
}

main::after {
  top: 100%;
  left: 100%;
  background: url('./images/bg-pattern-bottom.svg') no-repeat top left / cover;
}
```

- move image around within the parent container

```css
.profile-card__content {
  position: relative;
}

.profile-card__user-img-wrapper {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

## Author

- Frontend Mentor - [@DevShaunB](https://www.frontendmentor.io/profile/DevShaunB)
- Twitter - [@DevShaunB](https://www.twitter.com/DevShaunB)

## Acknowledgments

- [Profile card component](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ) by [Frontend Mentor](https://www.frontendmentor.io/)
