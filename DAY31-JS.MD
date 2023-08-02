# JAVASCRIPT 07/04/2023
---
## Contents

[What is JavaScript]()

[Getting started]()

[]()

## What is JavaScript?
## Getting started
### How to use?

```html
<script src=""></script>
```

> :memo: **Best practice:** to put inside at the end of the `<body>` tag.

---

##### HTML `<script>` Attribute

| Attribute | Description |
| --------- | ----------- |
| `defer`   |             |
| `async`   |             |

![defer illustration]()

![async illustration]()

---

##### JavaScript Code

| Method | Description | Example |
| --------- | ----------- | ------- |
| `alert`   |             | `alert("Hello World!");` |
| `console.log`   |             | `console.log("Hello World!");` |
| `console.warn`   |             | `console.warn("warning message");` |
| `console.debug`   |             | `console.debug("debug message");` |
| `console.dir`   |             | `console.dir();` |
| `console.error`   |             | `console.error("error message");` |

##### Variables

| Attribute | Description |
| --------- | ----------- |
| `var`   |             |
| `let`   |             |
| `const`   |             |

===
###### When to use `var`, `let`, or `const`?
> 1. Always declare variables
> 2. Always use `const` if the value should not be changed
> 3. Always use `const` if the type should not be changed (Arrays and Objects)
> 4. Only use `let` if you can't use const
> 5. Only use var if you MUST support old browsers.
===