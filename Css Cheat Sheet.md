# Css Cheat Sheet


This CSS Cheat Sheet provides a quick reference to commonly used CSS properties, selectors, and tips for styling web pages effectively. Below is a breakdown of the major sections and features covered in this cheat sheet:

## Selectors

- **Universal Selector (`*`)**: Targets all elements on the page.
- **Element Selector (`element`)**: Targets elements with a specific tag name (e.g., `div`, `p`, `a`).
- **Class Selector (`.class`)**: Targets elements with a specific class attribute (e.g., `.container`, `.btn`).
- **ID Selector (`#id`)**: Targets an element with a specific ID attribute (e.g., `#header`, `#nav`).
- **Grouping Selector (`selector1, selector2`)**: Targets multiple selectors at once.
- **Descendant Selector (`parent element`)**: Targets elements that are descendants of a specific parent element.
- **Child Selector (`parent > element`)**: Targets immediate child elements of a specific parent element.
- **Attribute Selector (`element[attr="value"]`)**: Targets elements with specific attribute-value combinations.




# CSS Cheat Sheet

## Selectors

### Universal Selector
```css
* {
  property: value;
}
```

### Element Selector
```css
element {
  property: value;
}
```

### Class Selector
```css
.class {
  property: value;
}
```

### ID Selector
```css
#id {
  property: value;
}
```

### Grouping Selector
```css
selector1, selector2 {
  property: value;
}
```

### Descendant Selector
```css
parent element {
  property: value;
}
```

### Child Selector
```css
parent > element {
  property: value;
}
```

### Attribute Selector
```css
element[attr="value"] {
  property: value;
}
```


## Colors and Backgrounds

- **Color**: Sets the text color using `color`.
- **Background Color**: Sets the background color using `background-color`.
- **Opacity**: Specifies the opacity of an element using `opacity` (range: 0 to 1).
- **Background Image**: Sets a background image using `background-image`.
- **Background Repeat**: Controls how the background image is repeated using `background-repeat`.
- **Background Attachment**: Specifies whether the background image scrolls with the content using `background-attachment`.
- **Background Position**: Sets the starting position of the background image using `background-position`.
- **Background Size**: Adjusts the size of the background image using `background-size`.

## Box Model

- **Width and Height**: Sets the width and height of elements using `width` and `height`.
- **Margin**: Sets the space outside an element's border using `margin`.
- **Padding**: Sets the space between an element's content and its border using `padding`.
- **Border**: Defines the border width, style, and color using `border`.
- **Border Radius**: Creates rounded corners for elements using `border-radius`.
- **Box Shadow**: Applies a shadow effect to elements using `box-shadow`.

## Text Styling

- **Font Family**: Specifies the font family for text using `font-family`.
- **Font Size**: Sets the font size using `font-size`.
- **Font Weight**: Defines the thickness of characters using `font-weight`.
- **Text Align**: Aligns text within its container using `text-align`.
- **Text Decoration**: Adds decoration to text, such as underline or line-through, using `text-decoration`.
- **Text Transform**: Controls the capitalization of text using `text-transform`.
- **Line Height**: Sets the height of a line of text using `line-height`.

## Display and Positioning

- **Display**: Defines the display behavior of an element using `display`.
- **Position**: Specifies the positioning scheme for an element using `position`.
- **Top, Right, Bottom, Left**: Positions an element relative to its closest positioned ancestor using `top`, `right`, `bottom`, and `left`.
- **Float**: Specifies whether an element should float to the left, right, or none using `float`.
- **Clear**: Prevents elements from wrapping around a floated element using `clear`.
- **Overflow**: Controls the behavior of content that overflows its container using `overflow`.

## Flexbox

- **Flex Container**: Defines a flex container using `display: flex`, with additional properties to control flex layout.
- **Flex Items**: Specifies properties for flex items within a flex container, such as `order`, `flex-grow`, `flex-shrink`, and `flex-basis`.

## Grid Layout

- **Grid Container**: Establishes a grid container using `display: grid`, with properties like `grid-template-columns`, `grid-template-rows`, and `grid-template-areas`.
- **Grid Items**: Specifies the placement and span of grid items using properties like `grid-column-start`, `grid-column-end`, `grid-row-start`, and `grid-row-end`.

## Other Features

- **Cursor**: Changes the cursor appearance when hovering over an element using `cursor`.
- **Pointer Events**: Specifies whether an element should respond to pointer events using `pointer-events`.
- **User Select**: Controls whether text can be selected by the user using `user-select`.
- **Box Decoration Break**: Determines how box decorations are split across lines using `box-decoration-break`.
- **@Media Query**: Allows applying CSS rules based on screen size using `@media`.

The cheat sheet provides examples and additional explanations for each CSS property and selector. For more detailed information and live examples, you can refer to the [CSS Reference website](https://cssreference.io/).


```


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

