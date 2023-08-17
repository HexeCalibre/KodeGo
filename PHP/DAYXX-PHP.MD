# PHP Documentation

PHP is a popular server-side scripting language used for web development. It's known for its versatility and ability to create dynamic web applications.

## Table of Contents

1. [Installation](#installation)
2. [Basic Syntax](#basic-syntax)
3. [Variables](#variables)
4. [Control Structures](#control-structures)
5. [Functions](#functions)
6. [Arrays](#arrays)
7. [Working with Forms](#working-with-forms)
8. [Database Connectivity](#database-connectivity)
9. [Error Handling](#error-handling)
10. [Security Considerations](#security-considerations)

## Installation

PHP is typically installed on web servers. To install it locally, consider tools like [XAMPP](https://www.apachefriends.org/) or [MAMP](https://www.mamp.info/).

## Basic Syntax

PHP code is embedded within HTML using `<?php` and `?>` tags. Example:

```php
<!DOCTYPE html>
<html>
<head>
    <title>PHP Example</title>
</head>
<body>
    <?php
    echo "Hello, World!";
    ?>
</body>
</html>
```

## Variables

Declare variables using the `$` symbol followed by the variable name. PHP is loosely typed, so variables are dynamically typed based on their values.

```php
$name = "John";
$age = 30;
```

## Control Structures

PHP supports common control structures like `if`, `else`, `while`, `for`, and `switch`:

```php
if ($age < 18) {
    echo "You're a minor.";
} else {
    echo "You're an adult.";
}
```

## Functions

Define functions using the `function` keyword:

```php
function greet($name) {
    echo "Hello, $name!";
}
```

## Arrays

Arrays can hold multiple values:

```php
$fruits = array("Apple", "Banana", "Orange");
echo $fruits[0];  // Output: Apple
```

---

## Working with Forms

PHP is commonly used for form processing:

```html
<form method="post" action="process.php">
    <input type="text" name="username">
    <input type="password" name="password">
    <input type="submit" value="Login">
</form>
```

```php
// process.php
$username = $_POST["username"];
$password = $_POST["password"];
```

Database Connectivity

PHP can connect to databases like MySQL using extensions like MySQLi or PDO:

```php
$connection = new mysqli("localhost", "username", "password", "database");
if ($connection->connect_error) {
    die("Connection failed: " . $connection->connect_error);
}
```

## Error Handling

Use `try` and `catch` for error handling:

```php
try {
    // code that may throw an exception
} catch (Exception $e) {
    echo "An error occurred: " . $e->getMessage();
}
```
---

## Security Considerations

- Sanitize user input to prevent SQL injection and XSS attacks.

- Use prepared statements for database queries.

- Keep sensitive data secure, such as using password hashing.

This documentation provides a basic overview of PHP and its features. For more in-depth information, refer to the
[PHP Manual](https://www.php.net/manual/en/index.php)