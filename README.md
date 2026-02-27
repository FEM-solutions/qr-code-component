# Frontend Mentor - QR Code Component

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H), part of learning path [Getting started on Frontend Mentor](https://www.frontendmentor.io/learning-paths/getting-started-on-frontend-mentor-XJhRWRREZd).

## Table of contents

- [Overview](#overview)
  - [Learning goals](#learning-goals)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Project Structure](#project-structure)
  - [Front-end style guide](#front-end-style-guide)
    - [Colors](#colors)
    - [Font](#font)
    - [Layout](#layout)
  - [What I learned](#what-i-learned)
    - [Semantic HTML Structure](#semantic-html-structure)
    - [CSS styles](#css-styles)
      - [CSS structure](#css-structure)

- [How to run locally](#how-to-run-locally)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Learning Goals

- Master semantic HTML structure
- Improve CSS layout techniques (Flexbox)
- Build responsive components that work on all devices

### The challenge

The challenge was to build out this QR code component and get it as close as possible to the original design.

### Screenshot

![QR code component desktop screenshot](./screenshots/desktop-screenshot.png)

[View more here](./screenshots/)

### Links

- Live Site URL: [https://fem-solutions.github.io/qr-code-component](https://fem-solutions.github.io/qr-code-component)
- Solution URL: [https://www.frontendmentor.io/solutions/card-component-built-with-css-custom-properties-krZg583OIP](https://www.frontendmentor.io/solutions/card-component-built-with-css-custom-properties-krZg583OIP)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Figma design

### Project Structure

```
qr-code-component/
|
|--- .gitignore
|--- README.md
|--- index.html
|--- CSS/
|    |--- base.css
|    |--- main.css
|    |--- tokens.css
|    |--- layout.css
|    |--- components/
|         |--- card.css
|         |--- footer.css
|--- IMAGES/ (project images)
|--- SCREENSHOTS/ (screenshots for mobile, tablet and desktop screens)
```

#### Front-end Style Guide

##### Colors

```
- White: hsl(0, 0%, 100%)
- Slate 300: hsl(212, 45%, 89%)
- Slate 500: hsl(216, 15%, 48%)
- Slate 900: hsl(218, 44%, 22%)
```

##### Font

- Font size (paragraph): 15px
- Family: `Outfit`
- Weights: `400, 700` (regular, bold)

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;700&display=swap"
  rel="stylesheet"
/>
```

##### Layout

- 320px > 768px: small screens
- 768px > 1440px: medium and large screens

### What I learned

#### Semantic HTML Structure

This component follows a **single-component architecture** `article`:

`article` represents a complete self-contained composition.

```html
<article>
  <img src="./images/image-qr-code.png" alt="QR code for Frontend Mentor" />
  <h1>Improve your front-end skills by building projects</h1>
  <p>
    Scan the QR code to visit Frontend Mentor and take your coding skills to the
    next level
  </p>
</article>
```

#### CSS styles

- Implemented a design system based on the `Figma design` and style guide, using `CSS custom properties` for colors, font styles and elements spacing
- `logical properties`
- `rem units` for responsive
- `Media prefers-reduced-motion` for links

##### CSS Structure

- Main stylesheet path in `index.html`

```html
<link rel="stylesheet" href="./main.css" />
```

`main.css` import stylesheets:

```css
/* 1. TOKENS - Variables */
@import "tokens.css";

/* 2. BASE - Global styles, reset, typography */
@import "base.css";

/* 3. LAYOUT - Page structure*/
@import "layout.css";

/* 4. COMPONENTS */
@import "components/card.css";
@import "components/footer.css";
```

## How to Run Locally

1. Clone this repository:

```bash
git clone https://github.com/FEM-solutions/qr-code-component.git
```

2. Navigate to project folder:

```bash
cd qr-code-component
```

3. Open `index.html`in your browser or use Live Server in VS Code.

## Author

- Frontend Mentor - [@amansgz](https://www.frontendmentor.io/profile/amansgz)
- Github - [@amansgz](https://github.com/amansgz)

## Acknowledgments

- [Frontend Mentor](https://www.frontendmentor.io/) challenges help you improve your coding skills by building realistic projects.
