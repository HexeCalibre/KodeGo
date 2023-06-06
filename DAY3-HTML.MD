# 2 DAY HTML 06/03/2023
## Contents
> [Prerequisite](https://github.com/HexeCalibre/KodeGo/blob/master/DAY3-HTML.MD#prerequisite)
>
> [Learn to code](https://github.com/HexeCalibre/KodeGo/blob/master/DAY3-HTML.MD#where-to-start)
>
> [What is OOP?](https://github.com/HexeCalibre/KodeGo/blob/master/DAY3-HTML.MD#object-oriented-programming-oop)
>
> [HTML Tags](https://github.com/HexeCalibre/KodeGo/blob/master/DAY3-HTML.MD#tags)
>
> [HTML Form Attributes and Usage](https://github.com/HexeCalibre/KodeGo/blob/master/DAY3-HTML.MD#html-form-attributes-and-usage)

## Prerequisite
> [Visual Studio Code Download](https://code.visualstudio.com/download)
>
> [GitHub Signup](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home)
### VSCODE Extensions to start with
Extension name | Extension ID
-------------- | --------------
Live Preview    | ms-vscode.live-server
LiveServer     | ritwickdey.LiveServer
Lorem Ipsum    | Tyriar.lorem-ipsum
Prettier - Code Formatter     | esbenp.prettier-vscode
GitLens    | eamodio.gitlens
GitHub Pull Requests and Issues     | GitHub.vscode-pull-request-github
Auto Rename Tag    | formulahendry.auto-rename-tag
CSS Flexbox Cheatsheet     | dzhavat.css-flexbox-cheatsheet
CSS Grid Snippets    | ohansemmanuel.css-grid-snippets
CSS Peek     | pranaygp.vscode-css-peek

### Where to Start?
[SoloLearn](https://www.sololearn.com/users/login?returnUrl=%2Fprofile)

[W3Schools](https://www.w3schools.com/html/default.asp)

[Roadmap.sh](https://roadmap.sh/frontend)

## Object-Oriented Programming (OOP)
### What is OOP?
OOP (Object-Oriented Programming) is a programming approach that emphasizes organizing code around objects. Objects are instances of classes and represent real-world entities or concepts. 

| Term        | Definition                                                  |
| ----------- | ----------------------------------------------------------- |
| Encapsulate | In programming, encapsulation refers to bundling data and methods into a single unit (object) and providing a well-defined interface for interacting with it. It helps hide internal details and protect data integrity. |
| Nesting     | In programming, nesting refers to placing one code construct (such as a loop or conditional statement) inside another. It allows for hierarchical structuring of code and is commonly used to create complex logic and relationships between different components. |
| Inheritance | In object-oriented programming, inheritance is the mechanism by which a class inherits properties and behaviors from another class. It promotes code reuse and enables the creation of hierarchical relationships between classes, with child classes inheriting features from parent classes. |
| Polymorphism | Polymorphism is the ability of an object or method to take on different forms or behaviors based on the context in which it is used. It allows for flexibility and extensibility in object-oriented programming, enabling objects to be treated as instances of their own class or any of their parent classes. |
| Abstraction | Abstraction involves simplifying complex systems by focusing on the essential aspects while ignoring irrelevant details. In programming, abstraction allows for the creation of abstract classes or interfaces that define common behavior without specifying the implementation, promoting code modularity and flexibility. |



## Tags
### Head Content
| Tags                                                         | Function                                                   |
| ------------------------------------------------------------ | ---------------------------------------------------------- |
| `<!DOCTYPE html>`                                             | Specifies the HTML version as HTML5.                       |
| `<html lang="en"> </html>`                                    | Defines the root element of an HTML document.              |
| `<head> </head>`                                              | Represents the container for the document's metadata.      |
| `<meta>`                                                      | Represents various types of metadata in an HTML document.  |
| `<meta charset="UTF-8">`                                       | Specifies the character encoding for the HTML document.    |
| `<meta http-equiv="X-UA-Compatible" content="IE=edge">`        | Sets the browser compatibility mode for Internet Explorer. |
| `<meta name="viewport" content="width=device-width, initial-scale=1.0">` | Configures the viewport settings for responsive web design. |
| `<meta name="author" content="Ritz Carl Feliciano">`           | Specifies the author of the HTML document.                |
| `<meta name="description" content="Another HTML">`            | Provides a brief description of the HTML document.         |
| `<meta name="keywords" content="HTML, CSS, JS, semantic, beginners">` | Defines keywords related to the HTML document.             |
| `<script src="https://kit.fontawesome.com/7902a8a385.js" crossorigin="anonymous"></script>` | Imports an external JavaScript file from a URL.           |
| `<link rel="stylesheet" href="css/style.css">`               | Links an external CSS file to the HTML document.           |
| `<title>HTML introduction</title>`                            | Defines the title of the HTML document displayed in the browser. |

#### Example
```html
<!DOCTYPE html>
<html lang='en'>
<head>
    <meta charset='UTF-8'>
    <meta http-equiv='X-UA-Compatible' content='IE=edge'>
    <meta name='viewport' content='width=device-width, initial-scale=1.0'>
    <meta name='author' content='Ritz Carl Feliciano'>
    <meta name='description' content='Another HTML'>
    <meta name='keywords' content='HTML, CSS, JS, semantic, beginners'>
    <script src="https://kit.fontawesome.com/7902a8a385.js" crossorigin="anonymous"></script>
    <link rel='stylesheet' href='css/style.css'>
    <title>HTML introduction</title>
</head>
</html>
```

### Body Elements
| Tags       | Function                                                     |
| ---------- | ------------------------------------------------------------ |
| `<body>`   | Represents the content of an HTML document.                   |
| `<div>`    | Defines a division or a section in an HTML document.         |
| `<span>`   | Defines an inline container for a specific text or a part of a document. |
| `<h1>`     | Defines a top-level heading in an HTML document.             |
| `<h2>`     | Defines a second-level heading in an HTML document.          |
| `<h3>`     | Defines a third-level heading in an HTML document.           |
| `<h4>`     | Defines a fourth-level heading in an HTML document.          |
| `<h5>`     | Defines a fifth-level heading in an HTML document.           |
| `<h6>`     | Defines a sixth-level heading in an HTML document.           |
| `<p>`      | Defines a paragraph in an HTML document.                     |
| `<a>`      | [Creates a hyperlink](URL) to another web page or resource.  |
| `<img>`    | Embeds an image into an HTML document.                       |
| `<ul>`     | Defines an unordered list in an HTML document.               |
| `<ol>`     | Defines an ordered list in an HTML document.                 |
| `<li>`     | Defines a list item in an HTML document.                     |
| `<table>`  | Represents tabular data in an HTML document.                 |
| `<tr>`     | Defines a row in an HTML table.                              |
| `<td>`     | Defines a cell in an HTML table.                             |
| `<form>`   | Creates an HTML form for user input.                         |
| `<input>`  | Defines an input control within an HTML form.                |
| `<button>` | Creates a clickable button in an HTML document.              |
| `<label>`  | Defines a label for an HTML form element.                    |
| `<select>` | Creates a dropdown list in an HTML form.                     |
| `<textarea>` | Defines a multiline text input control in an HTML form.      |
| `<strong>` | Represents strong importance or emphasis on text.            |
| `<em>`     | Indicates emphasis on text, typically displayed in italics.  |
| `<sub>`    | Defines subscript text.                                      |
| `<sup>`    | Defines superscript text.                                    |
| `<strike>` | Represents strikethrough text.                               |
| `<bookmark>` | Represents a bookmark or anchor point within an HTML document. |
    
#### Input Types
| Input Type    | Description                                                             |
| ------------- | ----------------------------------------------------------------------- |
| `text`        | Single-line input field for plain text.                                   |
| `password`    | Masked input field for passwords or sensitive information.               |
| `email`       | Input field for email addresses.                                          |
| `number`      | Input field for numeric values.                                           |
| `date`        | Input field for selecting a date.                                         |
| `checkbox`    | Checkbox for selecting multiple options.                                  |
| `radio`       | Radio buttons for selecting a single option.                              |
| `file`        | Input field for uploading files.                                          |
| `textarea`    | Multi-line input field for longer text or comments.                       |
| `select`      | Drop-down list for selecting an option from a list.                       |
| `color`       | Input field for selecting a color.                                        |
| `range`       | Slider input for selecting a value within a range.                        |

#### Case Style
| Case Style    | Description                                                           |
| ------------- | --------------------------------------------------------------------- |
| `camelCase`   | Style where words are joined together, and each subsequent word starts with a capital letter except for the first word. |
| `PascalCase`  | Style where words are joined together, and each word starts with a capital letter. |
| `kebab-case`  | Style where words are separated by hyphens.                            |
| `snake_case`  | Style where words are separated by underscores.                        |

#### HTML Form Attributes and Usage
| Attribute   | Usage                                                         |
| ----------- | ------------------------------------------------------------- |
| `for`       | Associates a label with a form element. It specifies which form element the label belongs to. |
| `type`      | Defines the type of input control to be displayed. It specifies the kind of data expected by the form element. |
| `id`        | Provides a unique identifier for the form element. It is used to associate the element with a label or manipulate it through JavaScript or CSS. |
| `required`  | Specifies that the form element must be filled out before submitting the form. It ensures the input is mandatory. |
| `name`      | Specifies the name of the form element. It is used to identify the form data on the server-side when the form is submitted. |
| `multiple`  | Allows multiple values to be selected for the form element. This attribute is typically used with `<select>` or `<input type="file">` elements. |
| `pattern`   | Specifies a regular expression pattern that the form element's value must match for successful validation. |
| `placeholder` | Provides a short hint or example text that is displayed in the form element before the user enters a value. |
| `value`     | Sets the initial value for the form element. It can be used to pre-fill or preset the input with a default value. |


```html
<body>
    <form action="#" method="post" enctype="application/x-www-form-urlencoded" >
        <fieldset>
            <legend>HTML Form</legend>
            <label for="firstname" >First Name<label>
            <input type="text" id="firstname" name="fname" required>
            <br><br>
            <label for="lastname">Last Name<label>
            <input type="text" id="lastname" name="lname" required>
            <br><br>
            <label for="bday">Birthday<label>
            <input type="date" id="bday" name="dob" required>
            <br><br>    
            <input type="radio" id="male" name="gender" value="M" required>
            <label for="male">Male</label>
            <input type="radio" id="female" name="gender" value="F" required>
            <label for="female">Female</label>
            <br><br>            
            <label for="email">Email<label>
            <input type="email" id="email" name="email" required>
            <br><br>
            <label for="password">Password<label>                   
            <input type="password" id="password" name="pword" required>
            <br><br>
            <input type="submit">
        </fieldset>
     <form>
    <form action="#" method="post" enctype="application/x-www-form-urlencoded" >
        <fieldset>
            <legend>HTML Form</legend>
            <label for="firstname" >First Name<label>
            <input type="text" id="firstname" name="fname" >
            <br><br>
            <label for="lastname">Last Name<label>
            <input type="text" id="lastname" name="lname" >
            <br><br>
            <label for="bday">Birthday<label>
            <input type="date" id="bday" name="dob" >
            <br><br>
            <label for="month">Birthday Month</label>
            <input type="month" id="birthdayMonth" name="birthdayMonth">
            <br><br>
            <label for="birthdayWeek">Birthday Week</label>
            <input type="week" id="birthdayWeek" name="birthdayWeek">
            <br><br>
            <label for="time">Birthday Time</label>
            <input type="time" id="time" name="time" >
            <br><br>
            <label for="birthdayTime">Birthday (date and time)<label>
            <input type="datetime-local" id="birthdayTime" name="dob" >
            <br><br>
            <input type="radio" id="male" name="gender" value="M" >
            <label for="male">Male</label>
            <input type="radio" id="female" name="gender" value="F" >
            <label for="female">Female</label>
            <br><br>
            <label>Languages</label>
            <br><br>
            <input type="checkbox" id="tagalogLanguage" name="tagalogLanguage" value="tag" >
            <label>Tagalog</label>
            <input type="checkbox" id="englishLanguage" name="englishLanguage" value="eng" >
            <label>English</label>
            <br><br>
            <label for="email">Email<label>
            <input type="email" id="email" name="email" >
            <br><br>
            <label>Education Attainment</label>
            <select name="educatoin" id="education" multiple>
                <option value="CD">College Degree</option>
                <option value="AD">Associate Degree</option>
                <option value="DD">Doctorate Degree</option>
            </select>
            <br><br>
            <label for="password">Password<label>
            <input type="password" id="password" name="pword" >
            <br><br>
            <label for="">Upload Picture</label>
            <input type="file" accept=".jpeg,.jpg,.jpeg,.png,.svg,.ico" >
            <br><br>
            <label for="">Favorite Color</label>
            <input type="color" id="favoriteColor" name="favoriteColor" >
            <br><br>
            <label for="age">Age</label>
            <input type="number" id="age" name="age" min="150">
            <br><br>
            <label for="">Salary Range</label>
            <input type="range" id="salaryRange" name="salaryRange" min="0" max="1">
            <br><br>
            <label for="tel">Mobile/Phone Number</label>
            <input type="tel" id="tel" name="tel" pattern="[0-9]{3}-[0-9]{7}" maxlength="11" placeholder="0919-2124611">
            <br><br>
            <label for="search">Search</label>
            <input type="search" id="search" name="search">
            <br><br>
            <label for="message">Message</label>
            <br>
            <textarea name="message" id="message" cols="20" rows="10" placeholder="Enter your message here."></textarea>
            <br><br>
            <label for="url">Webpage</label>
            <input type="url" id="url" name="url" placeholder="www.example.com">
            <br><br>
            <input type="hidden" id="id" name="id" value="1">
            <br><br>
            <input type="submit">
        </fieldset>
</body>
```

  


