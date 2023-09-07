# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

social-proof-section-master\Screenshot Social Proof Section.png

### Links

- Solution URL: (https://www.frontendmentor.io/solutions/responsive-layout-using-css-grid-and-flexbox-rCzmvhcvAc)
- Live Site URL: (https://alexayiecho.github.io/social-proof-section-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

During the project I learnt:
(1). How to add multiple background images and how to position them

```css
body {
  background: url(images/bg-pattern-top-desktop.svg) no-repeat top left, url(images/bg-pattern-bottom-desktop.svg)
      no-repeat bottom right;
}
```

(2). I ended up using display flex for max-width 800px for the header, .star-rating and reviews.

```css
@media (max-width: 800px) {
  header {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .star-rating {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .reviews {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}
```

### Continued development

(1). I need to have a better understanding of the width & max-width CSS properties. Though these are simple basic CSS properties, making alterations in the widths in the project was affecting the overall look and responsiveness of the page. I need to know what will happen to the design if the width property is altered.

(2). I was having a difficult time trying to align the H1, as can be seen with the placement of the
word 'products' for screen sizes below 800px. There is a difference in the position of the word 'products' in my final design compared to the problem design.

(3). For the background image, I had tried using the CSS property 'background-image' , but because of the two different images required for the background, the final design didn't have the images. I learnt that using the 'background' property was the best in making the final design to have both the top and bottom background images.

```css
body {
  background: url(images/bg-pattern-top-desktop.svg) no-repeat top left, url(images/bg-pattern-bottom-desktop.svg)
      no-repeat bottom right;
}
```

(4). The column gap is too big but it pushes the ratings so that they align vertically with the 3rd review(Alice)

```css
header {
  column-gap: 350px;
}
```

(5). I also need to learn more about media queries and responsive web-design

(6). I am proud that I was able to solve most part of the project on my own, considering this is the second problem from frontendmentor that I am attempting. The project helped me practice CSS grid and CSS positioning.

### Useful resources

- SuperSimple Dev (https://www.youtube.com/watch?v=G3e-cpL7ofc&t=1s)- The HTML & CSS reference available on the channel was valuable.

## Author

- Alex Ayiecho (https://www.github.com/AlexAyiecho)
- Frontend Mentor - [@AlexAyiecho](https://www.frontendmentor.io/profile/AlexAyiecho)
- Twitter - [@AlexAyiecho](https://www.twitter.com/AlexAyiecho)

## Acknowledgments

I'd like to thank AuddityCodes (https://www.youtube.com/watch?v=fcVglSYTymM). Through the youtube channel I gained some insight and was able to solve the background image issue I was having.
I'd also like to than SuperSimple Dev (https://www.youtube.com/watch?v=G3e-cpL7ofc&t=1s), where I learnt CSS positioning, and Traversy Media (https://www.youtube.com/watch?v=0xMQfnTU6oo), where I learnt CSS grid.
