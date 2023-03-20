# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![mobile screenshot](./design/Screenshot%20from%202023-03-20%2015-31-48.png)
![desktop screenshot](./design/Screenshot%20from%202023-03-20%2015-20-47.png)

### Links

- Solution URL: https://github.com/lawrence-yoon/qr-code-component-challenge

## My process

Starting the design with mobile first in mind, I had set the mobile display with developer tools to the iPhone SE screen resolution (375px by 667px). This fit the mobile responsiveness criteria of the challenge for a width of 375px. Looking at the desired mobile and desktop designs, it looked as if the card element did not scale with the scaling from mobile to desktop, so I decided to go with a fixed pixel width for the card.

For the setup, since this was a basic html css site, I just added the styles.css into the root of the directory. I also added a css reset. This adds a sizable amount of lines in the css, but I find that doing so makes the styling process much easier.

I've decided to use flexbox column to center the card div in the body, as well as center the contents in the card div. That is pretty much the bulk of it. I did a few calculations for the widths and paddings for constant pixel widths, e.g. the qr code image width and height.

For the image itself, I had some experience working with images and knew that the border radius gets a little wonky if applied to an <img> html element, so I decided to use it with background image in a div.

For the rounded borders, I knew that the card and the qr-code image would have the same properties, but I wasn't exactly sure what pixel/rem size the border radius should have. Normally I would just cycle through the different tailwindcss classes, so I decided to check the tailwindcss documentation for the standard css code. border radius of 16 px (1rem) turned out to match the solution.

The font style and weights were given, as well as the font size for the p element. I had to eyeball the font size of the larger text, which wasn't too hard after having all the other padding and images down. It was a matter of putting the end result side by side with the working page.

I added some finishing touches with a drop shadow, and inserted my portfolio website link into the attribution, and that was it. Due to the flexbox centering and constant pixel sizes, I did not have to make any media breakouts for the desktop.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### Useful resources

- [CSS reset](https://andy-bell.co.uk/a-modern-css-reset/) - This was my source for the css reset.
- [CSS documentation](https://tailwindcss.com/) - I am a huge fan of tailwindcss, and the css styles documentation is incredibly useful.

## Author

- Website - [Lawrence Yoon](https://larr.dev)
- Frontend Mentor - [@lawrence-yoon](https://www.frontendmentor.io/profile/lawrence-yoon)
