---
title: "JavaScript for Beginners: Unlocking the Basics of Datatypes, Methods, Arrays, and Functions"
seoTitle: "JavaScript Basics: Datatypes, Methods, Arrays, and Functions | Beginn"
seoDescription: "Learn the basics of JavaScript datatypes, methods, arrays, and functions in this beginner's guide. Discover how to manipulate variables, use math and string"
datePublished: Sat Apr 22 2023 04:43:51 GMT+0000 (Coordinated Universal Time)
cuid: clgrhwr70000209johp9td62l
slug: javascript-for-beginners-unlocking-the-basics-of-datatypes-methods-arrays-and-functions
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1682129388215/2c032f36-01cf-4d48-98f3-4d81bcf84bd5.png
tags: javascript, web-development, webdev, frontend-development, wemakedevs

---

## Introduction

Welcome to the wonderful world of JavaScript! Whether you are a complete beginner or someone who has dabbled in programming before, this blog is the perfect starting point for unlocking the basics of datatypes, methods, arrays, and functions in JavaScript.

JavaScript is one of the most popular programming languages in the world and for good reason. It is the backbone of modern web development and allows developers to create dynamic and interactive web pages.

In this blog, we will take a step-by-step approach to understand the fundamental concepts of JavaScript. From variables to functions, we will cover everything you need to know to start building your own JavaScript programs. So, put on your thinking caps, grab a cup of coffee, and let's dive into the world of JavaScript!

## Variables

In JavaScript, variables are used to store data values.

Before proceeding any further we need to understand the meaning of few simple terms:

### **Function Scope**

Variables declared using the `var` keyword has function scope. This means that they are accessible within the function in which they are defined, as well as any nested functions.

### **Block Scope**

Variables declared using the `let` and `const` keywords have a block scope. This means that they are only accessible within the block in which they are defined. A block is a group of statements enclosed in curly braces `{}`.

### var, let, and const

To create a variable in JavaScript, you use the `var`, `let`, or `const` keyword followed by the variable name. Here's an example of how to declare a variable:

**<mark>let</mark>**

* `let` variables are block-scoped.
    
* They can be reassigned but not redeclared.
    
    ```javascript
    function exampleFunction() {
      let x = 1;
      if (true) {
        let x = 2;
        console.log(x); // outputs 2
      }
      console.log(x); // outputs 1
    }
    ```
    

**<mark>const</mark>**

* `const` variables are block-scoped.
    
* They cannot be reassigned or redeclared.
    
    ```javascript
    const PI = 3.14159;
    console.log(PI); // outputs 3.14159
    
    PI = 3.14; // error - cannot reassign const variable
    ```
    

**<mark>var</mark>**

* `var` variables are function-scoped.
    
* They can be redeclared and reassigned.
    
    ```javascript
    function exampleFunction() {
      var x = 1;
      if (true) {
        var x = 2;
        console.log(x); // outputs 2
      }
      console.log(x); // outputs 2
    }
    ```
    

<mark>It is my advice to avoid using var because it can be error-prone.</mark>

### Rules for naming variables

The following are the rules for naming variables in JavaScript:

1. Variables must start with a letter, underscore (\_), or a dollar sign ($).
    
2. Subsequent characters can be letters, numbers, underscores, or dollar signs.
    
3. Variable names are case-sensitive.
    
4. Avoid using reserved words as variable names (such as "var" or "function").
    
5. Use descriptive and meaningful names to make your code more readable and understandable.
    

Here are some examples of valid and invalid variable names:

<mark>Valid variable names:</mark>

* firstName
    
* \_age
    
* $salary
    
* book1
    
* my\_favorite\_color
    

<mark>Invalid variable names:</mark>

* 1stName (cannot start with a number)
    
* first-name (cannot contain hyphens)
    
* var (reserved word)
    
* class (reserved word)
    

## Datatypes

In JavaScript, there are primitive and reference datatypes. The primitive types are Boolean, Null, Undefined, Number, and String. The reference types are Object, Array, and Function.

### **Primitive Types**

Primitive types are data types that are immutable, meaning their value cannot be changed. There are five main primitive types in JavaScript:

1. `string`: A sequence of characters enclosed in quotes.
    
2. `number`: A numeric value, including integers and floating-point numbers.
    
3. `boolean`: A value that is either `true` or `false`.
    
4. `null`: A value that represents the intentional absence of any object value.
    
5. `undefined`: A value that represents the absence of a value.
    

Here's an example of how to create variables with primitive datatypes:

```javascript
let str = "Hello, world!"; // String
let num = 42; // Number
let bool = true; // Boolean
let undef = undefined; // Undefined
let nul = null; // Null
```

### **Reference Types**

Reference types are data types that are mutable, meaning their value can be changed. Reference types are objects that are stored as a reference to a location in memory, rather than being stored directly in a variable. There are three main reference types in JavaScript:

1. `Object`: A collection of key-value pairs that represent a real-world entity or concept.
    
2. `Array`: An ordered collection of elements of any type.
    
3. `Function`: A reusable block of code that performs a specific task.
    

Here's an example of how to create variables with reference datatypes:

```javascript
let arr = [1, 2, 3]; // Array
let obj = { name: "John", age: 30 }; // Object
let func = function (a, b) { return a + b; }; // Function
```

## Methods

In JavaScript, an object is like a container that holds related data and functions that perform operations on that data.

A method is a function that is attached to an object, which means it is a property of that object. When you call a method on an object, you're telling the object to execute that function.

Methods can be used to perform a wide variety of tasks, from manipulating data within an object to interacting with other objects in your program.

### String Methods

JavaScript provides a variety of string methods for manipulating strings. Here are a few examples:

* `toUpperCase()` - Converts a string to uppercase.
    
* `toLowerCase()` - Converts a string to lowercase.
    
* `charAt()` - Returns the character at a specified index in a string.
    
* `concat()` - Joins two or more strings together.
    
* `includes()` - Determines whether a string contains a specified substring.
    
* `replace()` - Replaces a specified substring with another string.
    
* `slice()` - Extracts a section of a string and returns it as a new string.
    
* `split()` - Splits a string into an array of substrings based on a specified delimiter.
    
* `trim()` - Removes whitespace from both ends of a string.
    

Here are some examples of how to use these methods:

```javascript
let str = "Hello, world!";

console.log(str.toUpperCase()); // "HELLO, WORLD!"
console.log(str.toLowerCase()); // "hello, world!"
console.log(str.charAt(1)); // "e"
console.log(str.concat(" How are you?")); // "Hello, world! How are you?"
console.log(str.includes("world")); // true
console.log(str.replace("Hello", "Hi")); // "Hi, world!"
console.log(str.slice(7, 12)); // "world"
console.log(str.split(" ")); // ["Hello,", "world!"]
console.log("  hello  ".trim()); // "hello"
```

### Array Methods

Arrays are used to store multiple values in a single variable. JavaScript provides a variety of array methods for manipulating arrays. Here are a few examples:

* `push()` - Adds one or more elements to the end of an array.
    
* `pop()` - Removes the last element from an array.
    
* `shift()` - Removes the first element from an array.
    
* `unshift()` - Adds one or more elements to the beginning of an array.
    
* `splice()` - Adds or removes elements from an array at a specified index.
    
* `slice()` - Extracts a section of an array and returns it as a new array.
    
* `concat()` - Joins two or more arrays together.
    
* `sort()` - Sorts the elements of an array in place.
    
* `reverse()` - Reverses the order of the elements in an array.
    

Here are some examples of how to use these methods:

```javascript
let myArray = [1, 2, 3];
myArray.push(4, 5); // [1, 2, 3, 4, 5]
myArray.pop(); // [1, 2, 3, 4]
myArray.shift(); // [2, 3, 4]
myArray.unshift(0, 1); // [0, 1, 2, 3, 4]
myArray.splice(2, 1, 'two'); // [0, 1, 'two', 3, 4]
let slicedArray = myArray.slice(2, 4); // ['two', 3]
let secondArray = [5, 6];
let concatenatedArray = myArray.concat(secondArray); // [0, 1, 'two', 3, 4, 5, 6]
concatenatedArray.sort(); // [0, 1, 3, 4, 5, 6, 'two']
concatenatedArray.reverse(); // ['two', 6, 5, 4, 3, 1, 0]
```

### Math Methods

JavaScript provides a number of built-in Math methods for performing mathematical operations. Some commonly used Math methods include:

* Math.abs() - Returns the absolute value of a number
    
* Math.ceil() - Rounds a number up to the nearest integer
    
* Math.floor() - Rounds a number down to the nearest integer
    
* Math.round() - Rounds a number to the nearest integer
    
* Math.max() - Returns the largest of zero or more numbers
    
* Math.min() - Returns the smallest of zero or more numbers
    
* Math.random() - Returns a random number between 0 and 1 (exclusive)
    

```javascript
// Math.abs() - returns the absolute value of a number
let num = -5;
let absoluteNum = Math.abs(num);
console.log(absoluteNum); // Output: 5

// Math.ceil() - rounds a number up to the nearest integer
let decimalNum = 3.14;
let roundedUpNum = Math.ceil(decimalNum);
console.log(roundedUpNum); // Output: 4

// Math.floor() - rounds a number down to the nearest integer
let decimalNum2 = 3.99;
let roundedDownNum = Math.floor(decimalNum2);
console.log(roundedDownNum); // Output: 3

// Math.round() - rounds a number to the nearest integer
let decimalNum3 = 3.5;
let roundedNum = Math.round(decimalNum3);
console.log(roundedNum); // Output: 4

// Math.max() - returns the largest of zero or more numbers
let num1 = 10;
let num2 = 20;
let num3 = 30;
let largestNum = Math.max(num1, num2, num3);
console.log(largestNum); // Output: 30

// Math.min() - returns the smallest of zero or more numbers
let smallestNum = Math.min(num1, num2, num3);
console.log(smallestNum); // Output: 10

// Math.random() - returns a random number between 0 and 1 (exclusive)
let randomNum = Math.random();
console.log(randomNum); // Output: a random number between 0 and 1 (e.g. 0.123456)
```

## Functions

A function is a reusable block of code or programming statements designed to perform a certain task. A function is declared by a function keyword followed by a name, followed by parentheses (). Parentheses can take a parameter. If a function takes a parameter it will be called with an argument. A function can also take a default parameter. Here's an example of how to define a function:

```javascript
function greetings(name) {
  console.log("Hello, " + name + "!");
}
```

In this example, the function is named, `greetings` and it takes in a parameter called `name`. The function logs a greeting to the console with the parameter.

Here's an example of how to call this function:

```javascript
greetings("Nikhil"); // logs "Hello, Nikhil!"
```

Functions can also return a value using the `return` keyword. Here's an example:

```javascript
function add(a, b) {
  return a + b;
}

let result = add(2, 3);
console.log(result); // logs 5
```

In this example, the `add` function takes in two parameters `a` and `b`, and returns their sum using the `return` keyword. The `result` variable is assigned the returned value of the function, and is logged to the console.

There are also several ways to define functions in JavaScript, including:

* <mark>Function declarations</mark>
    
* <mark>Function expressions</mark>
    
* <mark>Arrow functions</mark>
    

Here are some examples of each:

```javascript
// Function declaration
function multiply(a, b) {
  return a * b;
}

// Function expression
let divide = function (a, b) {
  return a / b;
};

// Arrow function
let subtract = (a, b) => {
  return a - b;
};
```

## Conclusion

In this blog, we covered the basics of JavaScript datatypes, including primitive and reference types, and how to use them in variables. We also looked at different methods for working with strings and arrays, as well as an introduction to functions and scope.

There's still much more to explore in JavaScript, including objects, the Document Object Model (DOM), and advanced topics like asynchronous programming. But with a solid understanding of the basics covered in this blog, you're well on your way to becoming a proficient JavaScript developer.

Stay tuned for future blogs where we'll dive into more advanced JavaScript topics and take your skills to the next level.

Before ending the blog I wanted to say to all of my audience that you guys are now **<mark>JS Man/Woman.</mark>**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1682137870266/6b5fa198-6dce-466d-95b9-d88d285a343b.png align="center")

## **Let's Connect**

If you enjoyed this post and would like to stay updated on my work, feel free to connect with me on social media

* LinkedIn: Click [**here**](https://www.linkedin.com/in/nikhil-mishra-8a6710244)
    
* Github: Click [**here**](https://github.com/mnik7044)
    
* Twitter: Click [**here**](https://twitter.com/nikktwts?t=WxH0im12f-NtbUJGeV2Xsw&s=09)
    

I'm always open to new connections and networking opportunities, so don't hesitate to reach out and say hello. Thank you for reading!