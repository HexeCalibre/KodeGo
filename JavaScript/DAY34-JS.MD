# JAVASCRIPT Introduction 07/07/2023

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

> In this example, the add function is assigned to the variable myFunction. As a result, we can call the add function using the myFunction variable, passing 3 and 5 as arguments, and store the result in the result variable.
>
> Function assignment is a powerful technique that enables various programming patterns, including functional programming paradigms and higher-order functions. It provides flexibility and reusability in code, allowing developers to design more elegant and efficient solutions to complex problems.

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
