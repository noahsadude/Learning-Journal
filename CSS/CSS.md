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

### The Box model
-A heirarchy of boxes
Margin
Border
Padding
Content

#### Box Dimensions
-Can be set by using height: and width: 
-For responsive designs, min-width: and max-width: breakpoints allow us to specify changes in design depending on screen width.
-Also, for height, min-height: and max-height: breakpoins make it possible to change design based on screen height.

### Borders
-You can control the top, bottom, right and left width of your border all independently.
-Your border style is much the same. Bottom, top, right and left are all independently controllable.
-Border color can also be independently controlled like the above.
-Width and style are our options here.
-Width can be either:
--thin
--medium
--thick
OR
pixels
-border style can be:
--solid
--dotted
--dashed
--groove
--ridge
--inset
--outset
--hidden/none
--Border color can be controlled using rgb, hex codes or css color names
Width, Height, style and color can be all controlled using a single line: eg. border: 3px dotted #0088dd;

#### Border-image
-super complicated
-requires: url of the image, where to slice the image, and the three values: stretch, repeat, round

#### Box shadow
-Lets you add a drop shadow. Neat right?
-Technically not in CSS3? use -moz-box-shadow and -webkit-box-shadow properties to make this happen.

#### Centering content
-Can be done by setting the left-margin and right-margin to auto

### Display:
-inline: makes an element an inline element
-block: makes an element a block level element
-inline-block: causes block level elements to flow like inline elements but retain some block features
-none: hides the element

###Visibiliy:
-hidden: hides the element
-visible: shows the element. simple enough





## Layout

### Positioning Schemes
Normal flow 
-Block level elements appear on a new line. Two elements will not sit side by side.
-`position: static`

Relative positioning
-Shifts an element from it's position in normal flow. Does not affect the position of surrounding elements.
-`position: absolute`

Absolute positioning 
- Positions the element in relation to it's containing element. Taken completely out of normal flow. 
-`position: relative`

Fixed positioning 
- A form of absolute positioning that positions the element in relation to the browser window.
-`position: fixed`

Floating elements 
- Takes the element out of normal flow, positions it to the far left or right of a box. Floated element becomes a block level element around with other content can flow.
-`float:`

#### CSS for a 3 column fixed-width layout with floats using individual classes for each column
body {
	width: 960px;
	font-family: Arial, Verdana, sans-serif;
	color: #665544;}
    	.column1of3, .column2of3, .column3of3 {
		width: 300px;
		float: left;
		margin: 10px;}
}

### Fixed width layouts vs "Liquid"/Responsive layouts
*Fixed width:*
Advantages:
-Lots more control
-Pixel values can be used to accurately define size/position
-Image size and line length are always the same.
Disadvantages
-Does not take into account big or small screen sizes, limiting user experience.
-Users who increase font size for readability might break the layout.

*Liquid/Responsive layout*
Advantages:
-Page can contract or expand according to device screen size.
-Tolerant of high font size.
-No overabundance of whitespace on either side of a page
Disadvantages:
-Users with very wide windows or very narrow ones can experience long text line lengths or very short ones, decreasing readability. Recommendation: min and max widths and break points
-Can result in unexpected layouts
-Can result in overflow errors

#### CSS for a responsive layout header, footer, and two row layout with row two divided into 3 columns.

* {
		font-family: Arial, Verdana, sans-serif;
		color: #665544;
		text-align: center;}
	body {
		width: 90%;
		margin: 0 auto;}
	#content {
		overflow: auto;}
	#nav, #feature, #footer {
		margin: 1%;}
	.column1, .column2, .column3 {
		width: 31.3%;
		float: left;
		margin: 1%;}
	.column3 {
		margin-right: 0%;}
	li {
		display: inline;
		padding: 0.5em;}
	#nav, #footer {
		background-color: #efefef;
		padding: 0.5em 0;}
	#feature, .article {
		height: 10em;
		margin-bottom: 1em;
		background-color: #efefef;}
}







### General notes
-CSS code should be written from bottom left to top right.