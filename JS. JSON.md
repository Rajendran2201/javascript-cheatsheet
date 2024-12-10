**JavaScript Object Notation**

- It is a text format used to send and receive data in many programming languages.
- The `JSON.stringify()` is a function which takes an object as a parameter is used to convert an object to JSON format.
	- Only retains the data, eliminates the actions (functions)

 ```javascript
 const myJSON = JSON.stringify(myObj);
```

- The `JSON.parse()` is used to convert a JSON into Object. 
- It does the opposite operation of `JSON.stringify()`.

 ```javascript
 const myJSON = JSON.parse(JSONObj);
```

