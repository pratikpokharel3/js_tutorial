# Loops

Like any other programming languages, looping can be performed using `for`, `while` and `do..while` keywords in JavaScript.

Here is an example that demonstrates loop:

```js
for (let i = 1; i <= 5; i++) {
    console.log('I love JavaScript')
}
```

## for

The `for` loop is one of the most commonly used loop in JavaScript. The syntax structure of the loop is similar to other programming languages like C, C++, Java, etc.

Example:

```js
//for loop that print numbers from 1 to 10
for (let i = 1; i <= 10; i++) {
    console.log(i)
}
```

## while

The `while` loop is another way of looping in JavaScript. The syntax structure of the loop is also similar to other programming languages.

We can write the above code using `while` loop like this:

```js
let i = 1

//while loop that prints number from 1 to 10
while (i <= 10) {
    console.log(i)
    i++
}
```

## do...while

The `do...while` loop is used when we want to perform some initial task and only stop the loop when certain conditions are true. The syntax structure of the loop is also similar to other programming languages.

We can write the above code using `do...while` loop like this:

```js
let i = 1

//do...while loop that print even numbers from 1 to 10
do {
    if (i % 2 === 0) {
        console.log(i)
    }
    i++;
} while(i !== 10)
```

## break

The `break` keyword can be used to exit early from the loop if certain conditions are true.

Example:

```js
//for loop that print numbers from 1 to 5 only
for (let i = 1; i <= 10; i++) {
    if (i === 5) {
        break
    }
    console.log(i)
}
```

## continue

The `continue` keyword can be used to skip current iteration in the loop if certain conditions are true.

Example:

```js
let i = 1

//while loop that print odd numbers from 1 to 10 only
while (i !== 10) {
    if (i % 2 === 0) {
        continue
    }
    console.log(i)
}
```

## Label

::: info
This section will be updated in future.
:::
