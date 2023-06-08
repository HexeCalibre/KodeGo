# DAY 1 CASCADING STYLE SHEET (06-08-2023)
## What is CSS?
CSS stands for Cascading Style Sheet
CSS is used to style a HTML document
CSS can also dictate how HTML elements should be displayed
Not a programming language

## Prerequisite and Reminder
You need to know HTML
You need to be a little artistic
Every developer has its own way of using CSS

## Types of CSS
### Inline CSS
uses the style attribute inside the HTML Elements. (not recommended)
```html
 <h1 style="color: blue">CSS Introduction</h1>
```
### Internal CSS
uses the <style> element inside the <head> of the HTML page.
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
uses and external CSS file which is linked by the <link> element inside the <head> of the HTML page.
 
 ```html
 <head>
  <link rel="stylesheet" href="css/style.css>
 </head>
 ```
                               
 ```css
   @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300&display=swap');
                               
   body {
                               font-family: 'Lato', sans-serif;
       }
 ```
                            
                            
  
