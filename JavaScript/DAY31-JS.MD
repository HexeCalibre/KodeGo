# JAVASCRIPT Introduction 07/04/2023

---

## Contents

[What is JavaScript]()

[History of JavaScript]()

[How JavaScript Works?]()

[Prerequisite]()

[JavaScript Environments]()

[Getting Started]()

[JavaScript Output]()

[]()
## What is JavaScript?
JavaScript is a high-level, interpreted programming language used primarily for front-end web development. It enables interactive and dynamic elements on websites, making them more user-friendly and engaging. JavaScript is supported by all major web browsers and can also be used on the server-side through platforms like Node.js.

## History of JavaScript

JavaScript was created by Brendan Eich in just 10 days while he was working at Netscape Communications Corporation in 1995. Initially named "Mocha," it was later renamed "LiveScript" and finally "JavaScript" to capitalize on the popularity of Java at that time. JavaScript was released as a part of Netscape Navigator 2.0 and quickly became popular among web developers.

## How JavaScript Works

JavaScript is executed in the web browser, enabling it to interact with the Document Object Model (DOM) and manipulate HTML and CSS elements dynamically. It is also capable of handling user interactions, making asynchronous requests to servers, and performing complex computations.

## Prerequisite
Before diving into JavaScript, it is beneficial to have a basic understanding of HTML and CSS, as JavaScript often interacts with these technologies to manipulate web pages.

## JavaScript Environments

JavaScript can run in various environments, including:

1. **Web Browsers**: JavaScript is primarily used in web browsers to create dynamic web pages and interactive user interfaces.

2. **Node.js**: Node.js is a runtime environment that allows JavaScript to be executed outside the browser, enabling server-side scripting and building server applications.

3. **Mobile Applications**: JavaScript is commonly used in mobile app development with frameworks like React Native and Ionic.

4. **Desktop Applications**: Technologies like Electron enable developers to build desktop applications using JavaScript, HTML, and CSS.

## Getting Started

```html
<script src=""></script>
```

**> 📝 **Best practice:** to put inside at the end of the `<body>` tag.**

---

HTML `<script>` Attribute

| Attribute | Description                                                                                                                                                                     |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `defer`   | The script will be executed after the HTML document has been fully parsed. Multiple scripts with the defer attribute will maintain their execution order.                       |
| `async`   | The script will be fetched asynchronously while continuing to parse the HTML document. The script will be executed immediately after it is downloaded, regardless of the order. |

![defer illustration]()

![async illustration]()

---
### JavaScript Output

| Method          | Description                                                                                    | Syntax                             |
| --------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------- |
| `alert`         | Displays an alert dialog box with a message.                                                   | `alert("Hello World!");`           |
| `console.log`   | Logs a message to the browser's console for debugging purposes.                                | `console.log("Hello World!");`     |
| `console.warn`  | Logs a warning message to the console.                                                         | `console.warn("warning message");` |
| `console.debug` | Logs a debug message to the console.                                                           | `console.debug("debug message");`  |
| `console.dir`   | Displays an interactive list of the properties of a specified JavaScript object in the console | `console.dir();`                   |
| `console.error` | Logs an error message to the console.                                                          | `console.error("error message");`  |

---
## JavaScript Statements
In JavaScript, statements are individual instructions or commands that perform actions or computations. Each statement is terminated by a semicolon (;) to separate it from other statements. Here are some common types of JavaScript statements:

   1. Variable Declaration:
   ```javascript
   let name = "John";
   const age = 30;
   var count = 0; // 'var' is an older way to declare variables, 'let' and 'const' are preferred.
   ```
   2. Assignment Statement:
   ```javascript
   name = "Jane";
   age = 35; // Error: You can't reassign a value to a constant (const).
   ```
   3. Conditional Statements:
   ```javascript
   if (age >= 18) {
  console.log("You are an adult.");
   } else {
  console.log("You are a minor.");
  }
   ```
   4. Loops & Iterations:
   ```javascript
   for (let i = 0; i < 5; i++) {
  console.log("Iteration:", i);
  }

  let j = 0;
  while (j < 5) {
  console.log("Iteration:", j);
  j++;
  }
  ```
  5. Function Declaration and Invocation:
  ```javascript
  function greet(name) {
  console.log("Hello, " + name + "!");
  }
  greet("Alice");
  ```
  6. Return Statement:
  ```javascript
  function add(a, b) {
  return a + b;
  }

  const result = add(5, 3); // result will be 8
  ```
  7. Class Declaration and Constructor:
  ```javascript
  class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
   }
  }

  const person1 = new Person("John", 30);
  person1.greet();
  ```
  8. Exception Handling:
  ```javascript
  try {
  // Some code that might throw an error
  throw new Error("Something went wrong!");
  } catch (error) {
  console.error("Error:", error.message);
  } finally {
  console.log("This will always be executed.");
  }
  ```
  >These examples represent common JavaScript statements used for various programming tasks. Markdown format allows you to present code blocks with syntax highlighting and proper formatting, making it easier to read and understand code snippets.
---
### Data Types
In JavaScript, values are the fundamental data types that represent different kinds of information. JavaScript has several built-in value types, and each value belongs to a specific type. Here are the main JavaScript value types:

| Value Type | Example                       | Description                                      |
| ---------- | ----------------------------- | ------------------------------------------------ |
| Numbers    | `let age = 30;`               | Numeric values representing integers and floats. |
| Strings    | `let name = "John";`          | Sequence of characters enclosed in quotes.       |
| Booleans   | `let isAdult = true;`         | Represents true or false values.                 |
| null       | `let noValue = null;`         | Represents the intentional absence of any value. |
| undefined  | `let notAssigned;`            | Represents a declared variable without a value.  |
| Objects    | `let person = { ... };`       | Collection of key-value pairs.                   |
| Arrays     | `let numbers = [...];`        | Ordered collections of values.                   |
| Functions  | `function add(a, b) { ... }`  | A type of object that performs a specific task.  |
| Symbols    | `const symbolKey = Symbol();` | Unique and immutable values.                     |
---
### Primitive Literals

In JavaScript, primitive literals allow us to represent fixed values of the five primitive data types directly in our code. These literals provide a convenient way to define and work with simple data without the need for explicit constructor functions. Here are the five types of primitive literals in JavaScript:

#### 1. String Literal

String literals are used to represent textual data and are enclosed in either single or double quotes.

Example:

```javascript
const name = "John";
const message = 'Hello, world!';
```
#### 2. Numeric Literal
Numeric literal can be written as integers (`int`) or floating point numbers(`float`).
Numeric literals are used to represent numbers, including integers and floating-point numbers.

Example:
```javascript
const age = 30;
const pi = 3.14159;
```
#### 3. Boolean Literal
Boolean values are represented by keywords such as true/false that have no value associated with them like.
Boolean literals represent Boolean values, which can be either `true` or `false`.

Example :
```javascript
const isLogged = true;
const hasPermission = false;
```
#### 4. Undefined Literal
The undefined keyword represents an unknown variable state where it doesn't hold any value at all. It
is often used when we want to declare variables but not assign anything yet. The undefined literal represents the primitive value undefined, indicating the absence of a value.

Example:
```javascript
let value; // value is undefined
```
#### 5. Null Literal
Null is the only primitive type that does not contain any value. The null keyword represents this empty
state of variables holding nothingness. The null literal represents the primitive value `null`, often used to indicate the intentional absence of a value.

Example:
```javascript
const user = null; //No user data available
```
>Understanding primitive literals is essential for working with JavaScript's basic data types and creating simple data structures in your code. These literals serve as the foundation for more complex data structures and objects in the language.
---
### Variables

| Attribute | Description                                                                                           |
| --------- | ----------------------------------------------------------------------------------------------------- |
| `var`     | The old way of declaring variables. It has a function scope and can lead to some unexpected behavior. |
| `let`     | Introduced in ES6, it has block scope and is preferred over var in modern JavaScript.                 |
| `const`   | Also introduced in ES6, it creates a constant whose value cannot be changed after initialization.     |

When to use `var`, `let`, or `const`?

> 1. Always declare variables
> 2. Always use `const` if the value should not be changed
> 3. Always use `const` if the type should not be changed (Arrays and Objects)
> 4. Only use `let` if you can't use const
> 5. Only use `var` if you MUST support old browsers.

Note: Variables are containers for storing values.

---
### Operators
In JavaScript, operators are symbols or keywords that perform various operations on values or variables. They allow you to manipulate data, perform mathematical calculations, make comparisons, and control program flow. Here are some of the most commonly used operators in JavaScript:

- Arithmetic Operators
  
  Arithmetic operators perform mathematical calculations:
```javascript
let a = 5;
let b = 2;

a + b; // Addition: 7
a - b; // Subtraction: 3
a * b; // Multiplication: 10
a / b; // Division: 2.5
a % b; // Modulus (remainder of division): 1
a ** b; // Exponentiation: 25
```
- Relational Operators

  Relational operators compare two values and return a boolean result:
```javascript
let x = 5;
let y = 10;

x == y; // Equal to: false
x != y; // Not equal to: true
x === "5"; // Strict equal to: false (value and type must be the same)
x !== "5"; // Strict not equal to: true (value or type is different)
x > y; // Greater than: false
x < y; // Less than: true
x >= 5; // Greater than or equal to: true
y <= 10; // Less than or equal to: true
```
- Logical Operators

  Logical operators perform logical operations and return a boolean value:
```javascript
let p = true;
let q = false;

p && q; // Logical AND: false
p || q; // Logical OR: true
!p; // Logical NOT: false
!q; // Logical NOT: true
```
- Assignment Operators

  Assignment operators assign values to variables:
```javascript
let num = 5;

num += 2; // Addition assignment: num is now 7
num -= 3; // Subtraction assignment: num is now 4
num *= 2; // Multiplication assignment: num is now 8
num /= 4; // Division assignment: num is now 2
num %= 2; // Modulus assignment: num is now 0
```
- Increment and Decrement Operators
  
  Increment and decrement operators change the value of a variable by 1:
```javascript
let counter = 0;

counter++; // Increment: counter is now 1
counter--; // Decrement: counter is now 0
```
- Unary Operators
  
  Unary operators take a single operand and perform an operation on it:
```javascript
let value = 10;

-value; // Negation: -10
+value; // Unary plus: 10 (Note: Does not change the value)
!value; // Logical NOT: false (Note: Converts the value to a boolean and negates it)
++value; // Prefix increment: 11 (Note: Changes the value and returns the updated value)
value++; // Postfix increment: 11 (Note: Returns the original value and then changes it)
--value; // Prefix decrement: 9 (Note: Changes the value and returns the updated value)
value--; // Postfix decrement: 9 (Note: Returns the original value and then changes it)
```
- Bitwise Operators
```javascript
let a = 5; // Binary representation: 00000000000000000000000000000101
let b = 3; // Binary representation: 00000000000000000000000000000011

a & b; // Bitwise AND: 00000000000000000000000000000001 (1 in decimal)
a | b; // Bitwise OR: 00000000000000000000000000000111 (7 in decimal)
a ^ b; // Bitwise XOR: 00000000000000000000000000000110 (6 in decimal)
~a; // Bitwise NOT: 11111111111111111111111111111010 (-6 in decimal)
a << 1; // Left shift by 1: 00000000000000000000000000001010 (10 in decimal)
a >> 1; // Right shift by 1: 00000000000000000000000000000010 (2 in decimal)
a >>> 1; // Zero-fill right shift by 1: 00000000000000000000000000000010 (2 in decimal)
```
>These operators are essential for writing powerful and expressive JavaScript code. They provide the foundation for performing various operations and implementing complex logic in your programs.
---
## JavaScript Expressions

In JavaScript, an expression is a combination of values, variables, operators, and function calls that results in a single value. Expressions can be as simple as a single value or as complex as a combination of multiple sub-expressions.

### Literal Expressions

- `5` - A literal number expression, evaluates to 5.
- `"Hello"` - A literal string expression, evaluates to "Hello".
- `true` - A literal boolean expression, evaluates to true.
- `null` - A literal null expression, evaluates to null.

### Arithmetic Expressions

- `3 + 7` - Addition expression, evaluates to 10.
- `10 - 5` - Subtraction expression, evaluates to 5.
- `2 * 4` - Multiplication expression, evaluates to 8.
- `10 / 2` - Division expression, evaluates to 5.

### Comparison Expressions

- `5 > 3` - Greater than expression, evaluates to true.
- `10 <= 5` - Less than or equal to expression, evaluates to false.
- `"apple" === "orange"` - Strict equality expression, evaluates to false.

### Logical Expressions

- `true && false` - Logical AND expression, evaluates to false.
- `true || false` - Logical OR expression, evaluates to true.
- `!true` - Logical NOT expression, evaluates to false.

### Variable Expressions

```javascript
let x = 10;
x + 5 // Evaluates to 15, using the value of variable x
```

### Function Call Expressions
```javascript
function add(a, b) {
  return a + b;
}

add(3, 7) // Function call expression, evaluates to 10
```

### Conditional (Ternary) Expression
```javascript
let age = 25;
let message = age >= 18 ? "Adult" : "Minor"; // Evaluates to "Adult"
```

### Array and Object Access Expressions
```javascript
let numbers = [1, 2, 3, 4];
numbers[2] // Accessing array element, evaluates to 3

let person = { name: "John", age: 30 };
person.name // Accessing object property, evaluates to "John"
```
>Expressions are an essential part of JavaScript programming as they allow you to perform computations, make decisions, and produce dynamic values. They are used extensively in conditionals, loops, and function calls to create complex logic and functionality.
---
## JavaScript Keywords

In JavaScript, keywords are reserved words that have special meanings in the language. They cannot be used as identifiers (variable names, function names, etc.) as they are already predefined for specific purposes in JavaScript.

| Keywords    | Description                                                                  |
| ----------- | ---------------------------------------------------------------------------- |
| `abstract`  | Reserved for future use.                                                     |
| `arguments` | Represents the arguments passed to a function.                               |
| `await`     | Used to pause the execution of an async function.                            |
| `boolean`   | Represents a boolean value (true or false).                                  |
| `break`     | Exits from a loop or a switch statement.                                     |
| ...         | ...                                                                          |
| `while`     | Starts a while loop that executes a block of code while a condition is true. |
| `with`      | Specifies a default object for a block of code.                              |
| `yield`     | Pauses and resumes the execution of a generator function.                    |

---
### Comment
In JavaScript, comments can be added to provide explanatory notes within the code. Single-line comments start with //, while multi-line comments are enclosed between /* and */.
```javascript
// This is single line comment
/* This
is multiline comments
*/
```

#### Comment Guidelines

Comments in code serve as important explanatory notes and aid in understanding the codebase. Well-written comments can make the code more maintainable and help other developers comprehend the purpose and functionality of different code segments. Follow these guidelines to write effective and useful comments:

1. **Be Clear and Concise:** Write comments that are easy to understand and get straight to the point. Avoid unnecessary elaboration or ambiguity.

2. **Explain Intent:** Describe the purpose and intention of the code. Why is the code doing what it does? This helps others understand the rationale behind specific decisions.

3. **Avoid Obvious Comments:** Avoid commenting on self-explanatory code. Comments should add value by providing insights that are not apparent from the code itself.

4. **Use Proper Grammar and Spelling:** Keep comments grammatically correct and spell-checked. Poorly written comments can be confusing and unprofessional.

5. **Update Comments with Code Changes:** Ensure that comments are updated whenever the corresponding code changes. Outdated comments can lead to confusion.

6. **Keep Comments Updated and Relevant:** As the code evolves, make sure to review and update comments to reflect the current state of the codebase.

7. **Use Meaningful Variable Names:** Instead of explaining variables in comments, use descriptive names that convey their purpose.

8. **Comment Complex Logic:** Comment complex algorithms or logic to make it easier for others to grasp the reasoning behind the implementation.

9. **Avoid Commenting Trivial Steps:** Only comment when necessary. Trivial steps may clutter the code unnecessarily.

10. **Consider Future Readers:** Write comments as if you are explaining the code to someone who is not familiar with it.

11. **Use Proper Comment Formats:** Depending on the programming language, follow appropriate comment formats (e.g., `//` for single-line comments, `/* */` for multi-line comments).

12. **Avoid Leaving Debug Comments:** Remove or comment out debug statements before committing the code.

13. **Comment on Non-Obvious Workarounds:** If the code includes workarounds or non-standard solutions, explain the reasoning behind them.

14. **Group Related Code Blocks:** Commenting can help group and organize related sections of code.

15. **Be Respectful and Professional:** Avoid negative or offensive language in comments. Maintain a professional tone.

Remember, comments are for humans, not the computer. They should provide valuable insights, simplify understanding, and make collaboration easier for everyone involved in the project.

---
## JavaScript Identifiers / Names

In JavaScript, identifiers are used to name variables, functions, classes, and other entities in the code. An identifier is a sequence of characters that must follow certain rules and conventions. Here are the main rules for creating valid JavaScript identifiers:

1. The first character must be a letter (a-z or A-Z), an underscore (_), or a dollar sign ($). It cannot start with a digit (0-9).

2. After the first character, an identifier can include letters, digits, underscores, or dollar signs.

3. Identifiers are case-sensitive, meaning that `myVar`, `MyVar`, and `MYVAR` are considered different identifiers.

4. Reserved words (keywords) cannot be used as identifiers. For example, you cannot use `if`, `for`, `function`, etc., as identifiers.

5. JavaScript allows Unicode characters and Unicode escape sequences in identifiers.

### Examples of valid JavaScript identifiers:

- `firstName`
- `_userName`
- `$age`
- `hello123`
- `π`

### Examples of invalid JavaScript identifiers:

- `123abc` (Starts with a digit)
- `if` (Reserved keyword)
- `first-name` (Contains a hyphen - hyphens are not allowed in identifiers)

>It is essential to choose meaningful and descriptive names for identifiers to improve code readability and maintainability. Good naming practices contribute to writing clean and maintainable JavaScript code.

---

## JavaScript Best Practices

Best practices in JavaScript are guidelines and coding conventions that help improve code quality, maintainability, and performance. Following these practices ensures that your JavaScript code is more readable, less error-prone, and easier to maintain. Here are some of the most important JavaScript best practices:

1. Use Descriptive Naming: Choose meaningful and descriptive names for variables, functions, and classes. This makes your code self-explanatory and easier to understand.

2. Declare Variables Properly: Always declare variables using `let` or `const` to avoid unintentional global scope issues. Minimize the use of `var`, as it has function scope and can lead to unexpected behavior.

3. Avoid Global Variables: Minimize the use of global variables, as they can lead to naming conflicts and make it difficult to track changes. Prefer encapsulating variables within functions or modules.

4. Use Strict Mode: Enable strict mode (`"use strict";`) at the beginning of your script or function to catch errors and enforce more stringent rules for writing JavaScript.

5. Use `const` for Constants: Use `const` to declare variables that should not be reassigned after their initial value. This helps prevent accidental reassignments and enhances code predictability.

6. Prefer Arrow Functions: Use arrow functions (`() => {}`) for concise function expressions. They provide a more compact syntax and capture the surrounding `this` context automatically.

7. Avoid Global Namespace Pollution: Avoid polluting the global namespace with unnecessary functions and objects. Prefer using modules and namespaces to organize your code.

8. Embrace Promises or Async/Await: Use Promises or Async/Await for handling asynchronous operations to improve code readability and handle errors more effectively.

9. Proper Error Handling: Always handle errors properly using `try...catch` blocks or Promise `.catch()` to prevent unhandled exceptions and provide meaningful error messages.

10. Optimize Loops: Optimize loops by reducing unnecessary computations and avoiding excessive function calls inside loops to improve performance.

11. Use Template Literals: Use template literals (backticks) for concatenating strings and embedding expressions. This improves readability and simplifies string formatting.

12. Comment Your Code: Add comments to your code to explain complex logic, algorithms, or tricky parts. Good comments help other developers (including yourself) understand the code better.

13. Test Your Code: Write automated tests for your JavaScript code using testing frameworks like Jest or Mocha to ensure its correctness and catch bugs early.

14. Optimize Performance: Pay attention to performance-critical code and use techniques like memoization, debouncing, and throttling when dealing with expensive operations.

15. Stay Updated: Keep up with the latest ECMAScript features and browser support to leverage new language improvements and optimize compatibility.

>By following these best practices, you can write clean, efficient, and maintainable JavaScript code that is easier to work with and less prone to bugs and errors.

---
### String Manipulation

1. Old Style Concatination
```javascript
var firstName = "John";
var lastName = "Doe";
var fullName = firstName + " " + lastName; 
// Result: "John Doe"
```
Old-style concatenation involves using the + operator to join strings together. It was the traditional way to build strings in older versions of JavaScript.

Use old-style concatenation when:

You are working with older JavaScript environments that do not support string interpolation (e.g., ES5 or below).
You are building strings using variables that are not supported inside template literals (backticks).


2. String Interpolation
```javascript
var firstName = "John";
var lastName = "Doe";
var fullName = `${firstName} ${lastName}`; 
// Result: "John Doe"
```

String interpolation was introduced in ECMAScript 6 (ES6) using backticks (```). It allows embedding expressions (variables, functions, etc.) directly within the string using ${...} placeholders.

Use string interpolation when:

You are working with modern JavaScript environments (ES6 and above).
You want to make the code more readable and maintainable by avoiding the need for complex concatenation.
You have multiple variables or expressions to include within the string, making the code cleaner and easier to understand.
String interpolation is generally preferred over old-style concatenation because it offers cleaner syntax and makes the code more expressive. However, if you are dealing with older JavaScript environments or need to concatenate strings with complex expressions, old-style concatenation might be the only viable option. In modern JavaScript projects, string interpolation is the recommended approach for string manipulation.

---
### String method

| Method                                  | Description                                                                                                                                                                                                             |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `length`                                | Returns the length (number of characters) of a string.                                                                                                                                                                  |
| `charAt(index)`                         | Returns the character at the specified index in the string.                                                                                                                                                             |
| `indexOf(searchValue[, fromIndex])`     | Returns the index of the first occurrence of searchValue in the string, starting from the optional fromIndex. If not found, it returns -1.                                                                              |
| `lastIndexOf(searchValue[, fromIndex])` | Returns the index of the last occurrence of searchValue in the string, starting from the optional fromIndex. If not found, it returns -1.                                                                               |
| `slice(start[, end])`                   | Extracts a portion of the string starting from start index to end index (exclusive). If end is omitted, it extracts until the end of the string. Negative indices can also be used to count from the end of the string. |
| `concat(str1, str2, ..., strN)`         | Concatenates one or more strings with the original string and returns the resulting string.                                                                                                                             |
| `replace(searchValue, replaceValue)`    | Replaces occurrences of searchValue with replaceValue in the string. Only the first occurrence is replaced unless using a regular expression with the g flag.                                                           |
| `replaceAll()`                          | Replaces all occurrences of searchValue with replaceValue in the string. This method was introduced in ECMAScript 2021 (ES12).                                                                                          |
| `toLowerCase)`                          | Converts all characters in the string to lowercase.                                                                                                                                                                     |
| `toUpperCase)`                          | Converts all characters in the string to uppercase.                                                                                                                                                                     |

---

### Arrays
An array is a fundamental data structure in JavaScript used to store a collection of elements. It allows you to organize and work with multiple values in a single variable. Arrays in JavaScript can hold a mix of data types, including numbers, strings, objects, and even other arrays. They are versatile and widely used in JavaScript programming. Here's how you define and work with arrays:

1. Array Creation:
   
You can create an array using square brackets [] and adding elements separated by commas:
```javascript
// Creating an array with numbers
const numbers = [1, 2, 3, 4, 5];

// Creating an array with strings
const fruits = ['apple', 'banana', 'orange'];

// Creating an array with a mix of data types
const mixedArray = [1, 'hello', true, { key: 'value' }];
```

2. Accessing Array Elements:

You can access individual elements of an array using their index. The index starts at 0 for the first element, 1 for the second, and so on:
```javascript
const numbers = [10, 20, 30];

console.log(numbers[0]); // Output: 10
console.log(numbers[1]); // Output: 20
console.log(numbers[2]); // Output: 30

```

3. Modifying Array Elements:
   
You can modify array elements by assigning new values to the specific index:
```javascript
let fruits = ['apple', 'banana', 'orange'];

fruits[1] = 'grape';
console.log(fruits); // Output: ['apple', 'grape', 'orange']
```
4. Array Methods:
   
Arrays come with various built-in methods that allow you to manipulate their contents:

- `join(separator)`

The `join()` method converts all the elements of an array into a string and concatenates them using the specified `separator`. It returns the resulting string. The `separator` is optional, and if not provided, the elements are concatenated with a comma as the default separator.

  Example
  ```javascript
  const fruits = ['apple', 'banana', 'orange'];

   const joinedString = fruits.join(', ');
   console.log(joinedString); // Output: "apple, banana, orange"
  ```
- `splice(start, deleteCount, item1, item2, ...)`

The `splice()` method allows you to modify an array by adding or removing elements. It takes three parameters:

   - `start`: The index at which to start changing the array.

   - `deleteCount`: The number of elements to remove starting from the start index. If set to 0, no elements are removed.

   - `item1, item2, ...`: Elements to add to the array starting from the start index.

      Example

      ```javascript
      const numbers = [1, 2, 3, 4, 5];

      // Removing elements from the array (deleteCount > 0)
      numbers.splice(2, 2); // Removes 3 and 4
      console.log(numbers); // Output: [1, 2, 5]

      // Adding elements to the array (deleteCount = 0)
      numbers.splice(2, 0, 3, 4); // Inserts 3 and 4 at index 2
      console.log(numbers); // Output: [1, 2, 3, 4, 5]
      ```

- `split(separator[, limit])`

  The `split()` method splits a string into an array of substrings based on the specified `separator`. The resulting array elements will be the parts of the original string separated by the `separator`. The `limit` parameter is optional and represents the maximum number of splits to be performed.

   Example

  ```javascript
      const sentence = 'Hello, how are you?';

      const words = sentence.split(' '); // Split by space
      console.log(words); // Output: ['Hello,', 'how', 'are', 'you?']

      const letters = sentence.split(''); // Split by each character
      console.log(letters); // Output: ['H', 'e', 'l', 'l', 'o', ',', ' ', 'h', 'o', 'w', ' ', 'a', 'r', 'e', ' ', 'y', 'o', 'u', '?']
  ```
- `reverse()`

   The `reverse()` method reverses the order of elements in an array, modifying the original array.

    Example

    ```javascript
       const numbers = [1, 2, 3, 4, 5];

       numbers.reverse();
       console.log(numbers); // Output: [5, 4, 3, 2, 1]
    ```
- `shift()`

   The `shift()` method removes the first element from the array and returns that removed element. The length of the array is decreased by 1.

   Example

   ```javascript
  const fruits = ['apple', 'banana', 'orange'];

  const firstFruit = fruits.shift();
  console.log(firstFruit); // Output: "apple"
  console.log(fruits); // Output: ["banana", "orange"]
  ```

- `unshift(item1, item2, ...)`

   The `unshift()` method adds one or more elements to the beginning of the array and returns the new length of the array.

  Example
    
  ```javascript
  const numbers = [2, 3, 4, 5];

  const newLength = numbers.unshift(1);
  console.log(newLength); // Output: 5 (new length of the array)
  ```

- `push(element1, element2, ...)`

   The `push()` method adds one or more elements to the end of an array and returns the new length of the array. It modifies the original array by adding the elements provided as arguments to the end of the array.

   Example

   ```javascript
   const fruits = ['apple', 'banana'];

   const newLength = fruits.push('orange', 'grape');
   console.log(newLength); // Output: 4 (new length of the array)
   console.log(fruits); // Output: ['apple', 'banana', 'orange', 'grape']
   ```
- `pop()`

   The `pop()` method removes the last element from an array and returns that element. It modifies the original array by removing the last element.

   Example

   ```javascript
   const numbers = [1, 2, 3, 4, 5];

   const removedElement = numbers.pop();
   console.log(removedElement); // Output: 5 (removed element)
   console.log(numbers); // Output: [1, 2, 3, 4]
   ```
- `slice(start, end)`

   The `slice()` method extracts a section of an array and returns a new array containing the extracted elements. It takes two parameters:
   - `start`: The index at which to start the extraction. If start is negative, it counts from the end of the array.
   - `end`: The index before which to end the extraction. If end is negative, it counts from the end of the array. If end is omitted, the slice includes all elements from start to the end of the array.

   Example

   ```javascript
   const fruits = ['apple', 'banana', 'orange', 'grape', 'kiwi'];

   const slicedFruits = fruits.slice(1, 4);
   console.log(slicedFruits); // Output: ['banana', 'orange', 'grape']
   ```

- `Array.isArray()`

   `Array.isArray()` is a built-in function in JavaScript used to check whether a given value is an array or not. It returns `true` if the value is an array and `false` if it is not.

   Example

  ```javascript
  const myArray = [1, 2, 3];
  const myObject = { key: "value" };
  const myString = "Hello, world!";

  console.log(Array.isArray(myArray)); // Output: true
  console.log(Array.isArray(myObject)); // Output: false
  console.log(Array.isArray(myString)); // Output: false
  ```

- `map(callbackFn)`

   The `map()` method is used to create a new array by applying a callback function to each element of the original array. The callback function takes three arguments: the current element being processed, the index of that element, and the array itself. It then returns a new value, which will be added to the new array.

   Example

   ```javascript
   const numbers = [1, 2, 3, 4, 5];

   const squaredNumbers = numbers.map((number) => number * number);
   console.log(s
   ```

- `filter(callback(element[, index[, array]])[, thisArg])`
  
  The `filter()` method creates a new array with all elements that pass the test implemented by the provided callback function. The callback function is called for each element in the array, and if it returns `true`, the element is included in the new filtered array. If it returns `false`, the element is excluded.
  
  - `callback`: The function used to test each element of the array. It takes three arguments:

    Parameters:
    
    - `element`: The current element being processed in the array.
    - `index` (optional): The index of the current element in the array.
    - `array` (optional): The array that the `filter()` method was called upon.

  - `thisArg` (optional): The value to be used as `this` when executing the callback function.

  Return Value:

  - A new array containing all the elements for which the callback function returns `true`.

       Example:

      ```javascript
      const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    // Filter out even numbers
    const evenNumbers = numbers.filter((number) => number % 2 === 0);

    console.log(evenNumbers); // Output: [2, 4, 6, 8, 10]
    ```

> These are just a few examples of array methods; there are many more available for sorting, filtering, mapping, and more. Arrays provide a powerful way to work with collections of data in JavaScript.
---
### Conditional Statement
A conditional statement, also known as a conditional expression or conditional construct, is a programming concept that allows you to make decisions in your code based on certain conditions. It enables you to execute different blocks of code or take specific actions depending on whether a condition evaluates to true or false.

In JavaScript, there are several ways to implement conditional statements:

- `if` Statement:
  
  The `if` statement is the simplest conditional statement. It executes a block of code only if the specified condition is true.
  
```javascript
let num = 10;

if (num > 0) {
console.log("The number is positive.");
```

- `if-else` Statement:
  
  The `if-else` statement allows you to execute one block of code if the condition is true, and another block of code if the condition is false.

```javascript
let num = -5;

if (num > 0) {
  console.log("The number is positive.");
} else {
  console.log("The number is non-positive.");
}
```

- `if-else if-else` Statement:
  
  The `if-else if-else` statement allows you to test multiple conditions and execute different blocks of code based on which condition is true first.

```javascript
let num = 0;

if (num > 0) {
  console.log("The number is positive.");
} else if (num < 0) {
  console.log("The number is negative.");
} else {
  console.log("The number is zero.");
}
```

- `switch` Statement:

   The `switch` statement provides an alternative way to handle multiple conditions based on the value of an expression.

```javascript
let day = "Monday";

switch (day) {
  case "Monday":
    console.log("It's the start of the week.");
    break;
  case "Friday":
    console.log("It's the end of the week.");
    break;
  default:
    console.log("It's a regular day.");
    break;
}
```
Conditional statements are essential for implementing logic and making your programs responsive to different situations. They allow you to control the flow of execution and ensure that your code behaves as expected in various scenarios.
---
### Loops
Loops in JavaScript allow you to execute a block of code repeatedly until a certain condition is met. They are essential for performing repetitive tasks efficiently. JavaScript supports several types of loops:

1. `for` Loop

The `for` loop is one of the most commonly used loops in JavaScript. It allows you to execute a block of code for a specific number of iterations.
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```
2. `while` Loop

The `while` loop executes a block of code as long as a specified condition is true.
```javascript
let count = 0;

while (count < 5) {
  console.log(count);
  count++;
}
```
3. `do-while` Loop

The `do-while` loop is similar to the `while` loop, but it executes the block of code at least once before checking the condition.

```javascript
let number = 1;

do {
  console.log(number);
  number++;
} while (number <= 5);
```

4. `for-in` Loop

The `for-in` loop is used to iterate over the properties of an object.
```javascript
const person = {
  name: 'John',
  age: 30,
  occupation: 'Engineer',
};

for (const key in person) {
  console.log(key + ': ' + person[key]);
}
```
5. `for-of` Loop

The `for-of` loop is introduced in ES6 and is used to iterate over iterable objects like arrays and strings.
```javascript
const colors = ['red', 'green', 'blue'];

for (const color of colors) {
  console.log(color);
}
```
6. `forEach` Loop
   
   The forEach loop is inserted after the previous loops, and it iterates through the myArray and logs each element to the console, just like the other loops. It provides a convenient way to iterate through array elements without the need for explicitly managing the index.
   ```javascript
   // Sample array
   const myArray = [1, 2, 3, 4, 5];

   // Using forEach loop to iterate through the array
   console.log("Using forEach loop:");
   myArray.forEach((element) => {
   console.log(element);
   });

   // forEach Named Function
   function logCar(car) {
    console.log(car.model);
   }

   myCars.forEach(logCar);

   // forEach Anonymous function
   myCars.forEach(function (car) {
    console.log(car.model);
   })
   ```

7. Looping Through Arrays
   
   Looping through arrays is a common use case for many programming tasks. Here's an example of how you can do it in JavaScript:

```javascript
// Sample array
const myArray = [1, 2, 3, 4, 5];

// Using for loop to iterate through the array
console.log("Using for loop:");
for (let i = 0; i < myArray.length; i++) {
  console.log(myArray[i]);
}

// Using for...of loop to iterate through the array
console.log("Using for...of loop:");
for (const element of myArray) {
  console.log(element);
}

// Using while loop to iterate through the array
console.log("Using while loop:");
let j = 0;
while (j < myArray.length) {
  console.log(myArray[j]);
  j++;
}

// Using do...while loop to iterate through the array
console.log("Using do...while loop:");
let k = 0;
do {
  console.log(myArray[k]);
  k++;
} while (k < myArray.length);

// Using forEach loop to iterate through the array
console.log("Using forEach loop:");
myArray.forEach((element) => {
  console.log(element);
});
```
>In this example, we have an array `myArray` containing some numbers. We then use different types of loops to iterate over the elements of the array and print them to the console. You can perform any desired operations on the array elements within the loop's body.
>
>Loops are powerful tools for automating repetitive tasks and processing large amounts of data. However, be cautious about using infinite loops that might cause your program to hang or crash. Always ensure that your loop has a proper exit condition to prevent unintended behavior.

### Loop Choices and Use Cases

#### `for` Loop:

- Use when you know the exact number of iterations you need to perform.
- Ideal for looping over a numerical range or a fixed number of times.

#### `while` Loop:

- Use when you want to repeat a block of code based on a condition that might change during the loop.
- Appropriate when the number of iterations is uncertain.

#### `do-while` Loop:

- Similar to the while loop, but the block of code is executed at least once before checking the condition.
- Useful when you want to ensure that the loop runs at least once, regardless of the condition.

#### `for-in` Loop:

- Use when you want to loop through the enumerable properties of an object.
- Suitable for iterating over object properties and performing operations based on each property.

#### `for-of` Loop:

- Introduced in ES6, use when you want to iterate over elements of an iterable object, like arrays or strings.
- Convenient for working with arrays or collections of data.
### Common Scenarios and Loop Usage:

- Use a `for` loop when you know the number of iterations in advance or when you need to loop through an index-based collection.
- Use a `while` loop when you don't know the number of iterations in advance and need to loop based on a specific condition.
- Use a `do-while` loop when you want to execute a block of code at least once before checking the condition.
- Use a `for-in` loop when you want to iterate over the properties of an object.
- Use a `for-of` loop when you want to iterate over elements of an iterable object like an array or a string.

>Keep in mind that improper use of loops or using the wrong loop type can lead to unintended consequences, such as infinite loops or inefficient code. Always choose the loop that best fits the specific requirements of your task and make sure to have proper exit conditions to prevent infinite loops.
---
### Functions
Functions in programming are reusable blocks of code that can be called and executed to perform a specific task or return a value. They allow you to break down your code into smaller, manageable pieces, promoting code organization, modularity, and reusability.

In most programming languages, functions have the following components:

1. Function Declaration/Definition: This is where you create the function and specify its name, parameters (if any), and return type (if any). The function name is used to call the function later in your code.

2. Parameters: Parameters (also known as arguments) are values that you can pass into the function when you call it. Functions can accept zero or more parameters, which act as inputs to the function's logic.

3. Function Body: The function body contains the actual code that gets executed when the function is called. It defines the actions or calculations that the function performs.

4. Return Statement: If a function is expected to produce a result, you can use the `return` statement to send that result back to the code that called the function.

Here's a simple example of a function in JavaScript:
```javascript
// Function declaration with parameters
function addNumbers(a, b) {
  const sum = a + b;
  return sum; // Return the result
}

// Function call with arguments
const result = addNumbers(5, 10);
console.log(result); // Output: 15
```
In this example, we defined a function called `addNumbers` that takes two parameters (`a` and `b`) and returns their sum. When we call the function with `addNumbers(5, 10)`, it returns the result `15`, which is then stored in the variable `result` and printed to the console.

Functions are essential building blocks in programming, as they help modularize code and promote code reusability. They are widely used to encapsulate logic and provide a clear interface for interacting with various parts of the codebase.

#### Function Assignment

In programming, function assignment refers to the technique of assigning functions to variables. In languages that support first-class functions, like JavaScript, Python, and many others, functions are treated as first-class citizens, meaning they can be treated just like any other data type. This allows us to store functions in variables, pass them as arguments to other functions, and return them from functions.

Here's an example in JavaScript:

```javascript
// Define a function
function add(a, b) {
  return a + b;
}

// Save the function in a variable
const myFunction = add;

// Call the function using the variable
const result = myFunction(3, 5); // Result will be 8
```
>In this example, the add function is assigned to the variable myFunction. As a result, we can call the add function using the myFunction variable, passing 3 and 5 as arguments, and store the result in the result variable.
>
>Function assignment is a powerful technique that enables various programming patterns, including functional programming paradigms and higher-order functions. It provides flexibility and reusability in code, allowing developers to design more elegant and efficient solutions to complex problems.


#### Types of Function

1. **Named Functions**: These are traditional functions that have a specific name. They can be defined using the `function` keyword in JavaScript or similar constructs in other programming languages.
```javascript
function addNumbers(a, b) {
  return a + b;
}
```

2. **Anonymous Functions**: These functions do not have a specific name and are often defined using function expressions. They are usually assigned to variables and can be used as callbacks or immediately invoked.
   
```javascript
const myFunction = function (name) {
  console.log(`Hello, ${name}!`);
};
```
3. **Arrow Functions**: Arrow functions are a concise syntax for writing functions in JavaScript. They have a shorter syntax and do not bind their own `this` value.

```javascript
const multiply = (a, b) => a * b;
```
4. **Higher-Order Functions**: These are functions that take one or more functions as arguments or return a function as their result.

```javascript
function executeOperation(operation, a, b) {
  return operation(a, b);
}

const result = executeOperation((x, y) => x + y, 5, 10); // Result will be 15
```

5. **Recursive Functions**: These functions call themselves within their own definition. They are often used to solve problems that can be broken down into smaller subproblems.

```javascript
function factorial(n) {
  if (n === 0) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}
```

6. **Generator Functions**: Generator functions are special functions that can pause their execution and resume it later. They use the yield keyword to `yield` values one at a time.
  
```javascript
function* generateSequence() {
  yield 1;
  yield 2;
  yield 3;
}

const sequence = generateSequence();
console.log(sequence.next().value); // Output: 1
console.log(sequence.next().value); // Output: 2
console.log(sequence.next().value); // Output: 3
```
---
### Parameter Passing Mechanism

In computer programming, the parameter passing mechanism refers to how function arguments are passed to functions during function calls. Different programming languages employ specific rules for this mechanism, which affects how data is handled within functions and how modifications made to function parameters can impact the original values outside the function scope.

In JavaScript, the parameter passing mechanism can be categorized into two main scenarios:

1. **Pass by Value (for Primitive Types):**
   When you pass a primitive data type, such as a number, string, or boolean, as an argument to a function, JavaScript uses a "pass by value" mechanism. This means that a copy of the actual value is passed to the function's parameter. Any changes made to the function's parameter inside the function do not affect the original value outside the function.

   ```javascript
   function modifyValue(val) {
     val = val + 10; // Changes to the parameter val do not affect the original value outside the function
   }

   let num = 5;
   modifyValue(num);
   console.log(num); // Output: 5 (the original value remains unchanged)
   ```

2. **Pass by Reference (Pass by Sharing) for Objects:**
   When you pass an object (including arrays and functions) as an argument to a function, JavaScript uses a "pass by reference" mechanism, or more accurately, "pass by sharing." This means a reference to the original object is passed to the function, not a copy of the object itself. As a result, modifications to the object's properties inside the function affect the original object outside the function.
   ```javascript
   function modifyObject(obj) {
   obj.property = "modified"; // Changes to the object property affect the original object outside the function
   }

   let myObj = { property: "original" };
   modifyObject(myObj);
   console.log(myObj.property); // Output: "modified" (the original object is modified)
   ```
   However, reassigning the object parameter to a new object within the function does not affect the original object outside the function:
   ```javascript
   function reassignObject(obj) {
   obj = { newProperty: "new value" }; // Reassigning the parameter does not affect the original object outside the function
   }

   let myObj = { property: "original" };
   reassignObject(myObj);
   console.log(myObj); // Output: { property: "original" } (the original object remains unchanged)
   ```
   Understanding the parameter passing mechanism is fundamental for working effectively with functions in JavaScript, as it plays a significant role in how data is handled and modified within functions and throughout the program.

