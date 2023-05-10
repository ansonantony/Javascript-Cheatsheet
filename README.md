# Javascript-Cheatsheet


## Variables and Data Types

Declaring a variable:

```javascript
var variableName;
let anotherVariable;
const constantVariable = 'value';
```

Data types:

```javascript
// Primitive data types
let number = 42;
let string = 'Hello, world!';
let boolean = true;
let nullValue = null;
let undefinedValue = undefined;

// Non-primitive data types
let object = {};
let array = [];
let function = function() {};
```

## Operators

Arithmetic operators:

```javascript
let addition = 2 + 2;
let subtraction = 4 - 2;
let multiplication = 2 * 3;
let division = 6 / 2;
let modulo = 5 % 2;
```

Comparison operators:

```javascript
let equals = 2 == '2';
let strictEquals = 2 === '2';
let notEquals = 2 != '2';
let notStrictEquals = 2 !== '2';
let greaterThan = 3 > 2;
let lessThan = 2 < 3;
let greaterThanOrEqual = 3 >= 2;
let lessThanOrEqual = 2 <= 3;
```

Logical operators:

```javascript
let andOperator = true && false;
let orOperator = true || false;
let notOperator = !true;
```

Assignment operators:

```javascript
let assignment = 'value';
let additionAssignment = 2;
additionAssignment += 2;
let subtractionAssignment = 4;
subtractionAssignment -= 2;
let multiplicationAssignment = 2;
multiplicationAssignment *= 3;
let divisionAssignment = 6;
divisionAssignment /= 2;
let moduloAssignment = 5;
moduloAssignment %= 2;
```

## Control Flow

If statement:

```javascript
if (condition) {
  // code block to execute if condition is true
} else if (anotherCondition) {
  // code block to execute if anotherCondition is true
} else {
  // code block to execute if neither condition is true
}
```

Switch statement:

```javascript
switch (expression) {
  case value1:
    // code block to execute if expression matches value1
    break;
  case value2:
    // code block to execute if expression matches value2
    break;
  default:
    // code block to execute if expression matches none of the values
}
```

For loop:

```javascript
for (let i = 0; i < array.length; i++) {
  // code block to execute for each iteration
}
```

While loop:

```javascript
while (condition) {
  // code block to execute while condition is true
}
```

Do-while loop:

```javascript
do {
  // code block to execute at least once
} while (condition);
```

## Functions

Declaring a function:

```javascript
function functionName(parameter1, parameter2) {
  // code block to execute when the function is called
  return value;
}
```

Arrow function:

```javascript
const arrowFunctionName = (parameter1, parameter2) => {
  // code block to execute when the function is called
  return value;
};
```

## Objects and Arrays

Object:

```javascript
let object = {
  key1: 'value1',
  key2: 'value2',
  key3: function() {
    // code block to execute when the key3 method is called
  }
};
```

Array:

```javascript
let array = ['value1', 'value2', 'value3'];
array.push('value4');
array.pop();
```



## Error Handling

Try-catch block:

```javascript
try {
  // code that might throw an error
} catch (error) {
  // code to handle the error
} finally {
  // code to execute regardless of whether an error occurred or not
}
```

## DOM Manipulation

Accessing elements:

```javascript
// By ID
const elementById = document.getElementById('elementId');

// By class name
const elementsByClass = document.getElementsByClassName('className');

// By tag name
const elementsByTag = document.getElementsByTagName('tagName');

// By query selector
const elementByQuery = document.querySelector('selector');
const elementsByQueryAll = document.querySelectorAll('selector');
```

Modifying elements:

```javascript
element.textContent = 'new text'; // Modify text content
element.innerHTML = '<b>bold text</b>'; // Modify HTML content
element.setAttribute('attribute', 'value'); // Set attribute value
element.classList.add('className'); // Add a CSS class
element.style.property = 'value'; // Modify CSS styles
```

Event handling:

```javascript
element.addEventListener('event', function(event) {
  // code to handle the event
});
```

## Promises

Creating a promise:

```javascript
const promise = new Promise((resolve, reject) => {
  // code that performs an asynchronous operation
  if (/* operation successful */) {
    resolve(result); // resolve with a value
  } else {
    reject(error); // reject with an error
  }
});
```

Consuming a promise:

```javascript
promise
  .then(result => {
    // code to handle the resolved value
  })
  .catch(error => {
    // code to handle the rejected error
  })
  .finally(() => {
    // code to execute regardless of resolution or rejection
  });
```

## Modules

Exporting from a module:

```javascript
// module.js
export const variableName = 'value';

export function functionName() {
  // code for the exported function
}
```

Importing from a module:

```javascript
// app.js
import { variableName, functionName } from './module.js';
```

## Miscellaneous

Type conversion:

```javascript
let numberAsString = '42';
let number = Number(numberAsString);

let string = String(number);

let boolean = Boolean(value);
```

Timers:

```javascript
// setTimeout (executes a function after a delay)
setTimeout(function() {
  // code to execute after the delay
}, delay);

// setInterval (executes a function repeatedly with a fixed delay)
setInterval(function() {
  // code to execute repeatedly
}, delay);

// clearInterval (stops the execution of setInterval)
clearInterval(timerId);
```

This cheat sheet covers the basic syntax and concepts of JavaScript. Remember to refer to the specific documentation and resources for more detailed information and advanced features. Happy coding!

