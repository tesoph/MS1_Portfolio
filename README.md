<div><img src="https://github.com/tesoph/MS1_Portfolio/blob/master/assets/img/logo/logo2.png?raw=true" alt="logo">
<h1>Art Portfolio</h1>
</div>


## Stream One Project: User-Centric Frontend Development - Code Institute

This is my portfolio website designed with the purpose of creating an online presence as an artist. The main feature of the portfolio is a gallery of my artwork displayed on index.html. The website also features an about page, a shop of merchandise, and a contact page with a form.

## Table of contents
* [Demo](#Demo)
* [UX](#UX)
* [Features](#Features)
* [Technologies Used](#technologies-used)
* [Testing](#testing)
* [Deployment](#deployment)
* [Credits](#credits)
  
## Demo
A live demo can be found [here](https://tesoph.github.io/MS1_Portfolio/).

![Desktop Demo](https://github.com/tesoph/MS1_Portfolio/blob/master/assets/img/index-html1.gif "Desktop Demo")

## UX

### User Stories

The following user stories were used to focus on the features the website should have:

* As a user, I want to be able to view a virtual gallery of the artist’s work.

* As a user, I want to be able to enlarge the images in the gallery so that I can see more detail of the art.

* As a user, I want to be able to contact the artist so I can ask about commissions, collaborations and/or general inquiries. 

* As a user, I want to be clearly presented with links to the artist’s social media accounts so I can keep up to date and/or interact with them across the web.

* As a user, I want to be able to buy merchandise or artwork so that I can support the artist’s work.

### Wireframes
[Index.html](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/index.jpg?raw=true)

[About.html](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/about.jpg?raw=true)

[Shop.html](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/shop.jpg?raw=true)

[Contact.html](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/contact.jpg?raw=true)

## Features

### Existing Features
* Header (every page)
  * The header on every page features a navigation bar to navigate through the website.
  * The navigation bar is responsive and is collapsed to a navbar toggler on devices below 768px width to contribute to a minimal look.
  * The header features a logo which is an anchor link to the home page.
  * The logo is unconventially placed in the navigation bar (above the navigation links) in order to create a  memorable design.

* Footer (every page)
  * Social media icons
  * Copyright info 

* [Gallery page](https://tesoph.github.io/MS1_Portfolio/index.html)
  * A gallery of thumbnail images which can individually be clicked to view a large version of the image in a full-screen fancybox window. Within the fancybox window the user can navigate through all the images in the gallery.
  * On mobile devices this gallery is horizontally scrolling. This design was chosen as side-scrolling is intuitive to mobile users. At the begining of the gallery the second image is partially shown to visually indicate the presence of horizontally scrolling content. At the end of the gallery there is blank space left to visually indicate the end of the gallery. 
  * On viewports wider than 576px the gallery displays as a grid of thumbnail images. This grid is 4 columns wide on large devices and up, 3 columns wide on medium devices, and 2 columns wide on small devices.
  * There is no h1 level heading on the index page to contribute to a minimal design.

* [About page](https://tesoph.github.io/MS1_Portfolio/about.html)
  *  Presents information about the artist's work and background.

* [Shop page](https://tesoph.github.io/MS1_Portfolio/shop.html)
  * Banner to advertise a sale.
  * Features products for sale with images and product information.
  * On the product information section of the tote bag product the color can be selected which will change the product image to match the selected color.

* [Contact page](https://tesoph.github.io/MS1_Portfolio/contact.html)
  * Contact Information: email, phone number and address are provided. This information is in a single column on mobile devices and in 3 columns wide on devices larger than mobile.
  * Contact Form: the contact form is responsively designed to provide a visually pleasing design on both mobile and larger devices. The required attribute is set on the input elements of the form so that a form may not be submitted without valid data being entered in the required fields. The image upload input does not have the required attribute. This form also features a Send Message button. If the Send Message button is clicked without the required fields being completed the form will not send and the user will be prompted to fill them in.
  

### Features Left to Implement
* Gallery filtering 
  * In the future, I would like to add a feature using Javascript to filter the images in the gallery according to the medium used to create the image. This would be used to distinguish between different categories of images e.g. drawings, paintings, images created with code, and sketchbook images.
* Dynamically updating year of copyright in the footer using Javascript.
* Interactive google map on the contact page with address of studio.


## Technologies Used
* Visual Studio Code
* HTML
* CSS
* Javascript
  * Used to change the product image src on the shop page.
* Bootstrap (v4.3.1)
* [Fancybox (v3.5.7)](http://fancybox.net/)
* [Google fonts](https://fonts.google.com/)
*  FontAwesome
*  jQuery
*  Popper.js
*  [Autoprefixer](https://autoprefixer.github.io/)


## Testing
<a href="http://jigsaw.w3.org/css-validator/check/referer">
        <img style="border:0;width:88px;height:31px"
            src="http://jigsaw.w3.org/css-validator/images/vcss"
            alt="Valid CSS!" /></a>

* The [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/) was used to validate the CSS.
* The [W3c Markup Validation Service](https://validator.w3.org) was used to validate each page of html.
* Chrome DevTools was used to test each page across all media query breakpoints to ensure the responsive design works as expected.

The website has been manually tested to ensure it passes the following test cases:

* Navigation bar (every page)
  * The logo in the navigation bar is an anchor link that directs to index.html. 
  * Each item in the navigation menu points to the correct destination.
  * The navbar is collapsed to a navbar-toggler below 576px in viewport width and expanded above 576px.
  * On hover of a nav menu item, an animation effect is applied to make the hovered link `font-weight:bold;` and increase the letter spacing.

* Footer (every page)
  * On hover the footer icons will change color to black.
  * All icons in the footer when clicked will open in a new tab using 'target="_blank"' and href="`https://www.google.com`".
     
* Index.html
  * On the desktop version of the website, when an image in the gallery is hovered over it is enlarged and a blur effect is applied to the image to visually indicate that you can click on it. 
  * Each image thumbnail points to the correct enlarged image.
  * The gallery responds correctly to all media query breakpoints and that there is no screen width at which the images do not fill the columns correctly.

* Shop.html
  * The banner is responsive.
  * Clicking the "Add to Cart" buttons in the product-info section applies a CSS click animation.
  * The color of the tote bag in the shop can be selected between black and white. Clicking either "white" or "black" in the product-info section changes the iamge to a product of that color.
  * On hover of the product images, the image is scaled to 1.05.

* Contact.html
  * The contact form will not submit without all fields with a "required" atrribute being completed with properly-formatted values. In the email-input field the input must match the standard format for Internet e-mail addresses. 
  * If the user clicks on the "Send Message" button without completing the required fields, they will be prompted to fill them in.
  * If the user clicks on the "Send Message" button with all fields correctly filled in, the page will be refreshed.
  * The displayed contact information is responsive and is a single column wide on XS devices and 3 columns wide on small devices and above.

### Bugs found in the testing phase
* During the testing phase it was noted that there was white space showing up on right-hand side of the browser. This was fixed following [this stackoverflow response](https://stackoverflow.com/questions/4617872/white-space-showing-up-on-right-side-of-page-when-background-image-should-extend/4617920) and applying the following rule:
```css
html,body{
    width: 100%;
    height: 100%;
    margin: 0px;
    padding: 0px;
    overflow-x: hidden; 
}
```
* During testing, it was noted that on 4K screens the page content did not have enough vertical height to place the footer to the bottom of the viewport. This was fixed with by wrapping all the page content except the footer in a div with the property `flex: 1;` and applying the following rule to the body:
 ```css
body{
   display:flex;
   flex-direction: column;     
   justify-content: space-between;
}
```


## Deployment
This site is hosted using GitHub pages, deployed directly from the master branch. The deployed site will update automatically upon new commits to the master branch. In order for the site to deploy correctly on GitHub pages, the landing page must be named `index.html`.

To run locally, you can clone this repository directly into the editor of your choice by pasting `git clone https://github.com/tesoph/MS1_Portfolio.git` into your terminal. To cut ties with this GitHub repository, type `git remote rm origin` into the terminal.


## Credits

### Content
The content for the about page is taken from the Lorem Ipsum text.

### Media
All images on the site are my own with the following exceptions:
1. The mockup image for the tote bag in the shop is taken from [Graphic Burger](https://graphicburger.com/canvas-tote-bag-mockup/).
2. The mockup image for the t-shirt in the shop is taken from [Freepik](https://www.freepik.com/free-psd/simple-black-men-s-tee-mockup_3384897.htm#page=1&query=t%20shirt%20mockup&position=0)

### Acknowledgements 
* The horizontal scrolling gallery was created following the article [How To Create Horizontal Scrolling Containers](https://codeburst.io/how-to-create-horizontal-scrolling-containers-d8069651e9c6).

* The shop page was created following the article [Designing A Product Page Layout with Flexbox](https://css-tricks.com/designing-a-product-page-layout-with-flexbox/).

* The blur effect on hovering over an image was modelled after the [Mono theme from Themeforest](http://mono.flatheme.net/Home/Portfolio-Minimal.html).

* The form on the contact page was modelled after the Code Institute lesson "Putting It All Together | Mini Project with Bootstrap 4".

* The design of the navbar was inspired by this [artist's website](https://www.reddwalitzki.com/).

* This README was created following the format of the [Code Institute example project](https://github.com/Code-Institute-Solutions/StudentExampleProjectGradeFive/blob/master/README.md) and has taken inspiration from Code Institute student [AJGreaves's README](https://github.com/AJGreaves/portrait-artist/blob/master/README.md).

* The footer was positioned using the flexbox method from [this article](https://medium.com/@kayodeniyi/understanding-the-sticky-footer-trick-1e5686c232b6).

* Thanks to my mentor Brian Macharia for support and advice.