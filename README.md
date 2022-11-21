# marcioneuro.com

This is a website for Dr. Marcio Schneider Medeiros. He is a neurologist based in Porto Alegre, RS, Brazil.

## Table of contents

-   [Overview](#overview)
-   [My process](#my-process)
    -   [Built with](#built-with)
    -   [What I learned](#what-i-learned)
    -   [Continued development](#continued-development)
    -   [Useful resources](#useful-resources)
-   [Author](#author)
-   [Acknowledgments](#acknowledgments)

## Overview

The goal of this website was to introduce Dr. Marcio and highlight his specialties in the field of neurology.
We wanted to give information about the Parkinsons and Alzheimers diseases, as well as how you can use botox injections to ease some symptoms.
We included links to his published papers, CV, his contact and address information of his clinic.

## My process

My process started by having conversations with Marcio about his specific needs for this website. We went over the type of content he would use,
the types of features he would like for his site (mobile responsive, google map etc) and if he had a presence on other social media sites (instagram, facebook etc).

I tried to build a logical layout for the information he wanted to provide, while maintaining a flow based on the content rendered.

The colour scheme was based on his instagram presence, we wanted to have a unified message throughout different applications.

There were many consultations where we would go over any changes or ideas that we thought would add to the site.

### Built with

-   Semantic HTML5 markup
-   CSS custom properties
-   Flexbox
-   Mobile-first workflow

### What I learned

One of the biggest lessons I learned through this process was the LARGE difference in skills between programmer and designer. I was lucky enough that Marcio already had a colour scheme with his other online presence.
The layout was largely inspired by other neurologists websites we had found, our focus was on keeping everything responsive.

During this project, I learned some neat CSS tricks for hover effects and navbars.
I think the most interesting one was making a navbar toggle without using any JavaScript:

HTML

```html
<input type="checkbox" id="nav-toggle" class="nav-toggle">
<nav id="nav-bar" class="nav-bar">
    <ul class="nav-section">
        <li><a href="#about">Sobre</</li>
        <li><a href="#especialidades" >Especialidades</a></li>
        <li><a href="#pesquisa">Pesquisa</a></li>
        <li><a href="#contact">Contato</a></li>
        <li><a href="#map">Endereço</a></li>
    </ul>
</nav>
<label for="nav-toggle" class="nav-toggle-label">
    <span></span>
</label>
```

CSS

```css
.nav-toggle {
	display: none;
}

.nav-toggle-label {
	position: absolute;
	top: 0;
	right: 0;
	height: 90%;
	display: flex;
	align-items: center;
	margin-right: 1rem;
}

.nav-toggle-label span,
.nav-toggle-label span::before,
.nav-toggle-label span::after {
	display: block;
	background: var(--secondary-clr);
	height: 3px;
	width: 2em;
	border-radius: 2px;
	position: relative;
}

.nav-toggle-label span::before,
.nav-toggle-label span::after {
	content: "";
	position: absolute;
}

.nav-toggle-label span::before {
	bottom: 8px;
}

.nav-toggle-label span::after {
	top: 8px;
}

.nav-toggle:checked ~ nav {
	transform: scale(1, 1);
}

.nav-toggle:checked ~ nav a {
	opacity: 1;
	transition: opacity 250ms ease-in-out 275ms;
}
```

### Continued development

This website is fairly static in nature, but it was extremely helpful in solidifying my understanding of the core concepts in HTML and CSS.
In the future I would like to expand the functionality of a website by writing it with more JavaScript and/or React.

I feel that by creating more interactive elements, I could potentially improve user experience/engagement.

I tried to keep accessibility in mind during this project and I plan to continue learning and improving my methods for keeping the internet open to everyone.

Website optimization was something I had to learn about during this project. I will continue to try and keep websites as efficient as I can, using the most current 'best practices' techniques.

### Useful resources

-   [Kevin Powell](https://www.youtube.com/@KevinPowell) - This man is an amazing resource for explaining some of the intricacies of frontend development. If you're having trouble getting your websites to render how you want, I highly recommend watching some of his videos.

-   [freeCodeCamp](https://www.freecodecamp.com) - This is another great resource from which I was able to learn most of the basics needed for this website.

-   [CS50](https://learning.edx.org/course/course-v1:HarvardX+CS50+X/home) - Harvard's CS50 program was where I first dipped my toes into the world of computer science. It's a very challenging, yet rewarding course that I recommend to anyone who is also starting the journey to become a software developer.

## Author

I'm at the beginning of my journey as a web developer, so any feedback is greatly appreciated. I'm open for any discussions or collaborations. [Simon Tsui](https://github.com/yubdis)

## Acknowledgments

I would like to give a shout out to [Ozzie Nehar](https://github.com/ozziexsh) and to [Carey Underwood](https://github.com/cwillu) for providing feedback on this project. Their knowledge was an enormous help for my first build of a functional/responsive website.
