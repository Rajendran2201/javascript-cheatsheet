```javascript 

function showMyName(){
	return "raj";
}

console.log("Hey, This is " + showMyName())
```

A function can access outer/global variables.

```javascript 
let name = "raj"

function myName(){
	return name;
}

console.log("my name is " + myName())
```

---
#### Naming a function 

- The function names usually starts with verbs. 

Function starting with…

- `"get…"` – return a value,
- `"calc…"` – calculate something,
- `"create…"` – create something,
- `"check…"` – check something and return a boolean, etc.

> One function --> one action 

- Functions should be short and do exactly one thing. If that thing is big, maybe it’s worth it to split the function into a few smaller functions.

---
### Summary 

A function declaration looks like this:

- Values passed to a function as parameters are copied to its local variables.
- A function may access outer variables. But it works only from inside out. The code outside of the function doesn’t see its local variables.
- A function can return a value. If it doesn’t, then its result is `undefined`.

To make the code clean and easy to understand, it’s recommended to use mainly local variables and parameters in the function, not outer variables.

It is always easier to understand a function which gets parameters, works with them and returns a result than a function which gets no parameters, but modifies outer variables as a side effect.

**Function naming:**

- A name should clearly describe what the function does. When we see a function call in the code, a good name instantly gives us an understanding what it does and returns.
- A function is an action, so function names are usually verbal.
- There exist many well-known function prefixes like `create…`, `show…`, `get…`, `check…` and so on. Use them to hint what a function does.

---
## Arrow functions 

```javascript 
let showMyname = (name, age, city) => name;

console.log(showMyname("raj", 20, "hosur"))


let sum = (a, b) => {
	let ans = a + b;
	return ans
}

console.log(sum(10, 40))
```

---

> More to know: [Summary and best practices](https://javascript.info/javascript-specials)
