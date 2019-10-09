# Rachel Mc Laughlin Art Portfolio
## Stream One Project: User-Centric Frontend Development - Code Institute

This is my portfolio website designed to create an online presence as an artist. The main feature of the portfolio is a gallery of my artwork displayed on index.html. The website also features an about page, a shop of merchandise, and a contact page with a form.


## Demo
A live demo can be found [here](https://tesoph.github.io/MS1_Portfolio/).


## UX

The following user stories were used to focus on the features the website should have:

* As a user, I want to be able to view a virtual gallery of the artist’s work.

* As a user, I want to be able to enlarge the images in the gallery so that I can see more detail of the art.

* As a user, I want to be able to contact the artist so I can ask about commissions, collaborations and/or general inquiries. 

* As a user, I want to be clearly presented with links to the artist’s social media accounts so I can keep up to date and/or interact with them across the web.

* As a user, I want to be able to buy merchandise or artwork so that I can support the artist’s work.

### Wireframes
![gallery page wireframe](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/index.jpg?raw=true)

![about page wireframe](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/about.jpg?raw=true)

![shop page wireframe](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/shop.jpg?raw=true)

![contact page wireframe](https://github.com/tesoph/MS1_Portfolio/blob/master/wireframes/contact.jpg?raw=true)

## Features

### Existing Features
* Header (every page)
  * The header on every page features a navigation bar to navigate through the website.
  * The navigation bar is collapsed on mobile devices to contribute to a minimal look.
  * The header features a logo which is an anchor link to the home page.

* Footer (every page)
  * Social media icons
  * Copyright info 

* [Gallery page](https://tesoph.github.io/MS1_Portfolio/index.html)
  * A gallery of thumbnail images which can individually be clicked to view a full-screen-sized image. On mobile devices this gallery is horizontally scrolling. This design was chosen as side-scrolling is intuitive to mobile users. At the end of the gallery there is blank space left to visually indicate the end of the gallery. On viewports wider than 576px the gallery displays as a grid of images. 

* [About page](https://tesoph.github.io/MS1_Portfolio/about.html)
  *  Presents information about the artist's work and background

* [Shop page](https://tesoph.github.io/MS1_Portfolio/shop.html)
  * Features products for sale with images and product information. 

* [Contact page](https://tesoph.github.io/MS1_Portfolio/contact.html)
  * Features a contact form
  * Features contact information

### Features Left to Implement
* Gallery filtering 
  * In the future, I would like to add a feature using Javascript to filter the images in the gallery according to the medium used to create the image to distinguish between different categories of images e.g. drawings, paintings, images created with code, and sketchbook images.


## Technologies Used
* Visual Studio Code
* HTML
* CSS
* Javascript
  * Used to change the image src in shop.html
* Bootstrap (v4.3.1)
* [Fancybox (v3.5.7)](http://fancybox.net/)
* [Google fonts](https://fonts.google.com/)
*  FontAwesome
*  jQuery
*  Popper.js
*  [Autoprefixer](https://autoprefixer.github.io/)


## Testing

### Index.html
On the desktop version of the website, when an image in the gallery is hovered over it is enlarged and a blur effect is applied to the image to visually indicate that you can click on it. Clicking on an image is an intuitive action for a mobile user and there is not a :hover function on touchscreen devices, but when clicked the effect is applied.

There is no header on the index page to contribute to a minimal design.

### Shop.html
The "Add to Cart" buttons in the product-info section, only changes the css style on the button and does not complete any add to cart action.

The color of the tote bag in the shop can be selected between black and white, using javascript to change the img src on click.

### Contact.html
The contact page features a form with the method = "post" (sends the form-data as HTTP post transaction). The required attribute is set on the input elements of the form so that a form may not be submitted without valid data being entered in the required fields. The image upload input does not have the required attribute.

### Navbar
The logo in the navbar is an anchor link which directs to index.html

### Footer
All icons in the footer when clicked will open in a new tab using 'target="_blank"' and href="`https://www.google.com`". All links have been manually tested to ensure that they are pointing to the correct destination.

### Body
During the testing phase I noticed that there was white space showing up on right-hand side of the browser. This was fixed following [this stackoverflow response](https://stackoverflow.com/questions/4617872/white-space-showing-up-on-right-side-of-page-when-background-image-should-extend/4617920) to insert the following code:
```css
html,body
{
    width: 100%;
    height: 100%;
    margin: 0px;
    padding: 0px;
    overflow-x: hidden; 
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
The horizontal scrolling gallery was created following this tutorial [here](https://codeburst.io/how-to-create-horizontal-scrolling-containers-d8069651e9c6).

The shop page was created following this tutorial [here](https://css-tricks.com/designing-a-product-page-layout-with-flexbox/).

The blur effect on hovering over an image was modelled after the following theme [here](http://mono.flatheme.net/Home/Portfolio-Minimal.html).

The form on the contact page was modelled after the Code Institute lesson "Putting It All Together | Mini Project with Bootstrap 4".

The design of the navbar was inspired by the following artist's website [here](https://www.reddwalitzki.com/).

This readme was created following the format of the Code Institute example project found [here](https://github.com/Code-Institute-Solutions/StudentExampleProjectGradeFive/blob/master/README.md).
