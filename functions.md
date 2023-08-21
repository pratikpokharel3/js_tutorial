# Functions

A function is a self-contained block of code that is created for reusability. They are the building blocks of any programming language.

In JavaScript, we can define a function in the following way:

```js
function function_name(par1, par2, ... parN) {
    //block of code
}
```

To execute a function, we must invoke (or call) that function from somewhere within the program. Here is an example that demonstrates function declaration and calling the function.

```js
function show() {
    console.log('Hey there!')
}

show();
```

## Parameters

We can pass parameters to a function just like in any other programming langauges.

Example:

```js
function calculateArea(length, breadth) {
    console.log(length * breadth) //20
}

calculateArea(4, 5)
```

## Default Values

A function can use default values when no parameters are supplied to the called function.

Here is an example that demonstrates default values in a function.

```js
function show(message = 'Hello') {
    console.log(message)
}

show() //Hello
show('Hi') //Hi
show('Hola') //Hola
```

## return

We can return early from a function if certain conditions are true using the `return` keyword.

For example, we can modify the above function to use `return` in the following way:

```js
function calculateArea(length, breadth) {
    if (length < 0 || breadth < 0) {
        return 'Error: Cannot calculate area'
    }

    return length * breadth
}

console.log(calculateArea(4, 5)) //20
console.log(calculateArea(4, -5)) //Error: Cannot calculate area
```

## ES6

ECMAScript 6 (ES6) is a new way of creating a function using the arrow symbol, `=>`. It allows a short syntax for writing function expressions.

Here is an example of creating function using ES6 syntax:

```js
const calculateArea = (length, breadth) => {
    if (length < 0 || breadth < 0) {
        return 'Error: Cannot calculate area'
    }

    return length * breadth
}

console.log(calculateArea(4, 5)) //20
```

If the code is one-liner, we can reduce the amount of code by writing much cleaner function like this:

```js
const calculateArea = (length, breadth) => length * breadth

console.log(calculateArea(4, 5)) //20
```

::: info Things to Remember
Always define your functions earlier in the code before calling it. This is because the arrow functions are not hoisted to the top unlike regular functions. This would result in an error that functions are not initialized if you try to call the functions before its declaration.
:::
