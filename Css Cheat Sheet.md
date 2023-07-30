# Css Cheat Sheet

```css

 /* Selectors */

/* Universal Selector */
* {
  property: value;
}

/* Element Selector */
element {
  property: value;
}

/* Class Selector */
.class {
  property: value;
}

/* ID Selector */
#id {
  property: value;
}

/* Grouping Selector */
selector1, selector2 {
  property: value;
}

/* Descendant Selector */
parent element {
  property: value;
}

/* Child Selector */
parent > element {
  property: value;
}

/* Attribute Selector */
element[attr="value"] {
  property: value;
}


/* Colors and Backgrounds */

/* Color */
color: value;               /* For text color */
background-color: value;    /* For background color */

/* Opacity */
opacity: value;             /* Range: 0 to 1 */

/* Background Image */
background-image: url('image.jpg');

/* Background Repeat */
background-repeat: repeat | repeat-x | repeat-y | no-repeat;

/* Background Attachment */
background-attachment: scroll | fixed | local;

/* Background Position */
background-position: x y;

/* Background Size */
background-size: auto | cover | contain;


/* Box Model */

/* Width and Height */
width: value;               /* E.g., 100px, 50%, auto */
height: value;              /* E.g., 100px, 50%, auto */

/* Margin */
margin: top right bottom left;

/* Padding */
padding: top right bottom left;

/* Border */
border: width style color;

/* Border Radius */
border-radius: value;       /* E.g., 5px, 50% */

/* Box Shadow */
box-shadow: h-offset v-offset blur spread color;


/* Text Styling */

/* Font Family */
font-family: Arial, sans-serif;

/* Font Size */
font-size: value;           /* E.g., 16px, 1rem, 1em */

/* Font Weight */
font-weight: normal | bold | bolder | lighter | number;

/* Text Align */
text-align: left | right | center | justify;

/* Text Decoration */
text-decoration: none | underline | overline | line-through;

/* Text Transform */
text-transform: capitalize | uppercase | lowercase | none;

/* Line Height */
line-height: value;         /* E.g., 1.5, 24px, 150% */


/* Display and Positioning */

/* Display */
display: block | inline | inline-block | flex | grid | none;

/* Position */
position: static | relative | absolute | fixed | sticky;

/* Top, Right, Bottom, Left */
top: value;
right: value;
bottom: value;
left: value;

/* Float */
float: left | right | none;

/* Clear */
clear: left | right | both | none;

/* Overflow */
overflow: visible | hidden | scroll | auto;


/* Flexbox */

/* Flex Container */
display: flex;
flex-direction: row | row-reverse | column | column-reverse;
flex-wrap: nowrap | wrap | wrap-reverse;
justify-content: flex-start | flex-end | center | space-between | space-around;
align-items: flex-start | flex-end | center | baseline | stretch;
align-content: flex-start | flex-end | center | space-between | space-around | stretch;

/* Flex Items */
order: value;
flex-grow: value;
flex-shrink: value;
flex-basis: value;
flex: grow shrink basis;
align-self: auto | flex-start | flex-end | center | baseline | stretch;


/* Grid Layout */

/* Grid Container */
display: grid;
grid-template-columns: value;
grid-template-rows: value;
grid-template-areas: area-name;
grid-template: "header header header" 1fr
               "sidebar main main" 2fr
               "footer footer footer" 1fr;
grid-column-gap: value;
grid-row-gap: value;
grid-gap: row-gap column-gap;

/* Grid Items */
grid-column-start: value;
grid-column-end: value;
grid-row-start: value;
grid-row-end: value;
grid-column: start / end;
grid-row: start / end;
grid-area: area-name;


/* Flexbox and Grid Shortcuts */

/* Flex Container Shortcut */
display: flex;
flex-flow: flex-direction flex-wrap;

/* Flex Items Shortcut */
flex: flex-grow flex-shrink flex-basis;


/* Box Sizing */
box-sizing: content-box | border-box;


/* Visibility */
visibility: visible | hidden;


/* Opacity */
opacity: value;             /* Range: 0 to 1 */


/* Z-index */
z-index: value;


/* Transition */
transition: property duration timing-function delay;


/* Animation */
animation-name: name;
animation-duration: value;
animation-timing-function: value;
animation-delay: value;
animation-iteration-count: value;
animation-direction: normal | reverse | alternate | alternate-reverse;
animation-fill-mode: none | forwards | backwards | both;
animation-play-state: running | paused;


/* Other */

/* Cursor */
cursor: pointer | auto | crosshair | default | help | move | text | wait | ...;

/* Pointer Events */
pointer-events: none | auto;

/* User Select */
user-select: none | auto;

/* Box Decoration Break */
box-decoration-break: slice | clone;


/* @Media Query */
@media screen and (max-width: value) {
  /* CSS rules for specific screen size */
}

/* @Font Face */


@font-face {
  font-family: 'FontName';
  src: url('font.woff2') format('woff2'),
       url('font.woff') format('woff');
}

/* @Keyframes */
@keyframes animation-name {
  0% {
    property: value;
  }
  100% {
    property: value;
  }
}
```
## Reference (https://cssreference.io/)
