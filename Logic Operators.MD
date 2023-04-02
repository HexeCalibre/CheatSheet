# Logic Operators in JavaScript
Logic operators are used in JavaScript to perform logical operations on Boolean
values. These operators allow you to perform different operations on Boolean
values, such as AND, OR, and NOT.

## Logical AND (&&) Operator

The logical AND operator (&&) returns true if both operands are true, and false
otherwise. It is represented using the && symbol. Here's and example:

```javascript

const a = true;
const b = false;
console.log(a && b);
// Output: false

```

In the above example, logical AND operator returns false because both
operands (a and b) are not true.

## Logical OR (||) Operator

The logical OR operator (||) returns true if at least one of the operands is true, and
false otherwise. It is represented using the || symbol. Here's an example:

```javascript

const a = true;
const b = false;
console.log(a || b);
// Output: true

```

In the above example, the logical OR operator returns true because at least one
operand (a) is true.

## Logical NOT (!) Operator

The logical NOT operator (!) returns the opposite of the Boolean value of its
operand. It is represented using the ! symbol. Here's and example:

```javascript

const a = true;
console.log(!a);
// Output: false

```

In the above example, the logical NOT operator returns false because the Boolean
value of the operand (a) is true, and the NOT operator returns the opposite of that
value.

## Combining Logical Operators

You can combine multiple logical operators to perform complex operations on
Boolean values. For example:

```javascript

const a = true;
const b = false;
const c = true;
console.log((a || b) && c);
// Output: true

```

In the above example, the logical OR operator returns true because at least one
operand (a) is true. Then , the logical AND operator checks whether the result of
the OR operations is true and the operand (c) is also true. Since both operands are
true, the final result is true.

## Conclusion

In JavaScripot, logic operators are used to perform logical operations on Boolean
values. You can use the logical AND, OR, and NOT operators to perform different
operations on Boolean values, and you can combine multiple operators to perform
complex operations.
