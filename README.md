# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0).

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

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](images/ScreenshotHuddle.png)

### Links

- Solution URL: [FrontendMentor.io](https://www.frontendmentor.io/solutions/huddle-landing-page-w-single-intro-section-with-html-taiwindcss-7ONnymWuw)
- Live Site URL: [Vercel](https://prj-13-huddle-landing-page-with-single-introductory-section.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- CSS Grid
- Mobile-first workflow
- [Vitejs](https://vitejs.dev/) - Frontend Development Framework
- [Tailwindcss](https://tailwindcss.com) - A utility-first CSS framework

### What I learned

Using FontAwesome icons loading them directly from internet: The kit must be generated from your account

```html
<script
  src="https://kit.fontawesome.com/1234567890.js"
  crossorigin="anonymous"
></script>
<footer
  class="mt-16 mb-8 flex justify-center items-center xl:justify-end xl:mt-1"
>
  <div class="social-icon">
    <i class="fab fa-facebook-f"></i>
  </div>
  <div class="social-icon">
    <i class="fab fa-twitter"></i>
  </div>
  <div class="social-icon">
    <i class="fab fa-instagram"></i>
  </div>
</footer>
```

Using Tailwindcss @apply

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer components {
  .social-icon {
    @apply mx-1 w-8 h-8 border-[1px] border-white rounded-full text-white flex justify-center items-center hover:text-softMagenta hover:border-softMagenta hover:cursor-pointer;
  }
}
```

Using multiple background images in Tailwindcss

```js
module.exports = {
  content: ["./index.html", "./src/**/*.{vue,js,ts,jsx,tsx}"],
  theme: {
    extend: {
      fontFamily: {
        openSans: ["Open Sans", "sans-serif"],
        poppins: ["Poppins", "sans-serif"],
      },
      colors: {
        violet: "hsl(257, 40%, 49%)",
        softMagenta: "hsl(300, 69%, 71%)",
      },
      backgroundImage: {
        mobile: "url('/images/bg-mobile.svg')",
        desktop: "url('/images/bg-desktop.svg')",
      },
    },
  },
  plugins: [],
};
```

Using Tailwindcss flex basis to adjust 2 items to half of width

```html
<div
  class="xl:flex xl:flex-nowrap xl:justify-center xl:items-center xl:space-x-12"
>
  <div class="xl:basis-1/2">
    <img src="/images/illustration-mockups.svg" class="my-16" alt="" />
  </div>
  <div class="xl:basis-1/2">
    <h1>Build The Community <br />Your Fans Will Love</h1>
    <p>
      Huddle re-imagines the way we build communities. You have a voice, but so
      does your audience. Create connections with your users as you engage in
      genuine discussion.
    </p>
    <button>Register</button>
  </div>
</div>
```

### Continued development

Future projects will be developed using Vue.JS when interactivity must be included.

### Useful resources

- [TailwindCSS Directives](https://tailwindcss.com/docs/functions-and-directives) - Use of @apply directive
- [Customizing Colors in TailwindCSS](https://tailwindcss.com/docs/customizing-colors) - Adding personalized color names to be used in tailwindcss.
- [Customizing Fonts in TailwindCSS](https://tailwindcss.com/docs/font-family#using-custom-values) - Adding Google fonts to be used in tailwindcss.

## Author

- Website - [Gustavo Sanchez](https://www.gusanche.dev)
- Frontend Mentor - [@gusanchedev](https://www.frontendmentor.io/profile/gusanchedev)
- Github - [@gusanchedev](https://www.github.com/gusanchedev)
- Twitter - [@gusanchedev](https://www.twitter.com/gusanchedev)
- Linkedin - [gusanchedev](https://www.linkedin.com/in/gusanchedev/)

## Acknowledgments

Thanks to Mariapaz for being my friend and support 💙
