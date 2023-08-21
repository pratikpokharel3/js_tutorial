# Conditional Statements

These are the statements that are executed if certain conditions are true or false. For this, `if`, `if...else`, `if...else...if` keywords are used to evaluate conditions and based on it, the statements are executed accordingly.

## if

The `if` keyword is used to execute conditional statements in JavaScript. It is similar to other programming languages like C, C++, Java, etc.

Here is an example of using the `if` statement.

```js
let num = 26

if (num % 2 === 0) {
    console.log('It is an even number.')
}
```

::: info Info
If the code is one-liner, we can remove parentheses surrounding the `if` statement. However, it is always a good practice to use parentheses for better code readability.
:::

## if...else

The `if...else` statement can be used to execute different blocks of codes depending whether the conditions are either true or false.

We can write the above code using `if...else` statement like this:

```js
let num = 26

if (num % 2 === 0) {
    console.log('It is an even number.')
} else {
    console.log('It is a odd number.')
}
```

## if...else...if

The `if...else...if` statement can be used when multiple conditions need to be checked and execute the block of codes matching the conditions.

Here is an example of using `if...else...if` statement:

```js
let num = -4

if (num > 0) {
    console.log('It is a positive number.')
} else if (num < 0) {
    console.log('It is a negative number.')
} else {
    console.log('It is neither positive nor negative number')
}
```

Remember, we can have as many `if...else...if` statements to check for multiple conditions and execute the block of codes matching the conditions.

## switch

The `switch` keyword can be used to perform different actions based on different conditions. It provides more descriptive way to compare a value with multiple variants.

Here is an example of using `switch` statement:

```js
const day = 3

switch day
    case 1:
        console.log('Sunday')
        break
    case 2:
        console.log('Monday')
        break
    case 3:
        console.log('Tuesday')
        break
    case 4:
        console.log('Wednesday')
        break
    case 5:
        console.log('Thrusday')
        break
    case 6:
        console.log('Friday')
        break
    default:
        console.log('Saturday')
```

## Ternary Operator

The ternary operator is another way to execute conditional statement. It is an alternative to `if...else` statement.

Here is an example of using ternary operator `??`:

```js
let x = 10, y = 15
let result = x > y ? x : y
console.log(result) //15
```

## Null Coalescing Operator

The null coalescing operator `??` is a short syntax to get the defined value from the variable.

Consider an example below:

```js
let address

if (address !== null address !== undefined) {
    console.log(address)
}
```

The above code can be shorten using `??` operator like this:

```js
let address
console.log(address ?? 'Pokhara') //Pokhara
```
