# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS).  

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
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![blog preview solution](./screenshot-blogpreview.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process
This project was built using a **mobile-first workflow**, starting from a small screen layout and progressively enhancing it for larger screens using media queries.

I focused on matching the design as closely as possible, paying attention to spacing, typography, alignment, and hover effects.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Google fonts (figtree)
- Media quries for responsive design

### What I learned

This project helped me understand several important frontend concepts:

1. Mobile-first workflow
Instead of designing for desktop first, I learned to:
- Start with mobile styles as default
- Use `@media (min-width: ...)` to scale up for desktop

Example:

.description{
    font-size: 14px;
}

@media (min-width: 768px){
    .description{
        font-size: 16px;
    }
}

2. Flexbox alignment issues

I learned that misalignment often comes from default browser styles like paragraph margins.

Fix:

.author{
    display: flex;
    align-items: center;
    gap: 12px;
}

.author img{
    margin: 0;
}

3. Removing unwanted spacing

Extra space below elements was caused by:

default body margin
inline image baseline behavior

Fix:

body{
    margin: 0;
}

.card-image{
    display: block;
}

4. Hover states

I implemented interactive feedback on the title:

h1:hover{
    color: hsl(47, 88%, 63%);
    cursor: pointer;
}

5. Typography with Google Fonts

I used the Figtree font and learned how font weights and HSL colors affect visual hierarchy.

font-family: "Figtree", sans-serif;
color: hsl(0, 0%, 7%);

6. Semantic HTML improvement

I replaced unnecessary elements with better semantic choices:

<span> for tag labels instead of <button>
<main> for main card content instead of generic <div>

### Continued development

In future projects, I want to improve:
- Better responsive scaling (not just font size, but spacing and layout)
- Cleaner CSS organization (utility classes or structure systems)
- More consistent use of semantic HTML
- Faster debugging of layout issues like alignment and spacing

### Useful resources

- (https://fonts.google.com/) - For integrating Figtree font.
- (https://developer.mozilla.org/) - This is an amazing article which helped me to better understand CSS properties like flexbox, hover, and line-height. I'd recommend it to anyone still learning this concept.

### AI Collaboration

I used AI assistance (ChatGPT) during this project for:
- Debugging layout issues (flexbox alignment, spacing, and overflow problems)
- Understanding mobile-first workflow structure better
- Fixing CSS bugs like missing borders and font sizing issues
- Improving and understanding semantic HTML choices (span vs p, main usage)
- Learning best practices for responsive design

#### What worked well:

- Fast debugging of layout issues
- Clear explanations of CSS behavior
- Step-by-step guidance for structuring the project

#### What didn’t:

- Over-reliance initially instead of testing solutions myself first

Overall, AI helped speed up my learning process while still allowing hands-on practice.

## Author
- LinkedIn - [Ayinde Rukayat](www.linkedin.com/in/ayinde-rukayat-220b3130b)
- Frontend Mentor - [@rukkah](https://www.frontendmentor.io/profile/rukkah)
- GitHub - [@rukkah](https://github.com/rukkah)

## Acknowledgments

Thanks to the Frontend Mentor platform for providing realistic UI challenges and helping me improve my frontend development skills through practice.
