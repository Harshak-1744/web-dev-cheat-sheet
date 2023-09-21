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

# Selectors

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


# Colors and Backgrounds

### **Color**: Sets the text color using `color`.
```css
color: value;               /* For text color */
```

### **Background Color**: Sets the background color using `background-color`.
```css
background-color: value;    /* For background color */
```

### **Opacity**: Specifies the opacity of an element using `opacity` (range: 0 to 1).
```css
opacity: value;             /* Range: 0 to 1 */
```

### **Background Image**: Sets a background image using `background-image`.
```css
background-image: url('image.jpg');
```

### **Background Repeat**: Controls how the background image is repeated using `background-repeat`.
```css
background-repeat: repeat | repeat-x | repeat-y | no-repeat;
```

### **Background Attachment**: Specifies whether the background image scrolls with the content using `background-attachment`.
```css
background-attachment: scroll | fixed | local;
```

### **Background Position**: Sets the starting position of the background image using `background-position`.
```css
background-position: x y;
```

### **Background Size**: Adjusts the size of the background image using `background-size`.
```css
background-size: auto | cover | contain;
```


## Box Model

The Box Model in CSS refers to how elements are rendered and how their dimensions and spacing are calculated. It consists of the following properties:

### **Width and Height**: Sets the width and height of elements using `width` and `height`.
  ```css
  width: value;               /* E.g., 100px, 50%, auto */
  height: value;              /* E.g., 100px, 50%, auto */
  ```

### **Margin**: Sets the space outside an element's border using `margin`.
  ```css
  margin: top right bottom left;
  ```

### **Padding**: Sets the space between an element's content and its border using `padding`.
  ```css
  padding: top right bottom left;
  ```

### **Border**: Defines the border width, style, and color using `border`.
  ```css
  border: width style color;
  ```

### **Border Radius**: Creates rounded corners for elements using `border-radius`.
  ```css
  border-radius: value;       /* E.g., 5px, 50% */
  ```

### **Box Shadow**: Applies a shadow effect to elements using `box-shadow`.
  ```css
  box-shadow: h-offset v-offset blur spread color;
  ```

![box-model](https://github.com/Harshak-1744/web-dev-cheat-sheet/assets/85007461/ebd78dc9-f677-43ab-acba-52a81ee72cc1)


## Text Styling

Text Styling in CSS allows you to control the appearance of text within your web page. It includes various properties that affect the font, size, alignment, decorations, capitalization, and line height. Below are the details and examples of each property:

### **Font Family**: Specifies the font family for text using `font-family`.
  ```css
  font-family: Arial, sans-serif;
  ```

### **Font Size**: Sets the font size using `font-size`.
  ```css
  font-size: value;           /* E.g., 16px, 1rem, 1em */
  ```

### **Font Weight**: Defines the thickness of characters using `font-weight`.
  ```css
  font-weight: normal | bold | bolder | lighter | number;
  ```

### **Text Align**: Aligns text within its container using `text-align`.
  ```css
  text-align: left | right | center | justify;
  ```

### **Text Decoration**: Adds decoration to text, such as underline or line-through, using `text-decoration`.
  ```css
  text-decoration: none | underline | overline | line-through;
  ```

### **Text Transform**: Controls the capitalization of text using `text-transform`.
  ```css
  text-transform: capitalize | uppercase | lowercase | none;
  ```

### **Line Height**: Sets the height of a line of text using `line-height`.
  ```css
  line-height: value;         /* E.g., 1.5, 24px, 150% */
  ```


## Display and Positioning

The "Display and Positioning" section in CSS allows you to control how elements are displayed and positioned on your web page. It includes properties that determine the layout behavior and placement of elements. Below are the details and examples of each property:

### **Display**: Defines the display behavior of an element using `display`.
```css
display: block | inline | inline-block | flex | grid | none;
```

### **Position**: Specifies the positioning scheme for an element using `position`.
```css
position: static | relative | absolute | fixed | sticky;
```

### **Top, Right, Bottom, Left**: Positions an element relative to its closest positioned ancestor using `top`, `right`, `bottom`, and `left`.
```css
top: value;
right: value;
bottom: value;
left: value;
```

### **Float**: Specifies whether an element should float to the left, right, or none using `float`.
```css
float: left | right | none;
```

### **Clear**: Prevents elements from wrapping around a floated element using `clear`.
```css
clear: left | right | both | none;
```

### **Overflow**: Controls the behavior of content that overflows its container using `overflow`.
```css
overflow: visible | hidden | scroll | auto;
```




## Flexbox

Flexbox is a flexible layout system in CSS that provides a more efficient way to distribute and align elements within a container. It consists of two main components: the Flex Container and Flex Items.

### Flex Container

The Flex Container is the parent element that holds a collection of Flex Items. To create a flex container, you need to set the `display` property to `flex`. Additionally, there are several properties that allow you to control the layout and arrangement of the flex items within the container:

### **`display: flex`**: Defines a flex container.
```css
/* Flex Container */
display: flex;
```

### **`flex-direction`**: Specifies the main axis along which the flex items are laid out. It can take one of four values:
  - `row`: Flex items are arranged horizontally in a row (default).
  - `row-reverse`: Flex items are arranged horizontally in a row, but in reverse order.
  - `column`: Flex items are arranged vertically in a column.
  - `column-reverse`: Flex items are arranged vertically in a column, but in reverse order.
```css
flex-direction: row | row-reverse | column | column-reverse;
```

### **`flex-wrap`**: Controls whether the flex items should wrap to a new line or stay on the same line. It can take one of three values:
  - `nowrap`: Flex items are laid out in a single line (default).
  - `wrap`: Flex items wrap to a new line when they exceed the container's width.
  - `wrap-reverse`: Flex items wrap to a new line in reverse order when they exceed the container's width.
```css
flex-wrap: nowrap | wrap | wrap-reverse;
```

### **`justify-content`**: Aligns flex items along the main axis. It determines how extra space is distributed when flex items don't fill the container. It can take one of five values:
  - `flex-start`: Flex items are aligned to the start of the container (left for `row`, top for `column`).
  - `flex-end`: Flex items are aligned to the end of the container (right for `row`, bottom for `column`).
  - `center`: Flex items are centered along the main axis.
  - `space-between`: Flex items are evenly distributed along the main axis with equal space between them.
  - `space-around`: Flex items are evenly distributed along the main axis with equal space around them.
```css
justify-content: flex-start | flex-end | center | space-between | space-around;
```

### **`align-items`**: Aligns flex items along the cross axis. It determines how flex items are aligned when they don't stretch to fill the container. It can take one of five values:
  - `flex-start`: Flex items are aligned to the start of the cross axis.
  - `flex-end`: Flex items are aligned to the end of the cross axis.
  - `center`: Flex items are centered along the cross axis.
  - `baseline`: Flex items are aligned based on their baselines.
  - `stretch`: Flex items are stretched to fill the container along the cross axis (default).
```css
align-items: flex-start | flex-end | center | baseline | stretch;
```

### **`align-content`**: Aligns a flex container's lines within the container when there is extra space in the cross axis. It can take one of six values:
  - `flex-start`: Lines are packed at the start of the container.
  - `flex-end`: Lines are packed at the end of the container.
  - `center`: Lines are centered within the container.
  - `space-between`: Lines are evenly distributed with equal space between them.
  - `space-around`: Lines are evenly distributed with equal space around them.
  - `stretch`: Lines are stretched to fill the container.
```css
align-content: flex-start | flex-end | center | space-between | space-around | stretch;
```

### Flex Items

Flex Items are the child elements inside a flex container. By default, they will be arranged in a row along the main axis. However, there are properties that allow you to control the behavior of individual flex items:

### **`order`**: Specifies the order in which flex items appear within the flex container. It takes an integer value, and items are ordered based on their `order` value in ascending order.
```css
/* Flex Items */
order: value;
```

### **`flex-grow`**: Determines how much a flex item should grow relative to the other flex items within the same container. It takes a number value, and the ratio of `flex-grow` values determines how the remaining space is distributed among flex items.
```css
flex-grow: value;
```

### **`flex-shrink`**: Specifies how much a flex item should shrink relative to the other flex items when there is not enough space in the container. It takes a number value, and the ratio of `flex-shrink` values determines how much each flex item will shrink.
```css
flex-shrink: value;
```

### **`flex-basis`**: Defines the initial size of a flex item along the main axis before any remaining space is distributed. It can take a fixed value (e.g., `px`, `em`, etc.) or a relative value (e.g., `%`, `auto`, etc.).
```css
flex-basis: value;
```

### **`flex` (Shorthand)**: A shorthand property that combines `flex-grow`, `flex-shrink`, and `flex-basis` properties into one. It is specified as `flex: grow shrink basis`.
```css
flex: grow shrink basis;
```

### **`align-self`**: Allows you to override the `align-items` property for individual flex items. It can take the same five values as `align-items`: `auto`, `flex-start`, `flex-end`, `center`, `baseline`, or `stretch`.
```css
align-self: auto | flex-start | flex-end | center | baseline | stretch;
```


### Grid Container Properties

**Display**: Specifies that the element is a grid container.

```css
display: grid;
```

**Grid Template Columns**: Defines the size of grid columns. Values can be in pixels, percentages, or `auto`.

```css
grid-template-columns: value;
```

**Grid Template Rows**: Defines the size of grid rows. Values can be in pixels, percentages, or `auto`.

```css
grid-template-rows: value;
```

**Grid Template Areas**: Assigns grid areas defined with specific names to the elements within the grid.

```css
grid-template-areas: area-name;
```

**Grid Template**: Shorthand for defining both `grid-template-rows` and `grid-template-columns` in one property.

```css
grid-template: "header header header" 1fr
               "sidebar main main" 2fr
               "footer footer footer" 1fr;
```

**Grid Column Gap**: Sets the size of the gap (spacing) between columns.

```css
grid-column-gap: value;
```

**Grid Row Gap**: Sets the size of the gap (spacing) between rows.

```css
grid-row-gap: value;
```

**Grid Gap**: Shorthand for defining both `grid-row-gap` and `grid-column-gap` in one property.

```css
grid-gap: row-gap column-gap;
```

### Grid Items Properties

**Grid Column Start**: Defines the starting column line for a grid item.

```css
grid-column-start: value;
```

**Grid Column End**: Defines the ending column line for a grid item.

```css
grid-column-end: value;
```

**Grid Row Start**: Defines the starting row line for a grid item.

```css
grid-row-start: value;
```

**Grid Row End**: Defines the ending row line for a grid item.

```css
grid-row-end: value;
```

**Grid Column**: Shorthand for defining both `grid-column-start` and `grid-column-end` in one property.

```css
grid-column: start / end;
```

**Grid Row**: Shorthand for defining both `grid-row-start` and `grid-row-end` in one property.

```css
grid-row: start / end;
```

**Grid Area**: Assigns a grid area name to the grid item, as defined in the `grid-template-areas`.

```css
grid-area: area-name;
```


### Flexbox and Grid Shortcuts

**Flex Container Shortcut**: This property is used to create a flex container and set its main axis direction and wrapping behavior in one line.

```css
/* Flex Container Shortcut */
display: flex;
flex-flow: flex-direction flex-wrap;
```

- `display: flex`: Specifies that the element is a flex container.
- `flex-flow`: Shorthand for defining both `flex-direction` and `flex-wrap` in one property.

**Flex Items Shortcut**: This property is used to control the flex properties of individual flex items within a flex container.

```css
/* Flex Items Shortcut */
flex: flex-grow flex-shrink flex-basis;
```

- `flex`: Shorthand for defining both `flex-grow`, `flex-shrink`, and `flex-basis` in one property.

### Box Sizing

**Box Sizing**: This property allows you to control how the total width and height of an element are calculated. By default, an element's width and height only include its content box, but with this property, you can include padding and border in the total size.

```css
box-sizing: content-box | border-box;
```

- `content-box`: The element's width and height only include its content box.
- `border-box`: The element's width and height include content, padding, and border.

### Visibility

**Visibility**: This property determines whether an element is visible or hidden on the web page.

```css
visibility: visible | hidden;
```

- `visible`: The element is visible.
- `hidden`: The element is hidden and does not take up space on the page.

### Opacity

**Opacity**: This property controls the transparency of an element, allowing you to adjust its opacity from completely transparent to fully opaque.

```css
opacity: value;             /* Range: 0 to 1 */
```

- `value`: A number between 0 and 1, where 0 is completely transparent, and 1 is fully opaque.

### Z-index

**Z-index**: This property specifies the stacking order of elements on the z-axis, determining which element appears above or below other elements.

```css
z-index: value;
```

- `value`: An integer that determines the stacking order. Higher values appear above lower values.

### Transition

**Transition**: This property adds smooth transitions to CSS properties when they change, creating animations between different states.

```css
transition: property duration timing-function delay;
```

- `property`: The CSS property you want to apply the transition to.
- `duration`: The time it takes for the transition to complete, specified in seconds or milliseconds.
- `timing-function`: The speed curve of the transition, such as `ease`, `linear`, `ease-in`, `ease-out`, etc.
- `delay`: The time before the transition starts, specified in seconds or milliseconds.

### Animation

**Animation**: This property allows you to create complex animations by combining multiple animation properties.

```css
animation-name: name;
animation-duration: value;
animation-timing-function: value;
animation-delay: value;
animation-iteration-count: value;
animation-direction: normal | reverse | alternate | alternate-reverse;
animation-fill-mode: none | forwards | backwards | both;
animation-play-state: running | paused;
```

- `animation-name`: The name of the keyframes animation to be applied.
- `animation-duration`: The time it takes for the animation to complete, specified in seconds or milliseconds.
- `animation-timing-function`: The speed curve of the animation, such as `ease`, `linear`, `ease-in`, `ease-out`, etc.
- `animation-delay`: The time before the animation starts, specified in seconds or milliseconds.
- `animation-iteration-count`: The number of times the animation should repeat.
- `animation-direction`: The direction of the animation, whether `normal`, `reverse`, `alternate`, or `alternate-reverse`.
- `animation-fill-mode`: Determines what values are applied to the element before and after the animation, such as `none`, `forwards`, `backwards`, or `both`.
- `animation-play-state`: Controls whether the animation is running or paused, using `running` or `paused`.


### Cursor

**Cursor**: Changes the cursor appearance when hovering over an element.

```css
cursor: pointer | auto | crosshair | default | help | move | text | wait | ...;
```

- `pointer`: The cursor will be displayed as a hand, indicating a clickable element.
- `auto`: The browser will determine the cursor based on the context.
- `crosshair`: The cursor will be displayed as a crosshair, indicating selection mode.
- `default`: The default cursor for the element.
- `help`: The cursor will be displayed as a question mark, indicating help mode.
- `move`: The cursor will be displayed as a four-headed arrow, indicating movement mode.
- `text`: The cursor will be displayed as an I-beam, indicating text input mode.
- `wait`: The cursor will be displayed as an hourglass, indicating that the program is busy.

### Pointer Events

**Pointer Events**: Specifies whether an element should respond to pointer events.

```css
pointer-events: none | auto;
```

- `none`: The element will not respond to pointer events, making it non-clickable and non-selectable.
- `auto`: The element will respond to pointer events, making it clickable and selectable.

### User Select

**User Select**: Controls whether text can be selected by the user.

```css
user-select: none | auto;
```

- `none`: Text cannot be selected, preventing users from highlighting and copying the text.
- `auto`: Text can be selected by the user, allowing normal text selection behavior.

### Box Decoration Break

**Box Decoration Break**: Determines how box decorations are split across lines.

```css
box-decoration-break: slice | clone;
```

- `slice`: Box decorations (e.g., borders and backgrounds) will not be duplicated at the break points when content wraps.
- `clone`: Box decorations (e.g., borders and backgrounds) will be duplicated at the break points when content wraps.

### @Media Query

**@Media Query**: Allows applying CSS rules based on screen size and other media conditions.

```css
@media screen and (max-width: value) {
  /* CSS rules for specific screen size */
}
```

The `@media` rule is used to define a specific set of CSS rules that will be applied only when certain conditions are met. In this case, the rules within the media query block will only be applied on screens with a maximum width specified by the `value`.

### @Font Face

**@Font Face**: Defines custom font families that can be used within your CSS.

```css
@font-face {
  font-family: 'FontName';
  src: url('font.woff2') format('woff2'),
       url('font.woff') format('woff');
}
```

The `@font-face` rule allows you to use custom fonts on your web page. You can specify the font family name (`FontName`) and the URL to the font files in different formats (`woff2` and `woff`).

### @Keyframes

**@Keyframes**: Defines animations and their intermediate steps for use with the `animation` property.

```css
@keyframes animation-name {
  0% {
    property: value;
  }
  100% {
    property: value;
  }
}
```

The `@keyframes` rule is used to define the keyframes for an animation, specifying the intermediate steps at different percentages (0% to 100%) of the animation duration. The `animation-name` should match the animation name used in the `animation` property.



The cheat sheet provides examples and additional explanations for each CSS property and selector. For more detailed information and live examples, you can refer to the [CSS Reference website](https://cssreference.io/).


