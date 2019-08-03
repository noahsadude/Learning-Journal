## CSS (Cascading Style Sheets)

### Heirarchy of CSS
-Inline - <p style= "color:blue;">. Boo! Makes things difficult to troubleshoot.
-In Page - Between the <head> and </head> tags. Very hacky. Do not recommend.
-Last external stylesheet loaded between <head> and </head>
-All other external stylesheets

### Selectors
-Universal selector `*{}` targets literally everything.
-Type selectors. Match element names - h1 {} 
-Class selectors. Match an element whose class matches the selector - .hero {}
--Note, you can select both type and class via [type].[class]. p.hero {} targets only <p> elements whose class is hero.
-ID selectors. Match an element whose ID matches the value. #introduction {}
-Child selectors. Match elements that are children of elements. li>a {}
-Descendant selectors.

`margin: auto` is shorthand for `margin: 0 auto`

### Animations
-That's a thing in CSS3!

### General notes
-CSS code should be written from bottom left to top right.