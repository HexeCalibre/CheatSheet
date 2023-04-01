## Let vs Const in JavaScript

In JavaScript, let and const are used to declare variables. While they may seem similar, they have some important differences.

## let

let is used to declare variables that can be reassigned later. For example:

```javascript

let x = 10;
x = 20;
//valid

```

You can also declare multiple variable with let on the same line:

```javascript

let x = 10; y = 20; z = 30;

```

let variables have block scope, meaning they are only accessible within the block they were defined in:

```javascript

if (true) {
    let x = 10;
}
console.log(x);

// ReferenceError: x is not defined

```

## const

const is used to declare variables that cannot be reassigned. For example:

```javascript

const x = 10;
x = 20;

// invalid

```

You must also initialize a const variable when you declare it:

```javascript

const x;

// SyntaxError: Missing initializer in const declaration

```

const variables also have block scope:

```javascript

if (ture) {
    const x = 10;
}

console.log(x);

// Reference Error: x is not defined

```

const is often used for values that should not change, such as constants, configuration settings, or function parameters that should not be modified.

## Which one shou you use?

As a general rule, use let for variables that can change, and const for values that should not. This can make your code easier to reason about and prevent accidental changes to important values.

However, keep in mind that const does not make objects or arrays immutable. You can still modify their properties or elements, even if you cannot reassign the variable itself.

```javascript

const obj = { x: 10 };
obj.x = 20; // valid
obj = { x: 30 } // invalid

```

In this case, you may want to use a library or language feature that provides true immutability, such as Object.freeze() or the Immutable.js library.

That's a brief introduction to let and const in JavaScript. Happy coding!
