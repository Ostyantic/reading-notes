
# **Programming with JavaScript**

## Control Flow, what is it?

Control Flow is the order in which the computer executes statements in a script. Think of it as waking up in the morning. Everyday you wake up at a certain time, and perform certain specific tasks before starting your day, right? Well control is no different, the code performs specific tasks in order before moving on to the next task. Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:

```
if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}
```

## Functions & Operators

### **Function** - A block of code designed to perform a particular task. A function is executed when "something" invokes (or calls) it

- a block of code designed to perform a particular task.
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

### **What does the Syntax for a Function look like?**

A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
**(parameter1, parameter2, ...)**

The code to be executed, by the function, is placed inside curly brackets: **{}**

```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

Function **parameters** are listed inside the parentheses () in the function definition.

Function **arguments** are the **values** received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

### **Why do we use Functions?**

Functions can be used to define code once and used as many times as one wishes by using different arguements, to produce different results.

```
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}
document.getElementById("demo").innerHTML = toCelsius(77);
```

### **Function Return**

When JavaScript reaches a `return` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a return value. The return value is "returned" back to the "caller":

```
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
```
