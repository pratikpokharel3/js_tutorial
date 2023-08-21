# Data Types

Like other programming languages, JavaScript also have data types. A value assigned to a variable always belong to a certain data type.

There are eight data types in JavaScript. The language automatically infer the right data type based on the value of the variable.

## String

A string is an array of characters in JavaScript.

We can define string variables in the following way:

```js
let fruit = 'Apple'
let day = 'Monday'
// ...
```

## Number

A number data type represents both integer and floating point numbers.

We can define number variables in the following way:

```js
let num = 4
const PI = 3.1415
// ...
```

::: info Note
A number data type also includes `Infinity`, `-Infinity` and `NAN`. These are special numerical values that can be used in different situations.
:::

## Boolean

A boolean data type has only two values: `true` or `false`.

We can define boolean variables in the following way:

```js
let decision = true
let result = 5 > 7
// ...
```

## Null

The `null` is a special data type of its own which contains a single value, i.e. `null`. It’s just a special value which represents "nothing", "empty" or "value unknown".

We can define `null` to variables in the following way:

```js
let name = null
let age = null
// ...
```

## Undefined

The `undefined` is also a special data type of its own which indicates that the value of a variable is `undefined` if it is not assigned.

JavaScript automatically assigns `undefined` to a variable if its value is not assigned or we can manually assign `undefined` to a variable in the following way:

```js
let name //undefined
let age = undefined
// ...
```

## Object

An object data type represent collections of data or more complex entities. The data are stored in key-value pair and must be inside `{}`.

We can define object variables in the following way:

```js
let person = {
    name: 'John',
    age: 26
}

let car = {
    company: 'Tesla',
    model: 'X',
    type: 'Electric'
}
// ...
```

## Symbol

A symbol data type is used to add unique property keys to an object. They allow to create “hidden” properties of an object, that no other part of code can accidentally access or overwrite.

We can define symbol variables in the following way:

```js
let id = Symbol("id")
let name = Symbol("name")
// ...
```

## BigInt

The bigint data type can be used to represent very large numbers greater than (2<sup>53</sup> - 1) or less than (-2<sup>53</sup> - 1). These data types are usually used when working with involves large numbers (like cryptography).

We can define a bigint variables in the following way:

```js
const privateKey = 984003027147562554123258541n
const publicKey = 451254121548765654545487874n
// ...
```

The `n` at the end of the number indicates that the numbers are of type `bigint`.
