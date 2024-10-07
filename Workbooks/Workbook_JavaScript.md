# **JavaScript Workbook Notes 

---

## **Module 1: Introduction to JavaScript**

### **Section 1-1: Thinking About Programming**

#### **Programming**
- Programming involves writing instructions for computers to execute tasks.
  
**Example:**  
```javascript
let message = "Hello, Thounny!";
console.log(message);  // Output: Hello, Thounny!
```

---
### **Section 1-2: Learning to be Precise**

#### **Learning to Be Precise**
- Computers only execute what they are told, so instructions must be exact and clear.

#### **Expanded Command Vocabulary**
- Understanding programming vocabulary is essential to communicating with the computer.
---

### **Section 1-3: Dealing with Ambiguity**

#### **Dealing with Ambiguity**
- Ambiguity leads to errors. Programs need exact details to function correctly.

#### **Trying to Be Exact**
- Write your code as clearly as possible, avoiding assumptions or vague instructions.

#### **Complex Problems**
- Break complex problems down into smaller, manageable steps.

**Example:**  
```javascript
let score = 85;
if (score >= 90) {
    console.log("Thounny, you got an A!");
} else if (score >= 80) {
    console.log("Thounny, you got a B!");
} else {
    console.log("Thounny, keep working hard!");
}
```

---

### **Section 1-4: JavaScript Basics**

#### **JavaScript vs ECMAScript**
- **JavaScript** is a programming language, and **ECMAScript** is the standardized version of it.

#### **Using Semicolons to Separate Statements**
- Semicolons (`;`) are used to separate JavaScript statements.

**Example:**
```javascript
let x = 10;
let y = 20;
console.log(x + y);  // Output: 30
```

#### **Declaring Variables**
- Variables store values for later use. Use `let` or `const` to declare variables.

**Example:**
```javascript
let name = "Thounny";
const organization = "Year Up United";
```

#### **Storing Values in a Variable**
- You can store different types of data in variables, like strings, numbers, and booleans.

**Example:**
```javascript
let age = 25;
let isStudent = true;
```

#### **Using `console.log()` to Display a Message**
- `console.log()` prints output to the browser's console for debugging.

**Example:**
```javascript
console.log("Hello, Thounny! Welcome to Year Up United!");
```

#### **Comments**
- Comments are used to add notes to your code, which are ignored by JavaScript.
  - Single-line comments: `//`
  - Multi-line comments: `/* */`

**Example:**
```javascript
// This is a single-line comment
/* 
  This is a 
  multi-line comment
*/
```

#### **Primitive Types**
- Primitive types in JavaScript include:
  - **String:** `"Hello"`
  - **Number:** `42`
  - **Boolean:** `true` or `false`

**Example:**
```javascript
let greeting = "Hello, Thounny!";
let age = 30;
let isEnrolled = true;
```

#### **Exercises**
- Practice with basic JavaScript concepts, including variables, types, and `console.log()`.

#### **Getting Visual Studio Code Ready**
- Install and set up Visual Studio Code to write and run JavaScript code.

#### **Installing Extensions**
- Extensions like **ESLint** help detect code errors, while **Prettier** helps format code for better readability.

---

## **Module 2: Working with Numbers**

### **Section 2-1: Building Expressions**

#### **Expressions**
- An expression combines variables, values, and operators to produce a result.

**Example:**
```javascript
let result = 5 + 3 * 2;  // Output: 11 (multiplication happens first)
```

#### **Arithmetic Operators**
- Arithmetic operators in JavaScript include:
  - `+` (addition)
  - `-` (subtraction)
  - `*` (multiplication)
  - `/` (division)
  - `%` (modulus)

**Example:**
```javascript
let sum = 10 + 5;  // Output: 15
let remainder = 10 % 3;  // Output: 1
```

#### **Uninitialized Variables**
- Always initialize variables before using them to avoid errors.

#### **The `Math` Object**
- The `Math` object provides built-in functions for complex calculations.

**Example:**
```javascript
let squareRoot = Math.sqrt(16);  // Output: 4
```

#### **Pre/Post Increment/Decrement**
- **Pre-increment (`++x`)**: Increases the value before using it.
- **Post-increment (`x++`)**: Increases the value after using it.

**Example:**
```javascript
let x = 5;
console.log(++x);  // Output: 6 (pre-increment)
console.log(x++);  // Output: 6 (post-increment), then x becomes 7
```

---

### **Section 2-2: Parsing Strings into Numbers**

#### **Using `parseInt()` and `parseFloat()`**
- `parseInt()` converts strings to integers, and `parseFloat()` converts strings to decimal numbers.

**Example:**
```javascript
let numStr = "42";
let num = parseInt(numStr);  // Output: 42

let decimalStr = "3.14";
let decimal = parseFloat(decimalStr);  // Output: 3.14
```

#### **Using `Number()`**
- Converts strings or booleans to numbers.

**Example:**
```javascript
let str = "50";
let num = Number(str);  // Output: 50
```

---
## **Module 3: Programming with Conditionals**

### **Section 3-1: Making Decisions with `if/else`**

#### **Making Decisions using the `if` Statement**
- The **`if` statement** allows you to run code only when a certain condition is true.

**Example:**
```javascript
let age = 20;
if (age >= 18) {
    console.log("Thounny is an adult.");
}
```

#### **Comparison Operators**
- **Comparison operators** are used to compare two values:
  - `==` (equal to)
  - `===` (strict equal: value and type)
  - `!=` (not equal to)
  - `>` (greater than)
  - `<` (less than)

**Example:**
```javascript
let score = 85;
if (score >= 90) {
    console.log("Thounny got an A!");
} else if (score >= 80) {
    console.log("Thounny got a B!");
}
```

#### **Using the `if / else` Statement**
- The **`else` block** runs when the `if` condition is false.

**Example:**
```javascript
let hoursWorked = 35;
if (hoursWorked >= 40) {
    console.log("Thounny worked full-time.");
} else {
    console.log("Thounny worked part-time.");
}
```

---

#### **Exercises Using `if / else / if` Statements**
- Practice exercises that involve creating multiple conditions using `if`, `else if`, and `else`.

#### **Making AND / OR Decisions**
- Use logical operators like **`&&`** (AND) and **`||`** (OR) to combine multiple conditions.

**Example:**
```javascript
let age = 25;
let hasLicense = true;
if (age >= 18 && hasLicense) {
    console.log("Thounny can drive.");
}
```

#### **Exercises**
- Try making decisions with **`if / else`** and combining conditions using logical operators.

#### **`var` vs `let`**
- `let` is block-scoped, and `var` is function-scoped. In modern JavaScript, it's recommended to use `let`.

**Example:**
```javascript
let name = "Thounny";  // This variable is block-scoped
```

---

### **Section 3-2: Making Decisions with a `switch` Statement**

#### **The `switch` Statement**
- The **`switch` statement** is used to execute different code blocks based on the value of a variable.

**Example:**
```javascript
let day = 3;
switch (day) {
  case 1:
    console.log("It's Monday, Thounny.");
    break;
  case 2:
    console.log("It's Tuesday, Thounny.");
    break;
  case 3:
    console.log("It's Wednesday, Thounny.");
    break;
  default:
    console.log("Enjoy your day, Thounny!");
}
```

#### **Exercises Using the `switch` Statement**
- Practice using the `switch` statement to handle multiple possible conditions for a variable.

---

## **Module 4: JavaScript in the Browser**

### **Section 4-1: Building HTML Pages that Use JavaScript**

#### **Console Scripts vs Browser-Based Apps**
- You can use JavaScript both in the browser and in the console (e.g., Node.js).

#### **The `<script>` Element**
- To include JavaScript in an HTML page, use the `<script>` tag.

**Example:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Year Up United</title>
</head>
<body>
    <h1 id="welcome"></h1>
    <script>
        document.getElementById("welcome").innerHTML = "Welcome to Year Up United, Thounny!";
    </script>
</body>
</html>
```

#### **JavaScript Functions**
- JavaScript functions can be defined within an HTML file or in an external script.

**Example:**
```javascript
function greet(name) {
    return "Hello, " + name + "!";
}
console.log(greet("Thounny"));  // Output: Hello, Thounny!
```

#### **External Scripts**
- You can link external JavaScript files using the `<script src="file.js"></script>` tag.

**Example:**
```html
<script src="scripts.js"></script>
```

#### **Organizing Scripts**
- Organize your code by placing JavaScript in external files and linking them in your HTML.

---

### **Section 4-2: Interacting with Page Elements**

#### **Accessing Elements on the Page using `getElementById()`**
- Use **`document.getElementById()`** to access and manipulate HTML elements by their ID.

**Example:**
```javascript
document.getElementById("greeting").innerHTML = "Welcome back, Thounny!";
```

#### **Working with Contents of an Element using `innerHTML`**
- **`innerHTML`** allows you to change the content inside an HTML element.

**Example:**
```javascript
document.getElementById("message").innerHTML = "Thounny is learning JavaScript!";
```

#### **Working with `<input>` Elements**
- You can interact with user input using **`<input>`** elements and JavaScript.

**Example:**
```html
<input type="text" id="nameInput" value="Thounny">
<button onclick="showMessage()">Submit</button>

<script>
function showMessage() {
    let name = document.getElementById("nameInput").value;
    alert("Hello, " + name + "!");
}
</script>
```

#### **Combining Finding the HTML Element and Getting the Value**
- You can combine JavaScript methods to find elements and retrieve their values.

**Example:**
```javascript
let inputValue = document.getElementById("nameInput").value;
console.log("Input value:", inputValue);
```

---

### **Section 4-3: Event Handling**

#### **Events**
- JavaScript **events** are actions that happen in the browser, such as clicks or form submissions.

#### **Event Attributes**
- Event attributes, such as **`onclick`**, allow you to trigger JavaScript functions when events happen.

**Example:**
```html
<button onclick="showAlert()">Click Me!</button>

<script>
function showAlert() {
    alert("Thounny clicked the button!");
}
</script>
```

#### **Coding Event Logic in an HTML Attribute**
- Event logic can be placed inside HTML attributes, but it is generally better to separate JavaScript logic into scripts.

#### **Assigning Event Handlers When the Window Finishes Loading**
- Use the **`window.onload`** event to ensure scripts run after the page has fully loaded.

**Example:**
```javascript
window.onload = function() {
    document.getElementById("message").innerHTML = "Hello, Thounny!";
};
```

#### **Exercises**
- Practice handling various events such as `click`, `submit`, and `load`.

#### **Adding a Little Error Handling**
- Use **try/catch** blocks to handle errors in your JavaScript code.

**Example:**
```javascript
try {
    let value = null;
    console.log(value.toUpperCase());  // This will cause an error
} catch (error) {
    console.log("An error occurred:", error.message);
}
```

#### **Mini-Project**
- Create a mini-project that includes form inputs, event handling, and error checking.
