**[Hoisting](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)** is a JavaScript mechanism where variable declarations, function declarations, and class declarations are moved ("hoisted") to the top of their scope during the compile phase, before the code is executed. This means you can reference certain types of variables or functions before they are defined in the code.

However, **only the declarations are hoisted**, not the initializations. Here’s a breakdown of how hoisting works:

---

### 1. **Variable Hoisting**

Variables declared using `var` are hoisted to the top of their scope, but their initialization remains in place.

```javascript
console.log(a); // Output: undefined (declaration hoisted, but not initialization)
var a = 5;
console.log(a); // Output: 5
```

For `let` and `const`, the declarations are hoisted but are not initialized. They remain in a "temporal dead zone" from the start of the block until the declaration is encountered.

```javascript
console.log(b); // ReferenceError: Cannot access 'b' before initialization
let b = 10;
```

---

### 2. **Function Hoisting**

Function declarations are fully hoisted, meaning you can call the function before it is defined.

```javascript
greet(); // Output: Hello!
function greet() {
  console.log("Hello!");
}
```

But function expressions (e.g., using `var`, `let`, or `const`) are treated differently, as only the variable declaration is hoisted, not the function definition.

```javascript
console.log(sayHi); // Output: undefined
var sayHi = function () {
  console.log("Hi!");
};

sayHi(); // Output: Hi!
```

---

### 3. **Class Hoisting**

Classes are also hoisted, but like `let` and `const`, they remain in the temporal dead zone until declared.

```javascript
const obj = new MyClass(); // ReferenceError: Cannot access 'MyClass' before initialization
class MyClass {
  constructor() {
    this.name = "Class";
  }
}
```

---

### Key Takeaways:

- **Declarations** are hoisted, but **initializations** are not.
- Variables declared with `var` are partially hoisted (initialized to `undefined`).
- `let`, `const`, and `class` are hoisted but are in the temporal dead zone.
- Function declarations are fully hoisted, but function expressions are not.

Understanding hoisting helps avoid unexpected errors and write clearer, predictable JavaScript code.