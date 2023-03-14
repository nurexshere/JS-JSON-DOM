# JavaScript

JavaScript is a programming language used primarily for creating interactive web pages and applications. It is a high-level, dynamic language that can be used for a wide variety of tasks, from simple animations to complex web applications.

JavaScript is often used together with HTML and CSS to create web pages that can be updated dynamically without requiring a page reload. It can also be used on the server side with Node.js to create full-stack web applications.

JavaScript has many features that make it a powerful and flexible language, including:

- Variables: used to store data and values
- Datatypes: including strings, numbers, booleans, and more
- Conditional statements: used to execute code based on different conditions
- Loops: used to execute code multiple times
- Functions: used to define reusable pieces of code
- Objects: used to store collections of data in key-value pairs
- Events: used to listen for user actions and browser events
- JSON: a lightweight data interchange format that is easy to read and write

JavaScript is a popular language due to its versatility and ease of use. It can be used for everything from simple scripts to complex web applications, and its popularity has led to a large community of developers and resources available online.

### →V**ariables**

```jsx
//const can’t be reassigned 
const number = 23
let number = 23

// var and let can be reassigned

var number = 21
```

### → D**atatype**

```jsx
// String
const name = “Jhon”

// number

const age = 21

consrt height = 1.83

// boolean

const todayIsSunny = true

// null

const x = null
```

### →C**onditional statement**

```jsx
// if else

const x =3

if (x==3){

console.log(”x is 3”)

}

else{

console.log(”x is not 3”)
```

### SWITCH statement in JavaScript

The `switch` statement in JavaScript allows you to execute a block of code based on different cases. It is similar to an `if...else` statement but can be more concise in some cases. Here is an example:

```
const day = "Monday";

switch (day) {
  case "Monday":
    console.log("Today is Monday");
    break;
  case "Tuesday":
    console.log("Today is Tuesday");
    break;
  case "Wednesday":
    console.log("Today is Wednesday");
    break;
  default:
    console.log("Today is another day");
}

```

In this example, the `switch` statement is checking the value of the variable `day` and executing different code blocks depending on the case. If `day` is "Monday", the output will be "Today is Monday". If `day` is "Tuesday", the output will be "Today is Tuesday", and so on. If `day` is not any of these values (i.e., it is another day), the `default` code block will be executed.

Remember to include the `break` keyword after each case to prevent the code from executing the code blocks of subsequent cases.

### For Loop in JavaScript

A `for` loop is used to execute a block of code a specified number of times. Here is an example:

```
// for loop

for (let i = 0; i < 5; i++) {
  console.log(i);
}

```

In this example, the `for` loop is used to execute the code block five times. The loop starts with `i` equal to 0, and then executes the code block as long as `i` is less than 5. After each iteration, `i` is incremented by 1. The output of this code will be:

```
0
1
2
3
4

```

Note that the `let` keyword is used to declare the variable `i` inside the loop. This ensures that `i` is only accessible inside the loop and not outside of it.

You can also use a `for...in` loop to iterate over the properties of an object, or a `for...of` loop to iterate over the elements of an array.

### Do-While Loop in JavaScript

A `do-while` loop is similar to a `while` loop, but with one key difference: the code block in a `do-while` loop is always executed at least once, even if the condition is `false`. Here is an example:

```
// do-while loop

let i = 0;

do {
  console.log(i);
  i++;
} while (i < 5);

```

In this example, the `do-while` loop is used to execute the code block at least once, even though `i` is initially equal to 0, which is not less than 5. After each iteration, `i` is incremented by 1, and the loop continues until `i` is 5. The output of this code will be:

```
0
1
2
3
4

```

Note that the condition in the `while` statement is checked after the code block has been executed, so the code block is always executed at least once.

### Functions

Functions are a fundamental building block of JavaScript programs. They allow you to define reusable pieces of code that can be called multiple times with different arguments.

In this example, the `add()` function takes two arguments, `a` and `b`, and returns their sum. The function is declared using the `function` keyword, followed by the function name, the parameter list in parentheses, and the code block in curly braces. To call the function, you simply use its name followed by the arguments in parentheses.

```
// Function declaration

function add(a, b) {
  return a + b;
}

// Function call

console.log(add(2, 3)); // Output: 5

```

JavaScript functions can also be used as first-class citizens, which means they can be assigned to variables, passed as arguments to other functions, and returned as values from functions.

In a function expression, you declare a variable and assign it a function as its value. In an arrow function, you use the arrow (`=>`) instead of the `function` keyword to declare the function.

```
// Function expression

const add = function(a, b) {
  return a + b;
}

// Arrow function

const add = (a, b) => a + b;

```

Remember to include a `return` statement in your function if you want it to return a value. If you don't include a `return` statement, the function will return `undefined`.

In this example, we assign a function to a variable, pass a function as an argument to another function, and return a function from a function. These are all examples of how JavaScript functions can be used as first-class citizens.

```
// Assigning a function to a variable

const add = function(a, b) {
  return a + b;
}

const sum = add(2, 3);

// Passing a function as an argument

function multiply(a, b) {
  return a * b;
}

function doMath(operation, a, b) {
  return operation(a, b);
}

const result = doMath(multiply, 2, 3);

// Returning a function from a function

function createAdder(a) {
  return function(b) {
    return a + b;
  }
}

const addTwo = createAdder(2);
const sum = addTwo(3); // Output: 5

```

Functions are a fundamental building block of JavaScript programs. They allow you to define reusable pieces of code that can be called multiple times with different arguments. Here is an example of a function in JavaScript:

## EVENTS IN JAVASCRIPT

JavaScript has many events that can be triggered by the user or the browser itself. Here are some examples of events in JavaScript:

# **JSON**

JSON stands for JavaScript Object Notation. It is a lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate. JSON is a text format that is completely language-independent, but it is often used with JavaScript because it is based on a subset of the JavaScript programming language.

### **OBJECT In JSON**

A JSON object is a collection of key-value pairs, similar to a JavaScript object. The keys must be strings, and the values can be any valid JSON data type, including strings, numbers, booleans, null, arrays, and other JSON objects. Here is an example of a JSON object:

```
{
  "name": "John",
  "age": 30,
  "city": "New York"
}

```

### **ARRAYS In JSON**

JSON arrays are ordered lists of values, similar to JavaScript arrays. The values can be any valid JSON data type. Here is an example of a JSON array:

```
[
  "apple",
  "banana",
  "orange"
]

```

JSON data can be easily exchanged between different programming languages and platforms, making it a popular format for data interchange over the internet. Many web APIs return JSON data, which can be easily consumed by JavaScript code.

### **PARSING In JSON**

To parse JSON data in JavaScript, you can use the `JSON.parse()` method, which takes a JSON string as input and returns a JavaScript object or array. To generate JSON data from a JavaScript object or array, you can use the `JSON.stringify()` method, which takes a JavaScript object or array as input and returns a JSON string.

```
// Parsing JSON data
const jsonStr = '{"name":"John","age":30,"city":"New York"}';
const jsonObj = JSON.parse(jsonStr);
console.log(jsonObj); // Output: {name: "John", age: 30, city: "New York"}

// Generating JSON data
const arr = ['apple', 'banana', 'orange'];
const jsonArr = JSON.stringify(arr);
console.log(jsonArr); // Output: '["apple","banana","orange"]'

```

JSON is a simple and flexible data format that is widely used for data interchange on the web. It is easy to read and write, and can be easily consumed by JavaScript code.

# **DOM( Document Object Model)**

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can interact with the page.

The DOM tree is a hierarchical representation of the HTML document. Each node in the tree represents an HTML element, and the elements are organized in a parent-child relationship, where the parent node is the element that contains the child node. For example, the `<body>` element is the parent of all the content on the page.

JavaScript can be used to interact with the DOM and change the content and style of a web page. You can use methods like `getElementById()` and `querySelector()` to select elements on the page, and then use properties like `innerHTML` and `style` to change the content and style of those elements.

Here is an example of how to use JavaScript to change the content of an HTML element:

```
<!DOCTYPE html>
<html>
<head>
	<title>DOM Example</title>
</head>
<body>
	<h1 id="title">Hello World!</h1>

	<script>
		// Select the element with the ID "title"
		const title = document.getElementById("title");

		// Change the text of the element
		title.innerHTML = "Hello DOM!";
	</script>
</body>
</html>

```

In this example, we use the `getElementById()` method to select the `<h1>` element with the ID "title". We then use the `innerHTML` property to change the text of the element to "Hello DOM!".

You can also use JavaScript to add and remove HTML elements from the page. Here is an example of how to use JavaScript to add an HTML element to the page:

```
<!DOCTYPE html>
<html>
<head>
	<title>DOM Example</title>
</head>
<body>
	<div id="container">
		<p>This is the original content of the container.</p>
	</div>

	<script>
		// Create a new element
		const newElement = document.createElement("p");

		// Add text to the new element
		const newText = document.createTextNode("This is some new content.");

		// Add the text to the new element
		newElement.appendChild(newText);

		// Select the container element
		const container = document.getElementById("container");

		// Add the new element to the container
		container.appendChild(newElement);
	</script>
</body>
</html>

```

In this example, we use the `createElement()` method to create a new `<p>` element, and the `createTextNode()` method to add text to the element. We then use the `appendChild()` method to add the new element to the `<div>` element with the ID "container".

The DOM allows you to dynamically change the content and style of a web page using JavaScript. This can be useful for creating interactive web applications and adding dynamic content to your web pages.

## **EVENTS IN DOM**

### **Event Listeners**

Here are some examples of events in JavaScript that can be used with the DOM:

- `click`: Triggered when an element is clicked
- `submit`: Triggered when a form is submitted
- `keydown`: Triggered when a key on the keyboard is pressed down
- `load`: Triggered when a page or image finishes loading
- `resize`: Triggered when the browser window is resized
- `scroll`: Triggered when the user scrolls up or down on the page

You can use JavaScript to listen for these events and execute code when they occur. Here is an example of how to listen for a `click` event on a button:

```
const button = document.querySelector('button');

button.addEventListener('click', () => {
  console.log('Button clicked!');
});

```

In this example, we use the `querySelector()` method to select a button element on the page. We then use the `addEventListener()` method to listen for a `click` event on the button. When the button is clicked, the callback function is executed, which logs a message to the console.

You can also use the `removeEventListener()` method to remove an event listener from an element. This can be useful if you want to prevent a function from being executed multiple times.

```
const button = document.querySelector('button');

const handleClick = () => {
  console.log('Button clicked!');
  button.removeEventListener('click', handleClick);
};

button.addEventListener('click', handleClick);

```

In this example, we define a function called `handleClick()` that logs a message to the console and removes the event listener from the button. We then add the event listener to the button, passing in the `handleClick()` function as the callback. When the button is clicked, the `handleClick()` function is executed, logging a message to the console and removing the event listener from the button.

- `click`: Triggered when an element is clicked
- `submit`: Triggered when a form is submitted
- `keydown`: Triggered when a key on the keyboard is pressed down
- `load`: Triggered when a page or image finishes loading
- `resize`: Triggered when the browser window is resized
- `scroll`: Triggered when the user scrolls up or down on the page

You can use JavaScript to listen for these events and execute code when they occur. Here is an example of how to listen for a `click` event on a button:

```
const button = document.querySelector('button');

button.addEventListener('click', () => {
  console.log('Button clicked!');
});

```

In this example, we use the `querySelector()` method to select a button element on the page. We then use the `addEventListener()` method to listen for a `click` event on the button. When the button is clicked, the callback function is executed, which logs a message to the console.

You can also use the `removeEventListener()` method to remove an event listener from an element. This can be useful if you want to prevent a function from being executed multiple times.

```
const button = document.querySelector('button');

const handleClick = () => {
  console.log('Button clicked!');
  button.removeEventListener('click', handleClick);
};

button.addEventListener('click', handleClick);

```

In this example, we define a function called `handleClick()` that logs a message to the console and removes the event listener from the button. We then add the event listener to the button, passing in the `handleClick()` function as the callback. When the button is clicked, the `handleClick()` function is executed, logging a message to the console and removing the event listener from the button.

```
// Function declaration

function add(a, b) {
  return a + b;
}

// Function call

console.log(add(2, 3)); // Output: 5

```

In this example, the `add()` function takes two arguments, `a` and `b`, and returns their sum. The function is declared using the `function` keyword, followed by the function name, the parameter list in parentheses, and the code block in curly braces. To call the function, you simply use its name followed by the arguments in parentheses.

You can also define functions using function expressions or arrow functions:

```
// Function expression

const add = function(a, b) {
  return a + b;
}

// Arrow function

const add = (a, b) => a + b;

```

In a function expression, you declare a variable and assign it a function as its value. In an arrow function, you use the arrow (`=>`) instead of the `function` keyword to declare the function.

JavaScript functions can also be used as first-class citizens, which means they can be assigned to variables, passed as arguments to other functions, and returned as values from functions.

```
// Assigning a function to a variable

const add = function(a, b) {
  return a + b;
}

const sum = add(2, 3);

// Passing a function as an argument

function multiply(a, b) {
  return a * b;
}

function doMath(operation, a, b) {
  return operation(a, b);
}

const result = doMath(multiply, 2, 3);

// Returning a function from a function

function createAdder(a) {
  return function(b) {
    return a + b;
  }
}

const addTwo = createAdder(2);
const sum = addTwo(3); // Output: 5

```

In this example, we assign a function to a variable, pass a function as an argument to another function, and return a function from a function. These are all examples of how JavaScript functions can be used as first-class citizens.

Remember to include a `return` statement in your function if you want it to return a value. If you don't include a `return` statement, the function will return `undefined`.

### Objects in JavaScript

Here are some examples of objects in JavaScript:

```
// Object literal notation

const person = {
  name: "John",
  age: 30,
  city: "New York"
};

// Accessing object properties with dot notation

console.log(person.name); // Output: John
console.log(person.age); // Output: 30
console.log(person.city); // Output: New York

// Accessing object properties with bracket notation

console.log(person['name']); // Output: John
console.log(person['age']); // Output: 30
console.log(person['city']); // Output: New York

```

You can also create objects using the `Object()` constructor or the `class` syntax in JavaScript.

# **Session storage and local storage**

Session storage and local storage are two web storage options that allow you to store data on the client-side. This means that the data is stored on the user's computer, rather than on a server.

### **Session storage**

Session storage is a web storage option that allows you to store data for a single browsing session. This means that the data is only available for as long as the browser window or tab is open. Once the browser window or tab is closed, the data is deleted.

To use session storage in JavaScript, you can use the `sessionStorage` object. You can store data in session storage using the `setItem()` method, and retrieve data from session storage using the `getItem()` method. Here is an example:

```
// Store data in session storage
sessionStorage.setItem('username', 'John');

// Retrieve data from session storage
const username = sessionStorage.getItem('username');
console.log(username); // Output: John

```

In this example, we store the string `'John'` under the key `'username'` in session storage using the `setItem()` method. We then retrieve the value stored under the key `'username'` using the `getItem()` method, and log it to the console.

### **Local storage**

Local storage is a web storage option that allows you to store data for an indefinite period of time. This means that the data is available even after the browser window or tab is closed, and can be accessed across multiple browsing sessions.

To use local storage in JavaScript, you can use the `localStorage` object. You can store data in local storage using the `setItem()` method, and retrieve data from local storage using the `getItem()` method. Here is an example:

```
// Store data in local storage
localStorage.setItem('username', 'John');

// Retrieve data from local storage
const username = localStorage.getItem('username');
console.log(username); // Output: John

```

In this example, we store the string `'John'` under the key `'username'` in local storage using the `setItem()` method. We then retrieve the value stored under the key `'username'` using the `getItem()` method, and log it to the console.

It is important to note that both session storage and local storage have limitations on the amount of data that can be stored. The exact limit varies depending on the browser and the device being used. It is also important to consider the security implications of storing data on the client-side, as it can be accessed and manipulated by anyone with access to the user's computer.

### **Clearing storage**

To clear data from session storage or local storage, you can use the `clear()` method. This method removes all data stored in the storage object. Here is an example:

```
// Clear session storage
sessionStorage.clear();

// Clear local storage
localStorage.clear();

```

In this example, we use the `clear()` method to remove all data stored in session storage and local storage.