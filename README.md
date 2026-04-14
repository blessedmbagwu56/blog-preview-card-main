# Frontend Mentor - Blog preview card solution

This is my solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page
- View the optimal layout for the interface depending on their device's screen size

### Links

- Solution URL: [GitHub repository](https://github.com/blessedmbagwu56/blog-preview-card-main)
- Live Site URL: [View live site](https://blessedmbagwu56.github.io/blog-preview-card-main/)

## My process

### Built with

- Semantic HTML5 markup (`<article>`, `<time>`)
- CSS custom HSL color values
- Flexbox for centering and layout
- Google Fonts (Figtree)
- Mobile-friendly responsive design
- CSS pseudo-classes (`:hover`, `:focus`, `:active`)

### What I learned

This was one of my first real projects, and I learned a lot about writing clean, semantic HTML and CSS.

**Centering with Flexbox** — I used to try centering things with random margins. Flexbox changed that:

```css
body {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
```

**Semantic time element** — I learned that using `<time>` with a `datetime` attribute helps screen readers and search engines understand the content:

```html
<time datetime="2023-12-21">Published 21 Dec 2023</time>
```

**Accessible interactive states** — wrapping the title in an `<a>` tag makes it properly focusable for keyboard users, and I combined the selectors to keep the CSS clean:

```css
a:hover,
a:focus,
a:active {
  color: hsl(47, 88%, 63%);
  cursor: pointer;
}
```

**Fluid images** — using `width: 100%` on the main image instead of a fixed pixel value made the card scale nicely on mobile.

### Continued development

Things I want to keep improving:

- Getting more comfortable with responsive design on different screen sizes
- Learning more about accessibility (ARIA, focus management)
- Starting to learn JavaScript to add real interactivity
- Using CSS custom properties (variables) to keep my styles DRY

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/) - My go-to for understanding any HTML or CSS property.
- [CSS-Tricks Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Helped me finally understand `justify-content` vs `align-items`.
- [Frontend Mentor Community](https://www.frontendmentor.io/community) - For encouragement and seeing how others approached the same challenge.

### AI Collaboration

I used **Claude** (Anthropic's AI assistant) as a learning partner during this project.

- **How I used it:** I asked it questions when I was stuck (like why my shadow wasn't showing, or why my border-radius only rounded one corner). It guided me with hints and explanations instead of just giving me the code.
- **What worked well:** It explained the *why* behind concepts — like why `padding` on an image pushed the image content inside the box and made the rounded corners invisible. That "aha" moments helped me understand, not just copy.
- **What didn't:** Sometimes I needed to push back when the answers were too long. Shorter, step-by-step hints worked better for me.

## Author

- GitHub - [@blessedmbagwu56](https://github.com/blessedmbagwu56)
- Frontend Mentor - [@blessedmbagwu56](https://www.frontendmentor.io/profile/blessedmbagwu56)
