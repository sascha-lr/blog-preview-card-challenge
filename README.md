# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

Going into this challenge, I had much more knowledge than with the previous QR-Code component. I wanted to create something that was a little unique and not follow the guidelines 1:1. What I did was I made a dark-mode version that showcases just a tad bit more of my own personal style. I believe that I learned a lot of valuable lessons compared to the last challenge. Wrapping the content of the page inside `<main>` immediately, using units, such as `.rem`, by default instead of relying on `.px`. Creating classes and addressing `html`-elements in my `CSS` that way, thinking about the potential future of expanding the page, working like a real developer instead of addressing elements with just: `p {...}`. I also learned a lot when it comes to responsive design, centering elements in various ways, using flexbox, or grid when it's use-case was better suited. Using the `gap` CSS-property, instead of `margin`, when having a flexbox/grid layout. Using hover-effects for the first time, along with a nice animation, by utilizing `:hover` along with `transition`. Safe to  say, I learned a lot. I implemented a mobile-first approach, trying to implement responsibility, by also thinking about:"Ok, so when the screen is reaaally narrow, which, no one has a phone that narrow but whatever: The article-container becomes so narrow,  that content gets cut off, because it's correctly set to `overflow:hidden;`. How do I overcome  this? I found about about setting `overflow: hidden scroll;`. But that had a really ugly vertical scrollbar that I wanted to eliminate entirely. By googling and reading a post on [stackoverflow](https://stackoverflow.com), I removed the scroll-bar by setting `scrollbar-width: none;`. Also, I had a hard time centering all content on the page utilizing 

```css
body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
```
, because the margins I had set would just disappear when scaling to a narrow screen-size, which is why I utilized 

```css
body {
  height: 100vh;
  display: grid;
  place-content: center;
}
```
, instead.

All in all, I think it turned out great and I am proud of myself. I'm looking forward for what's to come! This is just the beginning!

![](/assets/images/screenshot.png)

### Links

- [Solution URL](https://github.com/sascha-lr/blog-preview-card-challenge)
- [Live Site URL](https://sascha-lr.github.io/blog-preview-card-challenge)

## My process

As previously stated, I utilized a mobile first-approach when going about this challenge. First, I added all elements needed in my `html`-code, after which I started designing them in CSS, while comparing the live results in my browser, with the screenshots provided on how the finished result should look. Fortunately, I didn't have a lot of problems or hiccups during this challenge, and when I did, as with the centering content problem I mentioned above, I researched and found a solution rather quickly.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### Continued development

In the future, I want my `html` to be more semantic, when and if possible. When doing this project, I was sometimes unsure of whether having used the correct elements for page content (which I still am now). However, that is something that, with research and practice, I will overcome. I want to improve pretty much everything and employ best-practices all around. So far, I have had, by my standards, great success. This journey is a marathon, not a sprint, however.

### Useful resources

- [Kevin Powell](https://github.com/kevin-powell) - While not working on this project, I watched some YouTube videos of content creator and CSS-master Kevin Powell. I really like his style of videos and teaching and in just one video I watched, I understood a variety of concepts easily, thanks to him. Currently, he is one of my favourite creators in this space.  Thank you Kevin!
- [The Odin Project](https://www.theodinproject.com) - While starting this challenge, I started TOP. An amazing course made by amazing people that I am sure will help me greatly on my journey to become a great Full-Stack Developer.
- [stackoverflow](https://stackoverflow.com) - For all questions programming.
- [prismic.io CSS Hover Effects Article](https://prismic.io/blog/css-hover-effects) - I read this specific article on prismic.io, when learning about hover-effects. This teached me a lot and I utilized pretty much the same code as they had for the 