# 3 DAY CSS (06-08-2023)

## Contents

## What is CSS?
- CSS stands for Cascading Style Sheet
- CSS is used to style an HTML document
- CSS can also dictate how HTML elements should be displayed
- Not a programming language

## Prerequisite and Reminder
- You need to know HTML
- You need to be a little artistic
- Every developer has its own way of using CSS

## Types of CSS
### Inline CSS
- Uses the style attribute inside the HTML elements. (not recommended)
```html
<h1 style="color: blue">CSS Introduction</h1>
```
### Internal CSS
- Uses the <style> element inside the <head> of the HTML page.
 ```html
<head>
  <style type="text/css">
    h1 {
        color: green;
    }
  </style>
</head>
<body>
  <h1>CSS Introduction</h1>
</body>
```
### External CSS
- Uses an external CSS file which is linked by the <link> element inside the <head> of the HTML page.
 #### HTML file
 ```html
 <head>
  <link rel="stylesheet" href="css/style.css">
</head>
 ```
 #### CSS file
 ```css
body {
   font-family: 'Lato', sans-serif;
}
 ```
 
## ID vs Class: Targeting and Usage

In CSS, both IDs and classes are used for targeting specific elements, but they have distinct characteristics and purposes. Here's a comparison of IDs and classes, along with examples of how to target them:

### ID Selector

- Represents a unique identifier for an element.
- Denoted by the `#` symbol followed by the ID name.

Example:
```css
#my-id {
  /* Styles applied to the element with ID 'my-id' */
}
 ```
 
### Class Selector
- Represents a group or category of elements. Denoted by a dot (.) followed by the class name.
 
Example:
```css
.my-class {
  /* Styles applied to all elements with the class 'my-class' */
}
```
> To target an element by ID, use the ID selector with the corresponding ID name. For example, if you have an element with the ID of my-id, you can target it using #my-id in your CSS.
>
> To target elements by class, use the class selector with the corresponding class name. For example, if you have multiple elements with the class of my-class, you can target them using .my-class in your CSS.
>
> Remember to replace my-id and my-class with the actual ID and class names used in your HTML code.

 
## CSS Anatomy
> Knowing about CSS anatomy is important because it provides a structured understanding of the different components and terminology used in CSS. Understanding the roles and relationships between selectors, pseudo-?
> classes, declarations, property names, and property values helps in writing more efficient and targeted CSS code. It allows developers to style specific elements, apply different styles based on element states, and 
> control various aspects of element appearance and behavior.
 
 ![CSS Anatomy](images/cssanatomy3.png)
 
 | Term            | Description                                                     |
|-----------------|-----------------------------------------------------------------|
| Selector        | Specifies which HTML elements the CSS rules will be applied to.  |
| Pseudo Class    | Represents a specific state or condition of an element.          |
| Declaration     | Consists of a property name and value, separated by a colon.     |
| Property Name   | Identifies the specific CSS property to be modified.             |
| Property Value  | Specifies the desired value for the corresponding property.      |
 
 
## What is CSS Selector

CSS Selector is a pattern used to select and style specific elements on a web page. Selectors allow you to target elements based on their attributes, types, classes, or relationships with other elements.

There are five categories of CSS selectors:

| Category          | Function and Example                                               |
|-------------------|-------------------------------------------------------------------|
| Type Selector     | Targets elements based on their element type.                     |
| Class Selector    | Targets elements based on their class attribute.                  |
| ID Selector       | Targets elements based on their ID attribute.                     |
| Attribute Selector | Targets elements based on their attribute values.                 |
| Pseudo-class Selector | Targets elements based on special states or conditions.           |

### Type Selector
Type selector targets elements based on their element type.

Example: Select all `<h1>` elements on the page.
```css
h1 {
  color: red;
}
 ```
### Class Selector
Class selector targets elements based on their class attribute.

Example: Select all elements with the class "highlight".
```css
 .highlight {
  background-color: yellow;
}
```
### ID Selector
ID selector targets elements based on their ID attribute.

Example: Select the element with the ID "logo".
```css
 #logo {
  width: 100px;
}
```
### Attribute Selector
Attribute selector targets elements based on their attribute values.

Example: Select all elements with the attribute "target" set to "_blank".
 ```css
 [target="_blank"] {
  text-decoration: underline;
}
```
### Pseudo-class Selector
Pseudo-class selector targets elements based on special states or conditions.

Example: Select the first child of an element.
```css
 :first-child {
  font-weight: bold;
}
```
## CSS Combinators

A combinator is something that explains the relationship between the selectors.

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

| Combinator              | Description                                            | Example                                          |
|-------------------------|--------------------------------------------------------|--------------------------------------------------|
| Descendant Selector     | Matches all elements that are descendants of a specified element. | `div p` { background-color: yellow; }           |
| Child Selector          | Selects all elements that are the children of a specified element. | `parent > child` { /* CSS rules */ }            |
| Adjacent Sibling Selector | Selects an element that is directly after another specific element. | `element + sibling` { /* CSS rules */ }         |
| General Sibling Selector | Selects all elements that are next siblings of a specified element. | `element ~ sibling` { /* CSS rules */ }         |
 
 ## CSS Box Model

The CSS Box Model is a fundamental concept in CSS that describes how elements are laid out on the web page. It consists of four main components:

1. Content: It represents the actual content of the element, such as text, images, or other media.

2. Padding: It creates space around the content inside the element. It is transparent by default and can be set using the `padding` property.

3. Border: It is a line that surrounds the padding and content. It can be styled and customized using properties like `border-width`, `border-color`, and `border-style`.

4. Margin: It creates space outside the element, separating it from other elements on the page. It can be set using the `margin` property.

The diagram below illustrates the CSS Box Model:


![CSS Box Model](images/css_box_model.png)

 ## Importance of Comments in CSS

Comments in CSS are essential for several reasons:

1. **Documentation**: Comments allow you to document your CSS code, providing explanations, descriptions, or reminders for yourself and other developers who may work on the codebase. It helps improve code readability and maintainability.

2. **Code Organization**: Comments can be used to divide your CSS into logical sections, making it easier to navigate and understand. You can create headings or labels within your CSS file to indicate different styles for different sections of your webpage.

3. **Debugging and Troubleshooting**: Comments can be useful for troubleshooting CSS issues. By commenting out sections of code, you can quickly identify problematic styles or isolate specific sections that may be causing unexpected behavior. It helps in the debugging process and makes it easier to locate and fix errors.

4. **Collaboration**: Comments facilitate collaboration among developers working on the same project. They can provide explanations, suggestions, or feedback on specific CSS styles or sections. Comments also make it easier for others to understand your code and make changes or improvements if needed.

5. **Version Control**: Comments can serve as markers or indicators when using version control systems like Git. By adding comments to your CSS code, you can make it easier to track changes, understand the purpose behind specific modifications, and revert to previous versions if necessary.

Remember to use clear and concise comments that effectively convey the intended information without cluttering the code unnecessarily.

Including comments in your CSS code is a good practice that can greatly benefit both you and others who interact with your codebase.

 | Comment Template                              | Example                               |
|-----------------------------------------------|---------------------------------------|
| Single-line comment                          | `/* Comment goes here */`             |
| Multi-line comment                           | `/*                               */` |
| Section Heading comment                  | `/* ========== Section Name ========== */` |
| Description comment                          | `/* Description: Comment goes here */` |
| Author comment                                 | `/* Author: Your Name */`              |
| Date comment                                    | `/* Date: YYYY-MM-DD */`              |
| TODO comment                                   | `/* TODO: Task to be done */`         |
| Deprecated comment                       | `/* Deprecated: Reason for deprecation */` |
| Code snippet comment                       | `/* Code snippet: Description of the code */ */` |
 
 ### How to Comment
 ```css
 /* This is a comment */
 ```
 
## CSS approach or methodology
- refers to a set of principles and guidelines for organizing and structuring CSS code. It provides a systematic way to manage styles, improve code reusability, and enhance maintainability of CSS in web development projects.

 
 | CSS Approach                 | Description                                                                 |
| ---------------------------- | --------------------------------------------------------------------------- |
| Utility-based CSS            | Approach where small, single-purpose utility classes are used for styling.   |
| Component-based CSS          | Styling based on individual components, encapsulating HTML and CSS together. |
| Atomic CSS                   | Extremely granular approach where styles are defined as individual classes.  |
| Object-oriented CSS (OOCSS)  | Separates structure and skin in CSS, promoting code reuse and modularity.    |
| CSS-in-JS                    | CSS styles written directly in JavaScript or JavaScript-based frameworks.   |
| Modular CSS                  | Organizes CSS code into specific modules or layers for improved structure.   |
| BEM (Block Element Modifier) | Naming convention that helps create reusable and modular CSS components.     |
| ACSS (Attribute-Class CSS)   | Uses attributes as selectors, targeting elements based on attribute values.  |
| MCSS (MindBEMding CSS)       | Variant of BEM methodology that focuses on logical CSS structure.            |
| SASS/SCSS                    | CSS preprocessor that adds features like variables, nesting, and mixins.     |
| LESS                         | CSS preprocessor with similar features to SASS but with a different syntax. |
| Stylus                       | Expressive and dynamic CSS preprocessor with a minimalist syntax.            |
| PostCSS                      | CSS post-processor that enhances CSS with various plugins and transformations. |
| Critical CSS                 | Optimizes styles for above-the-fold content to improve initial page load.    |
| Functional CSS               | Small, composable CSS classes that focus on specific visual functions.       |
| Mobile-first CSS             | Approach where CSS styles are designed for mobile devices first.            |
| Responsive CSS               | Uses media queries to apply different styles based on device or viewport.    |
| Flexbox CSS                  | Layout system for creating flexible and responsive designs with CSS.         |
| CSS Grid Layout              | Grid-based layout system for creating complex and responsive web layouts.    |
| Inverted Triangle CSS (ITCSS)| CSS architecture that organizes styles based on specificity and inheritance. |
 
 
## Common Selector Name List
 | Selector Name | Function                                     |
|---------------|----------------------------------------------|
| `#header`     | Represents the header section of a webpage    |
| `#content`    | Represents the main content area              |
| `#sidebar`    | Represents a sidebar or secondary content     |
| `#footer`     | Represents the footer section of a webpage    |
| `#navigation` | Represents a navigation menu or links         |
| `#logo`       | Represents the website or brand logo          |
| `#banner`     | Represents a prominent banner or advertisement|
| `#carousel`   | Represents a carousel or image slider         |
| `#form`       | Represents a form element or form container   |
| `#modal`      | Represents a modal or dialog box              |
| `.container`  | Defines a container element or wrapper         |
| `.title`      | Applies styling to a title or heading          |
| `.button`     | Represents a button element                   |
| `.nav-link`   | Defines a navigation link or menu item         |
| `.card`       | Represents a card or card-like element         |
| `.menu`       | Represents a menu or navigation component     |
| `.section`    | Defines a section or content block             |
| `.highlight`  | Applies highlighting effect to an element      |
| `.text-muted` | Defines muted or subdued text                  |
| `.alert`      | Represents an alert or notification component  |

 
 ## CSS Property Names and Functions

| Property Name      | Function                               | Parameters (if available)                       |
|--------------------|----------------------------------------|-------------------------------------------------|
| `color`            | Sets the text color                    | Color value                                     |
| `background-color` | Sets the background color              | Color value                                     |
| `font-size`        | Sets the font size                     | Size value                                      |
| `font-family`      | Sets the font family                   | Font family name(s)                             |
| `text-align`       | Sets the horizontal alignment of text  | `left`, `right`, `center`, `justify`            |
| `margin`           | Sets the margin around an element      | Size value or `auto`                            |
| `padding`          | Sets the padding inside an element     | Size value or `auto`                            |
| `border`           | Sets the border style, width, and color| Style, width value, and color value              |
| `width`            | Sets the width of an element           | Size value or `auto`                            |
| `height`           | Sets the height of an element          | Size value or `auto`                            |
| `display`          | Sets how an element is displayed       | `block`, `inline`, `inline-block`, `flex`, etc.  |
| `position`         | Sets the positioning method of an element | `static`, `relative`, `absolute`, `fixed`, etc. |
| `float`            | Sets the horizontal alignment of an element | `left`, `right`, `none`                       |
| `text-decoration`  | Sets the decoration of text            | `none`, `underline`, `line-through`, etc.        |
| `text-transform`   | Sets the capitalization of text        | `capitalize`, `uppercase`, `lowercase`, `none`   |
| `box-shadow`       | Sets the shadow of an element          | Shadow parameters (e.g., color, offset, blur radius) |
| `transition`       | Sets the transition effects on an element | Transition parameters (e.g., property, duration) |
| `animation`        | Sets the animation effects on an element | Animation parameters (e.g., name, duration)      |
 
 ## Absolute Units
 - These units are considered absolute because they represent fixed measurements that do not change based on the context or size of other elements. They provide precise control over element dimensions, font sizes, and other properties.

 | Unit   | Description                                      | Example               |
|--------|--------------------------------------------------|-----------------------|
| cm     | Centimeters                                      | `width: 5cm;`         |
| mm     | Millimeters                                      | `font-size: 3mm;`     |
| in     | Inches                                           | `margin-top: 0.5in;`  |
| px     | Pixels                                           | `padding-left: 10px;` |
| pt     | Points (1pt = 1/72 of an inch)                    | `font-size: 12pt;`    |
| pc     | Picas (1pc = 12 points)                           | `line-height: 1.5pc;` |
| Q      | Quarter-millimeters                               | `border-width: 0.25Q;`|
| rem    | Relative to the root element's font size          | `margin-bottom: 1.5rem;` |
| vw     | Relative to the viewport width                    | `width: 50vw;`        |
| vh     | Relative to the viewport height                   | `height: 75vh;`       |
| vmin   | Relative to the smaller dimension of the viewport | `font-size: 3vmin;`   |
| vmax   | Relative to the larger dimension of the viewport  | `padding: 2vmax;`     |
 
 ## Relative Units
 - These units are considered relative because they are calculated based on some reference point or context. They allow for flexible and responsive designs, as they adapt to changes in the parent element, viewport size, or root font size.

 | Unit   | Description                                      | Example                |
|--------|--------------------------------------------------|------------------------|
| em     | Relative to the font-size of the element          | `margin: 1em;`         |
| ex     | Relative to the x-height of the font              | `line-height: 2ex;`    |
| ch     | Relative to the width of the "0" (zero) character | `width: 10ch;`         |
| %      | Relative to the parent element's property value   | `width: 50%;`          |
| fr     | Fractional unit                                  | `grid-template-columns: 1fr 2fr;` |
| rem    | Relative to the root element's font size          | `font-size: 1.2rem;`   |
| vw     | Relative to the viewport width                    | `width: 25vw;`         |
| vh     | Relative to the viewport height                   | `height: 50vh;`        |
| vmin   | Relative to the smaller dimension of the viewport | `font-size: 2vmin;`    |
| vmax   | Relative to the larger dimension of the viewport  | `padding: 3vmax;`      |



 
 ### The Root Selector
 ```css
 * {
   font-size: 20px;
}
 ```
 ### Ways to set a color
 ```css
 /* Color Name */
 h1 {
   color: red;
}
/* Hexadecimal */
 h1 {
   color: #ff0000;
}
/* RGB */
 h1 {
   color: rgb(255, 255, 0);
}
```
 
 




