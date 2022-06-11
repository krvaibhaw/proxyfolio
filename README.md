# Proxyfolio | Minimalist Template ⚡️

[![GitHub](https://img.shields.io/github/license/krvaibhaw/proxyfolio?color=blue)](https://github.com/krvaibhaw/proxyfolio/blob/master/LICENSE.md) 
![GitHub stars](https://img.shields.io/github/stars/krvaibhaw/proxyfolio)
![GitHub forks](https://img.shields.io/github/forks/krvaibhaw/proxyfolio)
![](https://img.shields.io/badge/Excitement-High-red)
![](https://img.shields.io/badge/Pull_Requests-Accepting-yellow)

## A minimal, blazing fast portfolio template for Developers! 🚀

<p align="center">
<img src="video/demo.gif" >
</p>

## Features

- **Easy to Setup 💯** 
- **Modern UI Design + Reveal Animations 🍇**
- **OpenSource 📙** 
- **No Additional Frameworks 🤘🏻** 
- **No Additional Libraries 🔗** 
- **Multi Page 💎** 
- **Fully Responsive 🚀** 
- **Super Fast and Optimized for SEO ⚡** 
- **Valid HTML5 & CSS3 🎖️** 


## Why do you need a portfolio? 👇🏻

- A method of self discovery and confidence building
- Professional way to showcase your work
- Increases your visibility and online presence
- Shows you’re more than just a resume

## Getting started 🔧

From your command line, first clone Simplefolio:

```bash
# Clone the repository
$ git clone https://github.com/krvaibhaw/proxyfolio.git

# Move into the repository
$ cd proxyfolio

# Remove the current origin repository
$ git remote remove origin

# Open the index.html file
$ firefox index.html
```

## Template Instructions 🔭

### Step 1 - Structure

Go to `/index.html` and put your information, there are 5 sections:

1. Header Section

    - On `img/stuffs.jpg`, Add your own Image, Better if the background of the image is transparent so the background can match the theme color.
    - Add your own name and custom portfolio title.
    - On `<h4>` tag mention your Career Statement/Summary.

```html
<div class="header__title">
    <!-- <h1 onclick="alert('HTML alert')"> -->
    <h1>
      Hey, my name is
      <!-- Green highlight effect -->

      <!-- Your Name Here -->
      <span class="highlight">Proxy</span>
      <br>I'm a
      <span class="highlight">Web</span>
      Developer
    </h1>

    <!-- Your Career Statement/Summary  -->
    <h4>Lorem ipsum dolor sit amet consectetur adipisicing elit.</h4>
    <button class="btn--text btn--scroll-to">Learn more &DownArrow;</button>
    <img src="img/stuffs.jpg" class="header__img" alt="Minimalist items" />
</div>

```

2. About Section

    - On `<span>` tag under `class="operations"` mention your skills.
    - On `<h5 class="operations__header">` mention your skill title.
    - On `<p>` tag which is below ` <h5 class="operations__header">` tag, put a short description about your skill, I recommend to put 1 to 2 line of short and crisp details about your skills.
    - Copy `class="operations__content operations__content--n` with n being the `nth` skill, you can also add more skills to your liking.


```html
<section class="section" id="section--1">
    <div class="section__title">
      <h2 class="section__description">About Me</h2>
      <h3 class="section__header">
        This is where you can describe Yourself.
      </h3>
    </div>

    <div class="operations">
      <div class="operations__tab-container">
        <button class="btn operations__tab operations__tab--1 operations__tab--active" data-tab="1">
          <span>01</span>Skill 1
        </button>
        
            ...

        <button class="btn operations__tab operations__tab--3" data-tab="3">
          <span>n</span>Skill n
        </button>
      </div>
    
      <div class="operations__content operations__content--1 operations__content--active">
        <div class="operations__icon operations__icon--1">
            <svg><use xlink:href="img/icons.svg#icon-upload"></use></svg>
        </div>
        <h5 class="operations__header">
            
            <!-- Skill Title  -->
        </h5>
        <p>
            <!-- Skill Summary  -->
        </p>
      </div>

         ...

      <!-- Add more skills accordingly as above  -->

    </div>

</section>
```

3. Projects Section

    - On `<img>` tag with class name `class="features__img lazy-img"` add your project image.
    - On `<h5>` tag with class name `class="features__header"`, include your project title.
    - On `<p>` tag below `<h5>` tag, include your project description.
    - Replicate `<div> ... </div>` with class `class="features"` to add more projects.

```html
    <section class="section" id="section--2">
    <div class="section__title">
      <h2 class="section__description">Projects</h2>
      <h3 class="section__header">
        Talk about your projects and Open Source contributions.
      </h3>
    </div>

    <div class="features">

      <!-- Project featured image  -->
      <img src="img/digital-lazy.jpg" data-src="img/digital.jpg" alt="Computer"
      class="features__img lazy-img" />
      <div class="features__feature">
        <div class="features__icon">
          <svg><use xlink:href="img/icons.svg#icon-monitor"></use></svg>
        </div>

        <!-- Project Title  -->
        <h5 class="features__header">Project 1</h5>
        <p>
            <!-- Project Descriptions and links  -->
        </p>
      </div>

      <!-- Add more projects accordingly as above  -->
      
    </div>
</section>
```

4. Publication Section

    - On `<h5>` tag with class name `class="testimonial__header"`, include your publications title.
    - On `<blockquote>` tag with class name `class="testimonial__text"`, include your publications description.
    - On `<h6>` tag with class name `class="testimonial__name"`, include your username for the publishing site.
    - On `<p>` tag with class `class="testimonial__location"`, to  include publisher name.
    - Replicate `<div> ... </div>` with class `class="slide"` to add more publications.

```html
  <section class="section" id="section--3">
    <div class="section__title section__title--testimonials">
      <h2 class="section__description">Publications</h2>
      <h3 class="section__header">
        Talk about your Publications here.
      </h3>
    </div>

    <div class="slider">
      <div class="slide">
        <div class="testimonial">

          <!-- Publication Title  -->
          <h5 class="testimonial__header">Publication Title 1</h5>
          <blockquote class="testimonial__text">
              
              <!-- Publication Descriptions and links  -->
          </blockquote>
          <address class="testimonial__author">
            <img src="img/user-1.jpg" alt="" class="testimonial__photo" />

            <h6 class="testimonial__name">Proxy</h6>          <!-- Your Name  -->
            <p class="testimonial__location">On Medium</p>    <!-- Publisher Name  -->
          </address>
        </div>
      </div>

      <!-- Add more publications accordingly as above  -->

      <button class="slider__btn slider__btn--left">&larr;</button>
      <button class="slider__btn slider__btn--right">&rarr;</button>
      <div class="dots"></div>
    </div>
</section>
```

5. Contact Section

    - On `<h3>` tag with class name `class="section__header"`, include some custom call-to-action message.

```html
<section class="section section--sign-up">
    <div class="section__title">
      <h3 class="section__header">
        <!-- Mention different ways to contact you -->
      </h3>
    </div>
    <button class="btn btn--show-modal">Contact Me</button>
</section>
```

6. Footer Section 

    - Can add link to your blogs and other sites using `<a>` tag with class `class="footer__link"`.
    - Here you can also put your Social Media URL using `href` attribute of the `<a>` tags.

```html
<footer class="footer">
    <ul class="footer__nav">
      <li class="footer__item">
        <a class="footer__link" href="#section--1">About</a>
      </li>
      <li class="footer__item">
        <a class="footer__link" href="#section--2">Projects</a>
      </li>
      <li class="footer__item">
        <a class="footer__link" href="#section--3">Publications</a>
      </li>

        ...
      
</footer>
```

7. Contact Page

    - This is a custom contact me page.
    - Mention your custom message in `<h2>` with `class="modal__header"`.


```html
<div class="modal hidden">
    <button class="btn--close-modal">&times;</button>
    <h2 class="modal__header">
      Will reply within <br />                      <!-- Your message -->
      <span class="highlight">a day</span>
    </h2>
    <form class="modal__form">
      <label>First Name</label>
      <input type="text" />
      <label>Last Name</label>
      <input type="text" />
      <label>Email Address</label>
      <input type="email" />
      <button class="btn">Next step &rarr;</button>
    </form>
  </div>
  <div class="overlay hidden"></div>
```

### Step 2 - Styles

Go to `css/style.css` and tweaks value to change tp different colors and see which color suits you the most.
If you want to get some gradients inspiration I highly recommend you to check this website [UI Gradient](https://uigradients.com/#BrightVault).

```scss
// Default values
background-color: #f3f3f3;
color-primary: #5ec576;
```

## Deployment 📦

Once you finish your setup. You need to put your website online!

I highly recommend to use [Netlify](https://netlify.com) because it is super easy.

## Technologies used 🛠️

- **HTML**
- **CSS**
- **JavaScript**

## License 📄

This project is licensed under the  GPL-3.0 License - see the [LICENSE](LICENSE) file for details

## Acknowledgments 🎁

This work is inspired by [Bankist](https://github.com/jonasschmedtmann/complete-javascript-course/tree/master/13-Advanced-DOM-Bankist) project from complete JavaScript course by Jonas Schmedtmann. <br>
Special thanks to Jacobo Martínez for creating [Simplefolio](https://github.com/cobidev/simplefolio) which is another great Portfolio website Template for Developers.
