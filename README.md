> MalhoStephane_3_27032021
# Ohmyfood
> This is my second Openclassrooms course project.
> The project focuses in particular on the use of SASS and on CSS3 animations.

## REQUIREMENTS

Install Node.js v14.15.4. (or latest version)

## INSTALLATION

Clone the repository https://github.com/stephanemalho/MalhoStephane_3_27032021

Open your local folder in your code editor then, in a new terminal, run npm install

## USE

This project has 2 mode:

npm run serve
```
 -> For development mode. Once you run it, allows you to code in sass and see it in real time in your browser.
 ```

npm run start
```
 -> For production mode. Compile your sass into a minified css.
 ```
 

## General informations
Develop a site offering the menu of 4 major Parisian restaurants.
* The development must be done in CSS, without JavaScript.
* No framework should be used, however the use of SASS is recommended.
* No CSS code should be applied via a style attribute in an HTML tag.

## Screenshot
 ! [my menu page] (./assets/images/screen/menu.png)

## Prerequisites
* learn how to use SASS
* learn CSS3 animations

## Technologies
* HTML5
* CSS3
* SASS in SCSS format
* NPM

## Code examples
``` css
#entries {
  @include lazy (4.0);
}
# main-courses {
  @include lazy (3.0.6);
}
#desserts {
  @include lazy (3,1.2);
}
```
``` css
@mixin lazy ($ limit, $ delay) {
    @for $ i from 1 through $ limit {
        article: nth-of-type (# {$ i}) {
          animation: slide-top 1s ease-out ($ delay + (0.2s * $ i)) both;
        }
      }
}
// ANIMATION DELAY FOR LAZY LOADING //
```

## Characteristics

This site is a prototype created from a mobile model, the tablet and desktop format has been adapted by the developer. (Me ^^)

### Functionality
* a main page and four pages for restaurant menus
* structure of the mobile first site
* responsive format
* hover animation on menu items with check icon (hover)
* loading spinner on the main page
* the buttons change appearance on hover


## Status
The project is: finished
Although it is not functional, the deliverables have been respected,

## Inspiration
Course inspired project https://openclassrooms.com
additional source https://developer.mozilla.org/
validated https://validator.w3.org/