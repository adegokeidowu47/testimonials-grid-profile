# Frontend Mentor - Four card feature section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The Grid challenge](#the-grid-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with HTML & CSS](#built-with-HTML-&-CSS)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Responsiveness is a crucial aspect of modern web design, ensuring that websites adjust freely to various screen sizes and devices. A well-optimized responsive layout not only enhances usability but also delivers a consistent and engaging user experience across smartphones, tablets, and desktops.

Working through this challenge significantly deepened my understanding of responsive design principles, especially the strategic application of CSS Grid for creating adaptable and structured layouts. I also gained insights into the importance of flexible units, media queries, and mobile-first design strategies.

This experience was both practical and rewarding, sharpening my ability to craft visually balanced, accessible, and user-friendly interfaces that perform effectively in today’s multi-device world.

### Screenshot
- Screenshot of large screen final design.

![](images/Screenshot%202025-07-23%20at%2009-23-07%20testimonials%20grid%20profile.png)

- Screenshot of mobile final design.

![](images/Screenshot%202025-07-23%20at%2009-23-59%20testimonials%20grid%20profile.png)




### Links

- Solution URL: (https://github.com/adegokeidowu47/testimonials-grid-profile)

- Live Site URL: (https://testimonials-grid-profile.vercel.app/)

## My process
- Mark up with HTML5, How the web will look like and its contents
- Styles with Cascading Style Sheets(CSS).

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned


```css
/* Using flex-box styling format for the mobile or for smaller screen. */

.body-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 2.5rem;
}
/* Grid styling format for the tap or for medium screen. */

@media screen and (min-width: 768px){

  .body-content {
          display: grid;
          grid-template-rows: .5fr .5fr;
          grid-template-columns: 1fr 1fr;
          grid-gap: 15px 25px;
      }
  
      section {
          align-self: stretch;
          justify-self: stretch;
      }
  
  
      section.daniel {
          grid-row: 1 / 2;
          grid-column: 1 / 2;
      }
  
      section.patrick {
          grid-row: 1 / 2;
          grid-column: 2 / 3;
      }
  
      section.kira {
          grid-row: 3 / 4;
          grid-column: 1 / 3;
      }
}

/* Grid styling format for the destop or for larger screen. */

@media screen and (min-width: 1200px) {
    .body-content {
        display: grid;
        grid-template-rows: 1fr 1fr;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-gap: 15px 25px;
    }

    section.daniel {
        grid-row: 1 / 2;
        grid-column: 1 / 3;
    }

    section.kira {
        grid-row: -3 / -1;
        grid-column: 4 / 5;
    }

    section.patrick {
        grid-row: 2 / 3;
        grid-column: -2 / -4;

    }

}
```


### Useful resources

- **[Resource 1](https://www.frontendMentor.com/learning-path)** - The article was incredibly helpful, especially the referenced tutorial materials, which provided deeper insight and clarity. I found the design pattern particularly effective and plan to adopt it in my future projects.

- **[Resource 2](Niederst Robbins, Jennifer - Learning Web Design _ A Beginner’s Guide to HTML, CSS, JavaScript, and Web Graphics-O’Reilly Media (2018))** - A Beginner’s Guide to HTML, CSS, JavaScript, and Web Graphics by O’Reilly Media (2018) is an excellent textbook that greatly enhanced my understanding of the CSS Grid property and its various values. I highly recommend it to anyone still learning or seeking to strengthen their grasp of this concept.

## Author
- Frontend Mentor - [Adegoke Idowu(Shaddy)](https://www.frontendmentor.io/profile/adegokeidowu47)
- Twitter - [@Adegokeidowu20](https://www.twitter.com/Adegokeidowu20)
