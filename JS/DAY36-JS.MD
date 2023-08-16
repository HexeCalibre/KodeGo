# JAVASCRIPT DOM 07/08/2023

## DOM Manipulation

DOM manipulation refers to the practice of using programming techniques to interact with and modify the Document Object Model (DOM) of a web page using scripting languages like JavaScript. This allows developers to dynamically update, add, or remove elements and content on a web page without requiring a full page refresh.

## Anatomy of DOM Manipulation

DOM manipulation involves the following key components:

1. **Selection:**

   Choosing specific elements from the DOM using methods like `getElementById`, `querySelector`, `getElementsByClassName`, or `getElementsByTagName`.

2. **Modification:**

   Changing the content, attributes, styles, or structure of selected elements using methods like `textContent`, `setAttribute`, `classList`, and more.

3. **Creation:**

   Dynamically creating new elements using methods like `createElement`, and then adding them to the DOM using methods like `appendChild` or `insertBefore`.

4. **Removal:**

   Removing elements from the DOM using methods like `removeChild` or `remove`.

5. **Event Handling:**

   Attaching event listeners to DOM elements to respond to user interactions like clicks, input, and more.

## DOM Method

A DOM method is a function provided by the Document Object Model (DOM) API that allows developers to perform specific actions on DOM elements or the document itself. These methods are used to manipulate the structure, content, and behavior of web pages dynamically.

| Category             | DOM Method            | Description                                                                                                                                                                                           |
| -------------------- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DOM Selection        | `getElementById`      | Retrieves an element by its unique ID attribute.                                                                                                                                                      |
|                      | `querySelector`       | Returns the first element that matches a given CSS selector.                                                                                                                                          |
|                      |                       |                                                                                                                                                                                                       |
| DOM Creation         | `createElement`       | Creates a new HTML element.                                                                                                                                                                           |
|                      |                       |                                                                                                                                                                                                       |
| DOM Modification     | `appendChild`         | Appends a child element to a parent element.                                                                                                                                                          |
|                      | `removeChild`         | Removes a child element from a parent element.                                                                                                                                                        |
|                      | `replaceChild`        | Replaces a child element in a parent element with another element.                                                                                                                                    |
|                      | `setAttribute`        | Sets the value of an attribute on a DOM element.                                                                                                                                                      |
|                      | `removeAttribute`     | Removes an attribute from a DOM element.                                                                                                                                                              |
|                      | `getAttribute`        | Retrieves the value of a specific attribute on a DOM element.                                                                                                                                         |
|                      | `insertBefore`        | Inserts a node before a specific child node within a parent element.                                                                                                                                  |
|                      | `.toggle()` (Concept) | Toggles the state or properties of an element, often using JavaScript and CSS.                                                                                                                        |
|                      | `append`              | Adds specified content or elements as the last child of a parent element.                                                                                                                             |
|                      | `prepend`             | Adds specified content or elements as the first child of a parent element.                                                                                                                            |
|                      |                       |                                                                                                                                                                                                       |
| DOM Event Handling   | `addEventListener`    | Attaches an event handler function to an element, allowing it to respond to specific events like clicks.                                                                                              |
|                      | `removeEventListener` | Removes an event handler that has been attached using `addEventListener`.                                                                                                                             |
|                      | `dispatchEvent`       | Dispatches an event to an element, triggering any registered event listeners.                                                                                                                         |
| Event Object Methods | `preventDefault()`    | Prevents the default behavior associated with an event, such as preventing a link from being followed or a form from being submitted. This method is typically used within an event handler function. |
|                      | `stopPropagation()`   | Stops the propagation of an event through the DOM hierarchy, preventing parent elements from receiving the same event. This method is also used within an event handler function.                     |

| DOM Navigation | `parentNode` | Returns the parent node of an element. |
| | `childNodes` | Returns a collection of all child nodes of an element. |
| | `firstChild` | Returns the first child node of an element. |
| | `lastChild` | Returns the last child node of an element. |
| | `nextSibling` | Returns the next sibling node of an element. |
| | `previousSibling` | Returns the previous sibling node of an element. |

---

## DOM Properties

DOM properties are values associated with DOM elements that provide information about the element or allow you to set specific attributes, styles, or behaviors.

| DOM Property  | Description                                                                                                                    |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| `textContent` | Represents the visible text content of an element. Can be read and modified.                                                   |
| `innerText`   | Represents the visible text content of an element, but does not return hidden elements. It also respects CSS styling.          |
| `innerHTML`   | Represents the HTML content within an element. Can be read and modified, but be cautious about security risks when setting it. |
| `className`   | Represents the CSS class attribute of an element. Can be used to change or add classes to an element.                          |
| `style`       | Represents the inline style of an element. Allows you to get or set individual CSS properties directly.                        |
| `classList`   | Represents a list of classes on an element. Provides methods to manipulate classes, like `add`, `remove`, and `toggle`.        |

> DOM manipulation is a core aspect of building dynamic and interactive web applications, enabling developers to create seamless user experiences by updating the content and appearance of web pages in response to user actions or other events.

---

## Event Handling

Event handling involves using event listeners to create interactivity in web pages. An event listener is a function that "listens" for specific events on a DOM element and responds to those events with predefined actions. Events can include user actions like clicks, input, or changes in the DOM.

### How Event Handling Works

1. **Attaching Event Listeners:**

   Event listeners are attached to DOM elements using the addEventListener method. You specify the type of event you're interested in (e.g., "click," "input," "change") and provide a function that will be executed when the event occurs.

2. **Responding to Events:**

   When the specified event happens, the associated function is executed. This function can contain JavaScript code to perform specific actions or manipulate the DOM in response to the event.

   **Example: Attaching a Click Event Listener**

   ```javascript
   // Attaching a click event listener to a button element
   const myButton = document.getElementById("my-button");

   myButton.addEventListener("click", function () {
     // This function will be executed when the button is clicked
     alert("Button was clicked!");
   });
   ```

   > In this example, the function inside `addEventListener` is the event handler. It listens for a click event on the button with the ID "my-button" and displays an alert when the button is clicked.
   >
   > Event handling is a crucial technique for building interactive web applications. By responding to user actions and events, developers can create dynamic and engaging user experiences.
   >
   > Event handling plays a vital role in creating interactive web applications, allowing developers to respond to user actions and events, thus enhancing user engagement and interaction.

---

## JavaScript Modules

JavaScript modules are a fundamental feature introduced in ECMAScript 6 (ES6) that enable developers to organize and structure their code in a more modular and reusable way. Modules allow you to split your code into smaller, self-contained units, making it easier to manage, maintain, and collaborate on large codebases. They provide encapsulation and control over the visibility of variables, functions, and classes.

### Exporting from Modules

In JavaScript modules, you can export functionalities using the `export` keyword. There are multiple ways to export:

- **Named Exports**: Export specific functions, variables, or classes using the `export` keyword before their declaration.

  ```javascript
  // module.js
  export const myFunction = () => {
    /* ... */
  };
  export const myVariable = 42;
  ```

- **Default Exports**: Export a single main functionality from a module using the `export default` syntax.

  ```javascript
  // mainModule.js
  const mainFunction = () => {
    /* ... */
  };
  export default mainFunction;
  ```

### Importing Modules

Importing functionalities from modules is done using the import keyword. You can import named exports and default exports in different ways:

- **Named Imports**: Import specific functionalities using curly braces `{}`.

  ```javascript
  // anotherModule.js
  import { myFunction, myVariable } from "./module.js";
  ```

- **Default Imports**: Import the default export using any chosen name.

  ```javascript
  // app.js
  import mainFunction from "./mainModule.js";
  ```

- **Combining Named and Default Imports**: You can combine named and default imports in a single statement.

  ```javascript
  import mainFunction, { myFunction, myVariable } from "./combinedModule.js";
  ```

### Renaming Imports and Exports

You can rename imported and exported entities using the as keyword.

   ```javascript
   // renamingModule.js
   export { myFunction as renamedFunction } from './module.js';
   import { renamedFunction as func } from './renamingModule.js';
   ```

### Re-exporting

Modules can also re-export functionalities from other modules, allowing for a clean and consistent interface for consumers.

   ```javascript
   // reExportModule.js
   export { myFunction } from './module.js';
   export { mainFunction } from './mainModule.js';
   ```

### Module Paths

When specifying module paths in import and export statements, you can use relative paths (./, ../) or absolute paths. Node.js and modern browsers support the CommonJS syntax for module resolution.

### CommonJS vs. ES6 Modules
Node.js originally used the CommonJS module system (`require`/`module.exports`). With ES6 modules, JavaScript has a standardized module system that is also supported in modern browsers. ES6 modules offer a more static and predictable structure, whereas CommonJS modules are more dynamic.

### Browser Support
Most modern browsers support ES6 modules. However, older browsers might require transpilation or the use of a module bundler like Webpack to convert ES6 modules into a format they can understand.

JavaScript modules have transformed the way developers organize and structure their code. They promote better code organization, reusability, and encapsulation, making it easier to develop and maintain complex applications.

Remember to check the latest browser compatibility information and development practices for the most up-to-date information on using JavaScript modules effectively.