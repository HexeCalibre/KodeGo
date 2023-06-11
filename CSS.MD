# 2 DAY CSS (06-08-2023)

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
 
## CSS Anatomy
> Knowing about CSS anatomy is important because it provides a structured understanding of the different components and terminology used in CSS. Understanding the roles and relationships between selectors, pseudo-?
> classes, declarations, property names, and property values helps in writing more efficient and targeted CSS code. It allows developers to style specific elements, apply different styles based on element states, and > > > control various aspects of element appearance and behavior.
 
 | Term            | Description                                                     |
|-----------------|-----------------------------------------------------------------|
| Selector        | Specifies which HTML elements the CSS rules will be applied to.  |
| Pseudo Class    | Represents a specific state or condition of an element.          |
| Declaration     | Consists of a property name and value, separated by a colon.     |
| Property Name   | Identifies the specific CSS property to be modified.             |
| Property Value  | Specifies the desired value for the corresponding property.      |
 
 ![CSS Anatomy](images/cssanatomy3.png)
 
## What is Targeting?

Targeting in CSS refers to the process of selecting specific HTML elements to apply styles or modify their behavior. It involves using selectors, pseudo-classes, and combinators to pinpoint the elements you want to target.

### Why Do We Need to Know Targeting?

Understanding targeting in CSS is crucial for effective web development and styling. Here are a few reasons why it is important to grasp this concept:

- **Selective Styling**: Targeting allows us to apply styles selectively to specific elements, enhancing the visual appearance of our web pages.

- **Modifying Behavior**: By targeting elements, we can modify their behavior through CSS rules, enabling interactivity and dynamic effects.

- **Efficient Styling**: Knowing how to target elements helps us write more efficient and concise CSS code, reducing redundancy and improving performance.

- **Maintainable Code**: Targeting allows for better organization and structure in our CSS code, making it easier to maintain and update styles.

- **Consistency**: By understanding targeting, we can ensure consistent styling across our web pages, creating a cohesive user experience.

### Targeting Methods

| Method       | Description                                                                                   |
|--------------|-----------------------------------------------------------------------------------------------|
| Selectors    | Selectors allow us to target elements based on their tag names, classes, IDs, or attributes. |
| Pseudo-classes | Pseudo-classes target elements based on specific states or conditions.                          |
| Combinators  | Combinators help select elements based on their relationship with other elements.              |

 
 ### How to Comment
 ```css
 /* This is a comment */
 ```
 
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




