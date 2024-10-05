# Javascript

Java Script (1)

- Created by Brendan Eich , in Netscape (Mozilla) [ *1995* ]
- JS is not Java , and hence cant be used to develop applets
- Originally named **Mocha**
- Used **mainly in client side** scripting but lately being used in server side scripts also.

## Basics

- *Variables - Something to hold data*
    
    ```jsx
    var first = 'hello world';
    
    console.log(first);                  // will print the content of variable first //
    
    ```
    

- *Using computations:*
    
    ```jsx
    var a = 1;
    var b = 2;
    var total = a+b;
    total                                // will give output as 3 //
    ```
    

- *HTML integration* :

**Java script comes inside the script tag in html**

```html
<!DOCTYPE html>
<html>
<body>
<script>

var first = function() {
		console.log('hello world');
		alert('hello world1');
};

//calling function
first();
</script>

OMG!!!
</body>
</html>
```

**Java script can be included as a separate file outside html**

<aside>
👉🏻 using external JS will help the website to load faster

</aside>

- External js
    
    **sample.js**
    
    ```jsx
    function first() {
    		console.log('hello world');
    		alert('hello world1');
    };
    ```
    
    **sample.html**
    
    ```html
    <!DOCTYPE html>
    <html>
    <body>
    <script src ="sample.js">
    </script>
    <script>
    first();
    </script>
    
    OMG!!!
    </body>
    </html>
    ```
    
- *Getting input via STDIN*
    
    ```jsx
    const readline = require
    		("readline");
    const inp = readline
    		.createInterface({
    	input: process.stdin
    });
    
    inp.on("line",(data) => {
    	console.log(data)
    });
    ```
    

## Logical operators

### AND

- The `&&` operator returns `true` if both operands are `true`. Otherwise, it returns `false`.

```jsx
let a = true;
let b = false;

console.log(a && b); // false
console.log(a && true); // true
console.log(false && b); // false
console.log(true && true); // true

```

## OR

- The `||` operator returns `true` if at least one of the operands is `true`. If both are `false`, it returns `false`.

```jsx
let a = true;
let b = false;

console.log(a || b); // true
console.log(a || true); // true
console.log(false || b); // false
console.log(false || false); // false

```

<aside>
🚨 Note that as like in all languages js also will consider 0 as false and non-zero value as true

</aside>

## JavaScript comparison operators

### Equal

Checks if two values are equal. It performs type conversion if necessary.

```jsx
console.log(5 == '5'); // true
console.log(5 == 5);   // true
console.log(5 == 6);   // false

```

### Strict Equal

Checks if two values are equal and of the same type.

```jsx
console.log(5 === '5'); // false
console.log(5 === 5);   // true
console.log(5 === 6);   // false

```

### Not Equal

Checks if two values are not equal. It performs type conversion if necessary.

```jsx
console.log(5 != '5'); // false
console.log(5 != 5);   // false
console.log(5 != 6);   // true

```

### Strict Not Equal

Checks if two values are not equal or not of the same type.

```jsx
javascriptCopy code
console.log(5 !== '5'); // true
console.log(5 !== 5);   // false
console.log(5 !== 6);   // true

```

### Greater Than

Checks if the value on the left is greater than the value on the right.

```jsx
javascriptCopy code
console.log(5 > 3); // true
console.log(3 > 5); // false
console.log(5 > 5); // false

```

### Greater Than or Equal

Checks if the value on the left is greater than or equal to the value on the right.

```jsx
javascriptCopy code
console.log(5 >= 3); // true
console.log(3 >= 5); // false
console.log(5 >= 5); // true

```

### Less Than

Checks if the value on the left is less than the value on the right.

```jsx
javascriptCopy code
console.log(5 < 3); // false
console.log(3 < 5); // true
console.log(5 < 5); // false

```

### Less Than or Equal

Checks if the value on the left is less than or equal to the value on the right.

```jsx
javascriptCopy code
console.log(5 <= 3); // false
console.log(3 <= 5); // true
console.log(5 <= 5); // true

```

## JavaScript Increment Operator

The increment operator (`++`) is used to increase the value of a variable by 1. There are two types of increment operators in JavaScript:

### 1. Postfix Increment Operator (`x++`)

When the increment operator is placed after the variable (`x++`), it increases the value of the variable by 1 but returns the original value before the increment.

**Example:**

```jsx
let x = 5;
console.log(x++); // Output: 5 (original value before increment)
console.log(x);   // Output: 6 (value after increment)

```

### 2. Prefix Increment Operator (`++x`)

When the increment operator is placed before the variable (`++x`), it increases the value of the variable by 1 and returns the new value after the increment.

**Example:**

```jsx
let y = 5;
console.log(++y); // Output: 6 (value after increment)
console.log(y);   // Output: 6 (value after increment)

```

### Usage Example

Here is an example demonstrating both postfix and prefix increment operators:

```jsx
let a = 10;
let b = 10;

console.log("Postfix Increment:");
console.log(a++); // Output: 10 (original value before increment)
console.log(a);   // Output: 11 (value after increment)

console.log("Prefix Increment:");
console.log(++b); // Output: 11 (value after increment)
console.log(b);   // Output: 11 (value after increment)

```

## JavaScript Number and String Concatenation

JavaScript uses the `+` operator for string concatenation and arithmetic addition. When used with strings or mixed with numbers, it concatenates them.

### Using the `+` Operator

```jsx
let name = "John";
let age = 30;

// String concatenation
let message = "Hello, " + name + "! You are " + age + " years old.";
console.log(message); // Output: Hello, John! You are 30 years old.

// Mixing string and number
let info = "Name: " + name + ", Age: " + age;
console.log(info); // Output: Name: John, Age: 30

```

### Using Template Literals (ES6+)

Template literals (`${}`) provide a more flexible and readable way to concatenate strings and include expressions.

```jsx
let name = "Jane";
let age = 25;

// String concatenation with template literals
let greeting = `Hello, ${name}! You are ${age} years old.`;
console.log(greeting); // Output: Hello, Jane! You are 25 years old.

// Mixing string and number with template literals
let details = `Name: ${name}, Age: ${age}`;
console.log(details); // Output: Name: Jane, Age: 25

```

### Notes

- **Implicit Conversion:** JavaScript converts numbers to strings when using `+` with strings.
- **Template Literals:** Introduced in ES6, provide easier string interpolation and multiline strings with backticks (``).
    
    ### Usage Example
    
    ```jsx
    let firstName = "Alice";
    let lastName = "Smith";
    let age = 28;
    
    // Using template literals for complex concatenation
    let fullName = `${firstName} ${lastName}`;
    let profile = `${fullName} is ${age} years old.`;
    
    console.log(fullName); // Output: Alice Smith
    console.log(profile); // Output: Alice Smith is 28 years old.
    
    ```
    

## Loops and Iteration in JavaScript

Loops in JavaScript are used to repeatedly execute a block of code until a condition is met. There are several types of loops:

### 1. `for` Loop

The `for` loop executes a block of code a specified number of times.

```jsx
for (let i = 0; i < 5; i++) {
    console.log(i); // Outputs: 0, 1, 2, 3, 4
}

```

### 2. `while` Loop

The `while` loop executes a block of code as long as a specified condition is true.

```jsx
let i = 0;
while (i < 5) {
    console.log(i); // Outputs: 0, 1, 2, 3, 4
    i++;
}

```

### 3. `do...while` Loop

The `do...while` loop is similar to `while`, but it always executes the block of code once before checking the condition.

```jsx
let i = 0;
do {
    console.log(i); // Outputs: 0, 1, 2, 3, 4
    i++;
} while (i < 5);

```

### Iterating Over Arrays

You can iterate over arrays using loops or array methods like `forEach`, `map`, `filter`, etc.

```jsx
let numbers = [1, 2, 3, 4, 5];
for (let number of numbers) {
    console.log(number); // Outputs: 1, 2, 3, 4, 5
}

// Using forEach method
numbers.forEach(function(number) {
    console.log(number); // Outputs: 1, 2, 3, 4, 5
});

```

### Break and Continue Statements

- **`break`:** Terminates the loop immediately.
- **`continue`:** Skips the current iteration and continues to the next iteration.

```jsx
for (let i = 0; i < 10; i++) {
    if (i === 3) {
        continue; // Skips printing 3
    }
    if (i === 8) {
        break; // Stops loop at 8
    }
    console.log(i); // Outputs: 0, 1, 2, 4, 5, 6, 7
}

```

### Notes

- Loops are fundamental for iterating over data structures like arrays or performing repetitive tasks.
- Choose the appropriate loop type (`for`, `while`, `do...while`) based on the condition and requirements.

## JavaScript Break and Continue

## `break` Statement

The `break` statement terminates the current loop execution and resumes execution at the next statement after the loop.

**Example:**

```jsx
for (let i = 1; i <= 5; i++) {
    if (i === 3) {
        break;
    }
    console.log(i);
}
```

- Output:
    
    ```
    1
    2
    ```
    

## `continue` Statement

The `continue` statement skips the current iteration of the loop and proceeds to the next iteration.

**Example:**

```jsx
for (let i = 1; i <= 5; i++) {
    if (i === 3) {
        continue;
    }
    console.log(i);
}
```

- Output:
    
    ```
    1
    2
    4
    5
    ```
    

**Usage Scenarios:**

- `break`: Used to exit a loop early based on a condition.
- `continue`: Used to skip an iteration based on a condition and continue with the next iteration.

## JavaScript Reserved Words

### Keywords

These are reserved words that are part of the language syntax.

```
break
case
catch
class
const
continue
debugger
default
delete
do
else
enum
export
extends
false
finally
for
function
if
import
in
instanceof
new
null
return
super
switch
this
throw
true
try
typeof
var
void
while
with
yield
implements
interface
let
package
private
protected
public
static
```

## Arrays

JavaScript arrays are used to store multiple values in a single variable. They can hold any combination of values—strings, numbers, objects, or even other arrays.

## Creating Arrays

You can create arrays in JavaScript in several ways:

1. **Using Array Literal Syntax**:
    
    ```jsx
    let fruits = ["Apple", "Banana", "Mango"];
    ```
    
2. **Using the Array Constructor**:
    
    ```jsx
    let fruits = new Array("Apple", "Banana", "Mango");
    ```
    

## Accessing Array Elements

Array elements can be accessed using their index, starting from `0`.

```jsx
let fruits = ["Apple", "Banana", "Mango"];
console.log(fruits[0]); // Output: Apple
console.log(fruits[1]); // Output: Banana
```

## Array Properties and Methods

1. **Length Property**:
    - The `length` property returns the number of elements in an array.
    
    ```jsx
    let fruits = ["Apple", "Banana", "Mango"];
    console.log(fruits.length); // Output: 3
    ```
    
2. **push() Method**:
    - Adds one or more elements to the end of an array and returns the new length of the array.
    
    ```jsx
    let fruits = ["Apple", "Banana"];
    fruits.push("Mango");
    console.log(fruits); // Output: ["Apple", "Banana", "Mango"]
    ```
    
3. **pop() Method**:
    - Removes the last element of an array and returns that element.
    
    ```jsx
    let fruits = ["Apple", "Banana", "Mango"];
    let lastFruit = fruits.pop();
    console.log(lastFruit); // Output: Mango
    console.log(fruits);    // Output: ["Apple", "Banana"]
    ```
    
4. **shift() Method**:
    - Removes the first element of an array and returns that element.
    
    ```jsx
    let fruits = ["Apple", "Banana", "Mango"];
    let firstFruit = fruits.shift();
    console.log(firstFruit); // Output: Apple
    console.log(fruits);     // Output: ["Banana", "Mango"]
    ```
    
5. **unshift() Method**:
    - Adds one or more elements to the beginning of an array and returns the new length of the array.
    
    ```jsx
    let fruits = ["Banana", "Mango"];
    fruits.unshift("Apple");
    ```
    

## Functions

In JavaScript, functions are blocks of reusable code designed to perform a particular task. They are fundamental to structuring and organizing code for better maintainability and reusability.

## Creating Functions

There are a few ways to create functions in JavaScript:

1. **Function Declaration**:
    
    ```jsx
    function greet(name) {
        return "Hello, " + name + "!";
    }
    
    ```
    
2. **Function Expression** (Anonymous Function):
    
    ```jsx
    let greet = function(name) {
        return "Hello, " + name + "!";
    };
    
    ```
    
3. **Arrow Function** (ES6+):
    
    ```jsx
    let greet = (name) => {
        return "Hello, " + name + "!";
    };
    
    ```
    

## Calling Functions

Once defined, functions are called or invoked by using their name followed by parentheses containing any arguments (if required).

```jsx
let message = greet("Alice");
console.log(message); // Output: Hello, Alice!

```

## Function Parameters and Arguments

- **Parameters**: These are placeholders listed in the function definition.
    
    ```jsx
    function greet(name) { // `name` is a parameter
        return "Hello, " + name + "!";
    }
    
    ```
    
- **Arguments**: These are the actual values passed to the function when calling it.
    
    ```jsx
    let message = greet("Alice"); // "Alice" is an argument
    
    ```
    

## Return Statement

Functions can return values using the `return` statement. If no `return` statement is specified, the function returns `undefined`.

```jsx
function add(a, b) {
    return a + b;
}
let result = add(3, 4);
console.log(result); // Output: 7

```

## Function Scope

Variables declared inside a function are local to that function (function scope), meaning they are not accessible from outside the function.

```jsx
function sayHello() {
    let message = "Hello!";
    console.log(message); // Output: Hello!
}

// console.log(message); // Error: message is not defined outside sayHello()

```

## Function Hoisting

In JavaScript, function declarations are hoisted to the top of their scope, which allows you to call a function before it's declared in the code.

```jsx
console.log(add(2, 3)); // Output: 5

function add(a, b) {
    return a + b;
}

```

## Named vs Anonymous Functions

- **Named Function**:
    
    ```jsx
    function greet(name) {
        return "Hello, " + name + "!";
    }
    
    ```
    
- **Anonymous Function** (Function Expression):
    
    ```jsx
     let greet = function(name) {
        return "Hello, " + name + "!";
    };
    
    ```
    

Functions play a crucial role in JavaScript for code organization, encapsulation, and modularity, making it easier to manage and scale applications.

## Objects

JavaScript objects are collections of key-value pairs, where the keys are strings (or Symbols) and the values can be any type, including other objects. Objects are used to store data and functionality in a structured way.

## Creating Objects

1. **Object Literal Syntax**:
    
    ```jsx
    let person = {
        firstName: "John",
        lastName: "Doe",
        age: 30,
        isEmployed: true
    };
    ```
    
2. **Using the `Object` Constructor**:
    
    ```jsx
    let person = new Object();
    person.firstName = "John";
    person.lastName = "Doe";
    person.age = 30;
    person.isEmployed = true;
    ```
    

## Accessing Object Properties

You can access object properties using dot notation or bracket notation.

1. **Dot Notation**:
    
    ```jsx
    console.log(person.firstName); // Output: John
    console.log(person.age);       // Output: 30
    ```
    
2. **Bracket Notation**:
    
    ```jsx
    console.log(person["firstName"]); // Output: John
    console.log(person["age"]);       // Output: 30
    ```
    

## Adding and Modifying Properties

You can add or modify properties of an object using dot notation or bracket notation.

```jsx
person.middleName = "Michael"; // Adding a new property
person.age = 35;               // Modifying an existing property
```

## Removing Properties

You can remove a property from an object using the `delete` operator.

```jsx
delete person.isEmployed;
console.log(person.isEmployed); // Output: undefined
```

## Methods in Objects

Methods are functions that are stored as object properties.

```jsx
let person = {
    firstName: "John",
    lastName: "Doe",
    age: 30,
    fullName: function() {
        return this.firstName + " " + this.lastName;
    }
};

console.log(person.fullName()); // Output: John Doe
```

## Iterating Over Object Properties

You can iterate over the properties of an object using a `for...in` loop.

```jsx
for (let key in person) {
    if (person.hasOwnProperty(key)) {
        console.log(key + ": " + person[key]);
    }
}
```

## Object Methods and Properties

JavaScript objects come with several built-in methods and properties that make working with objects easier.

1. **`Object.keys()`**:
    - Returns an array of the object's own property names (keys).
    
    ```jsx
    console.log(Object.keys(person)); // Output: ["firstName", "lastName", "age", "fullName"]
    ```
    
2. **`Object.values()`**:
    - Returns an array of the object's own property values.
    
    ```jsx
    console.log(Object.values(person)); // Output: ["John", "Doe", 30, function() { return this.firstName + " " + this.lastName; }]
    ```
    
3. **`Object.entries()`**:
    - Returns an array of the object's own key-value pairs.
    
    ```jsx
    
    console.log(Object.entries(person)); // Output: [["firstName", "John"], ["lastName", "Doe"], ["age", 30], ["fullName", function() { return this.firstName + " " + this.lastName; }]]
    ```
    
4. **`Object.assign()`**:
    - Copies the values of all enumerable own properties from one or more source objects to a target object.
    
    ```jsx
    
    let additionalInfo = { isEmployed: true, nationality: "American" };
    Object.assign(person, additionalInfo);
    console.log(person); // Output: { firstName: "John", lastName: "Doe", age: 30,
    
    ```
    

## Anonymous Function

Anonymous functions in JavaScript are functions that are defined without a name. They are often used for short-term tasks that don’t require a separate, named function. They can be assigned to variables, passed as arguments to other functions, or used in places where functions are expected but don't need to be reused.

### Syntax and Examples

**Basic Anonymous Function**

```jsx

let sum = function(a, b) {
    return a + b;
};

console.log(sum(5, 3)); // Output: 8
```

In this example, an anonymous function is assigned to the variable `sum`. The function takes two parameters, `a` and `b`, and returns their sum.

**Anonymous Function as an Argument**

```jsx

setTimeout(function() {
    console.log("This message is displayed after 2 seconds");
}, 2000);
```

Here, an anonymous function is passed as an argument to the `setTimeout` function. It will be executed after a delay of 2000 milliseconds (2 seconds).

**Immediately Invoked Function Expression (IIFE)**

```jsx

(function() {
    console.log("This is an immediately invoked function expression");
})();
```

An IIFE is an anonymous function that is executed immediately after it is defined. This is useful for creating a new scope and avoiding polluting the global scope.

**Anonymous Function in Event Handling**

```jsx
document.getElementById('myButton').addEventListener('click', function() {
    console.log("Button was clicked!");
});
```

An anonymous function is used as an event handler for a button click event. This function will execute whenever the button with the ID `myButton` is clicked.

**Arrow Functions**

Arrow functions are a shorter syntax for writing anonymous functions and were introduced in ES6.

```jsx
let multiply = (a, b) => {
    return a * b;
};

console.log(multiply(4, 7)); // Output: 28
```

Arrow functions can also be written in a more concise form if they contain only a single expression.

```jsx
let divide = (a, b) => a / b;

console.log(divide(10, 2)); // Output: 5
```

### When to Use Anonymous Functions

- **Callbacks**: When passing a function as an argument to another function, such as in event handlers or asynchronous operations.
- **IIFE**: To create a new scope and avoid variable name conflicts.
- **Short-Term Usage**: For functions that are used only once and don’t need a name.