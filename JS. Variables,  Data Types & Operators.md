## Variables 
#### Defining Variables 

To create a variable in JavaScript, use the `let` keyword.

```javascript
let x = 10;
console.log(x);
```

```javascript
let x = 10, y = 'raj', z = 5.5;
alert(y);
```

We can also use the `var` keyword for defining a variable. This is kinda old-fashion way.

```javascript
var x = 90
console.log(x)
```


A variable should be defined only once. Incase of doing it multiple times, it leads to syntax error.

```javascript
let x = 10;
let x = 50;
```
`SyntaxError: Identifier 'x' has already been declared`

---
**Naming rules of variables:**

- A variable should contain only 
	- letters
	- digits
	- dollar sign $
	- underscore symbol _
- A variable should not begin with a digit.
- Variables in JS are CASE-SENSITIVE.
- Reserved names or keywords should not be used as variables.

----
#### Constants

```javascript
const x = 80;
console.log(x)
```

The value stored in constants are permanent. they can't be changed at any point.


```javascript
const x = 80;
x = 90;
```

`TypeError: Assignment to constant variable.`

> **Best practice:** The best practice to define constants is to name them in UPPERCASE and underscores.

```javascript
const PI = 3.14
const ARRAY_SIZE = 1000
```

>  *A glance at variable names can reveal which code was written by a beginner versus an experienced developer.*

---
## [Summary](https://javascript.info/variables#summary)

We can declare variables to store data by using the `var`, `let`, or `const` keywords.

- `let` – is a modern variable declaration.
- `var` – is an old-school variable declaration. Normally we don’t use it at all, but we’ll cover subtle differences from `let` in the chapter [The old "var"](https://javascript.info/var), just in case you need them.
- `const` – is like `let`, but the value of the variable can’t be changed.

Variables should be named in a way that allows us to easily understand what’s inside them.

---
## Tasks

#### Working with variables

1. Declare two variables: `admin` and `name`.
2. Assign the value `"John"` to `name`.
3. Copy the value from `name` to `admin`.
4. Show the value of `admin` using `alert` (must output “John”).

```javascript 
let admin, name;
name = "John";
admin = name;
alert(admin);
```

> More to know: [Hoisting](https://github.com/Rajendran2201/javascript-cheatsheet/blob/main/Hoisting.md)

---

## Data types 

There are eight basic data types in JavaScript.

```javascript 

// 1. Number
let n = 100
let inf = Infinity;
let x = NaN;  // NaN ** 0 is 1

// 2. BigInt
console.log(9007199254740991 + 1) // 9007199254740992
// n is appended at the end of the integer
const bigInt = 6574324787446768979886876n;

// 3. String
let str = "rajendran";
let str2 = 'hello buddy';
let str3 = `hey everyone`;

console.log('Hello, ${str}');

// 4. Boolean 
let isEven = true;

// 5. null value
let age = null;

// 6. undefined 

let x;
console.log(x)

// 7. Objects

// 8. Symbols

```

##### typeof operator

```javascript
console.log(
	typeof undefined,
	typeof 99,
	typeof true,
	typeof "rajendran",
	typeof 5.23423,
	typeof 1/7,
)
```

---
### Summary 

There are 8 basic data types in JavaScript.

- Seven primitive data types:
    - `number` for numbers of any kind: integer or floating-point, integers are limited by `±(253-1)`.
    - `bigint` for integer numbers of arbitrary length.
    - `string` for strings. A string may have zero or more characters, there’s no separate single-character type.
    - `boolean` for `true`/`false`.
    - `null` for unknown values – a standalone type that has a single value `null`.
    - `undefined` for unassigned values – a standalone type that has a single value `undefined`.
    - `symbol` for unique identifiers.
- And one non-primitive data type:
    - `object` for more complex data structures.

The `typeof` operator allows us to see which type is stored in a variable.

- Usually used as `typeof x`, but `typeof(x)` is also possible.
- Returns a string with the name of the type, like `"string"`.
- For `null` returns `"object"` – this is an error in the language, it’s not actually an object.
---
## Type Conversion 

```javascript 
let value = true
value = String(value)
console.log(value)
```


```javascript 
console.log(Number("   123  "))
```

---
## Operators 

**Math Operators**
- Addition `+`,
- Subtraction `-`,
- Multiplication `*`,
- Division `/`,
- Remainder `%`,
- Exponentiation `**`.
- String concatenation operator +
- unary +, -
- assignment =

```javascript 
let a, b, c;
a = b = c = 22;
console.log(a, b, c);
```

**Bitwise Operators**
- AND ( `&` )
- OR ( `|` )
- XOR ( `^` )
- NOT ( `~` )
- LEFT SHIFT ( `<<` )
- RIGHT SHIFT ( `>>` )
- ZERO-FILL RIGHT SHIFT ( `>>>` )

- Comma operator

  > There are some other basics operators such as logical, comparative and so on.
