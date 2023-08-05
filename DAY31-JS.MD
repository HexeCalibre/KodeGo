# JAVASCRIPT 07/04/2023

---

## Contents

[What is JavaScript]()

[Prerequisite]()

[How to use?]()

## What is JavaScript?
JavaScript is a high-level, interpreted programming language used primarily for front-end web development. It enables interactive and dynamic elements on websites, making them more user-friendly and engaging. JavaScript is supported by all major web browsers and can also be used on the server-side through platforms like Node.js.

## Prerequisite
Before diving into JavaScript, it is beneficial to have a basic understanding of HTML and CSS, as JavaScript often interacts with these technologies to manipulate web pages.

## How to use?

```html
<script src=""></script>
```

> 📝 **Best practice:** to put inside at the end of the `<body>` tag.

---

HTML `<script>` Attribute

| Attribute | Description |
| --------- | ----------- |
| `defer` |   The script will be executed after the HTML document has been fully parsed. Multiple scripts with the defer attribute will maintain their execution order.          |
| `async` |  The script will be fetched asynchronously while continuing to parse the HTML document. The script will be executed immediately after it is downloaded, regardless of the order.           |

![defer illustration]()

![async illustration]()

---
Declaration
---
### Variables

| Attribute | Description |
| --------- | ----------- |
| `var`   | The old way of declaring variables. It has a function scope and can lead to some unexpected behavior.            |
| `let`   | Introduced in ES6, it has block scope and is preferred over var in modern JavaScript.            |
| `const` | Also introduced in ES6, it creates a constant whose value cannot be changed after initialization.            |

When to use `var`, `let`, or `const`?

> 1. Always declare variables
> 2. Always use `const` if the value should not be changed
> 3. Always use `const` if the type should not be changed (Arrays and Objects)
> 4. Only use `let` if you can't use const
> 5. Only use `var` if you MUST support old browsers.

Note: Variables are containers for storing values.

---
### Data Types


| Data Type | Description |
| --------- | ----------- |
| String    | Represents textual data, e.g., "Hello, World!".            |
| Integer   | Represents whole numbers, e.g., 42.            |
| Float     | Represents decimal numbers, e.g., 3.14.            |
| Boolean   | Represents true or false.            |
| Undefined | Represents a variable that has been declared but not assigned a value.            |
| Null      | Represents the intentional absence of any object value.            |

---
### JavaScript Code

| Method            | Description | Syntax                              |
| ----------------- | ----------- | ------------------------------------ |
| `alert`         |  Displays an alert dialog box with a message.           | `alert("Hello World!");`           |
| `console.log`   | Logs a message to the browser's console for debugging purposes.            | `console.log("Hello World!");`     |
| `console.warn`  | Logs a warning message to the console.            | `console.warn("warning message");` |
| `console.debug` |  Logs a debug message to the console.           | `console.debug("debug message");`  |
| `console.dir`   |  Displays an interactive list of the properties of a specified JavaScript object in the console           | `console.dir();`                   |
| `console.error` |  Logs an error message to the console.           | `console.error("error message");`  |

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

| Method            | Description | 
| ----------------- | ----------- | 
| `length`          | Returns the length (number of characters) of a string. | 
| `charAt(index)`        |Returns the character at the specified index in the string.|
| `indexOf(searchValue[, fromIndex])`|Returns the index of the first occurrence of searchValue in the string, starting from the optional fromIndex. If not found, it returns -1.| 
| `lastIndexOf(searchValue[, fromIndex])`   |Returns the index of the last occurrence of searchValue in the string, starting from the optional fromIndex. If not found, it returns -1.| 
| `slice(start[, end])`         |Extracts a portion of the string starting from start index to end index (exclusive). If end is omitted, it extracts until the end of the string. Negative indices can also be used to count from the end of the string.|
| `concat(str1, str2, ..., strN)`        |Concatenates one or more strings with the original string and returns the resulting string.|
| `replace(searchValue, replaceValue)`       |Replaces occurrences of searchValue with replaceValue in the string. Only the first occurrence is replaced unless using a regular expression with the g flag.|
| `replaceAll()`       |Replaces all occurrences of searchValue with replaceValue in the string. This method was introduced in ECMAScript 2021 (ES12).|
| `toLowerCase)`    |Converts all characters in the string to lowercase.|
| `toUpperCase)`    |Converts all characters in the string to uppercase.|

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
```javascript
const sentence = 'Hello, how are you?';

const words = sentence.split(' '); // Split by space
console.log(words); // Output: ['Hello,', 'how', 'are', 'you?']

const letters = sentence.split(''); // Split by each character
console.log(letters); // Output: ['H', 'e', 'l', 'l', 'o', ',', ' ', 'h', 'o', 'w', ' ', 'a', 'r', 'e', ' ', 'y', 'o', 'u', '?']
```
- `reverse()`
  
The `reverse()` method reverses the order of elements in an array, modifying the original array.
```javascript
const numbers = [1, 2, 3, 4, 5];

numbers.reverse();
console.log(numbers); // Output: [5, 4, 3, 2, 1]
```
- `shift()`
  
The `shift()` method removes the first element from the array and returns that removed element. The length of the array is decreased by 1.

```javascript
const fruits = ['apple', 'banana', 'orange'];

const firstFruit = fruits.shift();
console.log(firstFruit); // Output: "apple"
console.log(fruits); // Output: ["banana", "orange"]
```
- `unshift(item1, item2, ...)`
  
The `unshift()` method adds one or more elements to the beginning of the array and returns the new length of the array.

```javascript
const numbers = [2, 3, 4, 5];

const newLength = numbers.unshift(1);
console.log(newLength); // Output: 5 (new length of the
```

- `push(element1, element2, ...)`
  
The `push()` method adds one or more elements to the end of an array and returns the new length of the array. It modifies the original array by adding the elements provided as arguments to the end of the array.
```javascript
const fruits = ['apple', 'banana'];

const newLength = fruits.push('orange', 'grape');
console.log(newLength); // Output: 4 (new length of the array)
console.log(fruits); // Output: ['apple', 'banana', 'orange', 'grape']
```
In this example, the `push()` method adds two elements, `'orange'` and `'grape'`, to the end of the fruits array, and the array becomes `['apple', 'banana', 'orange', 'grape']`. The `push()` method returns the new length of the array, which in this case is `4`.

- `pop()`
  
The `pop()` method removes the last element from an array and returns that element. It modifies the original array by removing the last element.
```javascript
const numbers = [1, 2, 3, 4, 5];

const removedElement = numbers.pop();
console.log(removedElement); // Output: 5 (removed element)
console.log(numbers); // Output: [1, 2, 3, 4]
```
In this example, the `pop()` method removes the last element `5` from the numbers array, and the array becomes `[1, 2, 3, 4]`. The method also returns the removed element, which in this case is `5`.

- `slice(start, end)`
  
The `slice()` method extracts a section of an array and returns a new array containing the extracted elements. It takes two parameters:

- `start`: The index at which to start the extraction. If `start` is negative, it counts from the end of the array.
- `end`: The index before which to end the extraction. If `end` is negative, it counts from the end of the array. If end is omitted, the slice includes all elements from `start` to the end of the array.

```javascript
const fruits = ['apple', 'banana', 'orange', 'grape', 'kiwi'];

const slicedFruits = fruits.slice(1, 4);
console.log(slicedFruits); // Output: ['banana', 'orange', 'grape']
```
In this example, the `slice(1, 4)` method extracts elements from index `1` (inclusive) to index `4` (exclusive), creating a new array `['banana', 'orange', 'grape']` from the `fruits` array. The original `fruits` array remains unchanged.

The addition of these explanations completes the overview of the `push`, `pop`, and `slice` array methods. These methods are widely used for adding, removing, and extracting elements from arrays in JavaScript.

> These are just a few examples of array methods; there are many more available for sorting, filtering, mapping, and more. Arrays provide a powerful way to work with collections of data in JavaScript.
---
