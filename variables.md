# Variables

In any programming language, a variable is used to store data. Here, data can be anything like a string, number, boolean, array, object, etc. 

In JavaScript, we can define a variable using three keywords: `var`, `let`, and `const`. 

Here is an example that defines a variable in JavaScript.

```js
let city = 'Kathmandu'
```

## var

The `var` keyword is the old way of defining a variable in JavaScript. It is similar to `let` keyword but it differs internally in many ways like:
- `var` has no block scope.
- Variables that are declared with `var` can be redeclared with the same variable name.
- `var` can be declared below their use.

Don't worry, we've dedicated a section that explains how `var` internally differs from `let` [here](https://javascript.info/var). For now, understand that `var` is the old way of declaring a variable and you should always declare a variable with the `let` keyword which is the modern way of defining a variable in JavaScript.

So, the above code can be rewritten using `var` keyword like this:
```js
var city = 'Kathmandu'
```

## let

The `let` keyword is the modern way of defining variables in JavaScript. You should always use the `let` keyword when declaring variables to prevent any weird bugs or side effects that are associated with the `var` keyword.

We can write the above code using `let` keyword like this:
```js
let city = 'Kathmandu'
```

## const

The `const` keyword is another way of declaring a variable. The difference here is that once you declare a variable with a `const`, you cannot re-assign the variable with a different value. JavaScript will throw an error if you do so.

Example:
```js
const city = 'Kathmandu'

city = 'Pokhara' //Uncaught TypeError: Assignment to constant variable.
```

## Variable Naming

Now that you've understood how to define variables in JavaScript, it is also important to understand the rules for naming it. The rules that you must follow when defining a variable name are:

- A variable name can contain letters, numbers, underscores and dollar signs.
- A variable name can start with a letter, `_` or `$` sign but not with the number.
- Variables are case-sensitive which means `CITY` and `city` are two different variables.
- Reserved words like `var`, `let`, `const`, etc. used by JavaScript cannot be used as variable names.

```js
//Correct Declaration
let city = 'Kathmandu'
let age = 25
const PI = 3.1415
let $ = 420
let _ = 1997

//Incorrect Declaration
let 4life = 'Good'
let let = 45
```

While you are free to name variables to anything you like, naming variables with a meaning is always a good programming practice. It helps to improve code readability.