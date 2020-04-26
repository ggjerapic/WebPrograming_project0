# Project 0
Web Programming with Python and JavaScript

# Author
Gordan Gjerapic, e-mail: ggjerapic@gmail.com
# Overview
This project contains the framework for a personal 
website created as a requirement for EdX - Project0. 
#Table of contents

# GIT Repository
    
# Project0 Requirements
##Four different `.html` pages
The website consists of the following four .html pages

    - index.html (landing page)
    - short_bio.html
    - education.html
    - skills.html

## List, table and image
Every `.html` includes an unordered list as a part of the Bootstrap's  
`navbar` component. On the landing page `index.html`, `short_bio.html` and `education.html`, the `navbar` component (an unordered list)
is followed by a table that includes an image (author's photo).
Other lists and tables are included as a part of the content.

##Stylesheet files
The website utilizes a conventional stylesheet `.css` file `project0_style.css`
as well as the stylesheet file created via SASS `project0_SASS_style.scss`.

##Stylesheet properties and selectors
###Properties
Some of the CSS properties and the accompanying attributes used for the website creation include
-  `font-size: large`
-  `font-weight: bold`
-  `text-decoration: none`
-  `color: black`
-  `width: 120px`
-  `border-collapse: separate`
-   `border-collapse: collapse`
-  `background-color: lightblue`
-  `background-image: url(project0/asfalt-dark.png)`
### Selectors
The following CSS selector types were used:
- \#  - id 
- .   - class
- ::  - pseudo class 
- a[href] - attribute
- th - tag

##Using mobile responsive @media query
Mobile responsive `@media` queries were used to suppress the display 
of the last row in the `education.html` table for widths smaller than 750 pixels.
Also, '@media' query was used to change the display settings `font-size` and `color` 
in `skills.html`.

##Bootstrap 4
A simple bootstrap component `navbar` was used to create all `.html` pages.
The bootstrap grid model was used more extensively on `skills.html` page.
The entire `skills.html` page is implemented as a bootstrap `container`.
The page elements are placed within the bootstrap grid using `row` and `column` 
 classes.
 
 ##SCSS variable, nesting and inheritance
 The examples of SCSS variable definition, nesting and inheritance are included in 
 `project0_SASS_style.scss` stylesheet.  The defined styles were used to control the content on the `skills.html` page.
 
 ### Variable definition
        $text_size_large: 18px;
        $text_size_small: 12px;
 ### Nesting example
     /* SCSS nesting                     */
     div {
       font-family: "Times New Roman", "sans-serif";
        ol, ul {
          font-family: "Arial", "sans-serif";
          color: gray;
        }
      }
 ###Inheritance
     /* inheritance */
    %format_baseline {
        font-family: sans-serif;
        color: black;
        border: 1px solid black;
        padding: 10px;
        margin: 30px;
    }
    .format_grid_th{
      @extend %format_baseline;
      font-size: $text_size_large;
      font-weight: bold;
      background-color: lightgray;
    }
    