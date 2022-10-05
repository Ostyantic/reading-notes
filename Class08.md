
# **Operators and Loops**

Loops are used to perform repeated tasks. Various loop mechanisms offer different ways to determine the start and end points of the loop.

## Types of statements for loops

- for statement
- while statement
- do...while statement
- labeled statment
- break statement
- continue statement
- for...in statement
- for...of statement

## **for statement**

A `for` loop repeats until a specified condition evaluates to false.

### Syntax

```
for ([initialExpression]; [conditionExpression]; [incrementExpression]){statement}
```

```
for (i = 0; i < 5; i++){
  console.log(i);
}
```

When a `for` loop executes, the following occurs:

1. The initializing expression `i = 0` is executed.
2. The condition expression `i < 5` is evaluated. If the the value of `i < 5` is true , the loop statements execute. This loop continues until the value returns false, at which it wil terminate or break.
3. The statement `console.log(i)` executes.
4. The update expression `i++` is executed.
5. Step 2 is repeated.

## **while statement**

A `while` statement executes its statement as long as a specified condition evaluated to true. If the condition becomes false, the loop ends and control passes to the next statement. The condition is tested before the statement is executed. If the condition returns true, the statement is executed and the condition is tested again. This loop continues until the statement returns false. After the loop ends, control is passed to the next statement.

### Syntax

```
while (condition){statement}
```

### ***Infinite Loops***

It is possible for a loop to execute infinitly if your condition never returns a false evaluation. Always make sure your condition will return false so as to avoid infinite loops.

### Example

```
while (true) {
  console.log('Hello, world!');
}
```

For the example above, the condition `true` is being tested before executing the statement `console.log('Hello, world!')`. Since the condition returns as true, the statement continuously executes `Hello, World!` in the console. This is an inifite loop.

## Expressions

Ant **expression** is a vlaid unit of code that resolves to a value. There are two types of expressions: those that have side effects such as assigning values, and those that purely evaluate.

```
// expression with side effect
x = 7 
// expression that evaluates
x = 3 + 4
```

## Operators

Operators are special symbols in Javascript that are used to perform specific operations on values and variables (also known as operands).

### Types of Operators

- Assignment operator
- Comparison operator
- Arithmetic operator
- Bitwise operator
- Logical operator
- BigInt operator
- String operator
- Conditional (ternary) operator
- Comma operator
- Unary operator
- Relational operator
