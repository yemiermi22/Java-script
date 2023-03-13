# Java script

## variables

variables can be declared using the var, let, or const keyword. var is the oldest way to declare a variable, while let and const were introduced in ES6. Variables declared with var are function-scoped, while variables declared with let and const are block-scoped. const is used to declare a variable that can't be reassigned to a new value, while let is used for variables that can be reassigned var is a keyword in JavaScript that allows you to declare a variable with either function scope or global scope.

JavaScript has several built-in data structures, including arrays, objects, and maps.

```jsx
//var
let a;
let name = "Simon";
console.log(name);
```

## **const**

- constant variable are used mostly for a constant data type that cannot be changed. const is a keyword in JavaScript that allows you to declare a variable with block scope that cannot be reassigned. This means that the variable is only accessible within the block of code in which it is declared, and its value cannot be changed once it has been assigned.
- And we use const to declare a constant datatype.

```jsx
<!DOCTYPE html>
<html>
<body>

<h1>JavaScripta Variables</h1>

<p>In this example, price1, price2, and total are variables.</p>

<p id="demo"></p>

<script>
const price1 = 5;
const price2 = 6;
let total = price1 + price2;
document.getElementById("demo").innerHTML =
"The total is: " + total;
</script>

</body>
</html>
```

### object

Objects are collections of key-value pairs, where the keys are strings and the values can be any type of data.

```jsx
new Object(value)

Object(value)

let object_name = {
    key_name : value,
    ...
}
```

## Condition

- JavaScript also allows you to write code that perform different actions based on the results of a logical or comparative test conditions at run time.
    - There are several conditional statements in JavaScript that you can use to make decisions:

### if else statement

The if else statement in JavaScript allows you to execute a block of code if a specific condition is true, and another block of code if the condition is false. Here is an example:

```
let name = "kittens";
if (name === "puppies") {
  name += " woof";
} else if (name === "kittens") {
  name += " meow";
} else {
  name += "!";
}

```

### switch statement

The switch statement in JavaScript allows you to execute a block of code depending on the value of a variable. Here is an example:

```
switch (action) {
  case "draw":
    drawIt();
    break;
  case "eat":
    eatIt();
    break;
  default:
    doNothing();
}

```

JavaScript has several types of loops, including the while loop, the do while loop, and the for loop.

### do while loop

The do while loop is similar to the while loop, except that the code block is always executed at least once. Here is an example:

```
do {
  // code block to be executed
} while (condition);

```

### for loop

 is used to execute a block of code a specific number of times. Here is an example:

```
for (let i = 0; i < 5; i++) {
  // code block to be executed
}
//for loop
for (let i = 0; i < 5; i++) {
  // Will execute 5 times
```

### Functions

In JavaScript are blocks of code that can be reused. They can take in parameters and return values. 

- Functions reduces the repetition of code within a program.
- Functions makes the code much easier to maintain.
- Functions makes it easier to eliminate the errors.

Here is an example of a simple function:

```jsx
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>JavaScript Define and Call a Function</title>
</head>
<body>
    <script>
    // Defining function
    function sayHello() {
        document.write("Hello, welcome to this website!");
    }
     
    // Calling function
    sayHello(); // Prints: Hello, welcome to this website!
    </script>
</body>
</html>

output:

Hello, welcome to this website!

```

### Events

events are actions or occurrences that happen in the browser, such as a user clicking on a button or the browser finishing loading a page. JavaScript can be used to listen for these events and respond to them with a function. Here is an example of attaching an event listener to a button:

```jsx

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <title>JavaScript Attaching Event Handlers Inline</title>
</head>
<body>
    <button type="button" onclick="alert('Hello World!')">Click Me</button>
</body>
</html>
```

## Data Structure

- Data structures are techniques for storing and organizing data that make it easier to modify, navigate, and access. Data structures determine how data is collected, the functions we can use to access it, and the relationships between data.
- JavaScript has primitive and non-primitive data structures.
    - **Primitive data structures** and data types are native to the programming language
    - **Integer Float**
    - **Boolean:**
    - **Character**
    
    - **Non-primitive data structures** are not defined by the programming language but rather by the programmer. These include linear data structures, static data structures, and dynamic data structures, like queue and linked lists.
    - **Array:**
     An array is a data structure that can hold the elements of same type. It cannot contain the elements of different types like integer with character

### Data type

 Data type JavaScript provides different **data types**
 to hold different types of values 

JavaScript has 8 Datatype

1. String

2. Number

3. Bigint

4. Boolean

5. Undefined

6. Null

7. Symbol

8. Object