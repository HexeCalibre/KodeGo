# 2 DAY CSS (06-08-2023)

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
 ```html
 @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&display=swap');

body {
   font-family: 'Lato', sans-serif;
}
 ```
 ### How to Comment
 ```html
 /* This is a comment */
 ```
 
 ### The Root Selector
 ```html
 * {
   font-size: 20px;
}
 ```
 ### Ways to set a color
 ```html
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




