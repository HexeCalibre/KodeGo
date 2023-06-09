# 2 DAY CSS (06-08-2023)
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

#### How to comment?
```css
  /* this is a comment */
```
#### How to root
```css
*{
   font-size: 20px;
}
```
##### Ways to set a color
###### Color name
```css
h1{
   color: red;
}
``` 
###### Hexadecimal
```css
h1{
   color: #ff0000;
}
``` 
###### RGB
```css
h1{
   color: rgb(255, 255, 0);
}
``` 
##### How to use class with divs
```html
 <div class="container">
  <div class="main-content">
   <h1> CSS Introduction</h1>
  </div>
  <div class="sub-content">
  <h2> CSS Subcontent</h2>
</div>
</div>
```
```css
    container {
    }
    main-content{
    }
    sub-content{
    }
```
                          
class vs id

targeting
selector
propertyname
propertyvalue
call back font
parent
class
id
container

                               
color
background-color
font-family
                               
                               
