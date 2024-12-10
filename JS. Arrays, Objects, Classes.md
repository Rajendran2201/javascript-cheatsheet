## Arrays
Arrays are a collection of objects. 

```javascript
let x = [1, 2, 3, 4, 5, 6,7 ,8 ];
console.log(x[3])
```

## Objects 
Objects are key-value pairs

```javascript 
const myObj = {name:"raj", age:19};

console.log(myObj['name'])
console.log(myObj.name)
```


## Classes


```javascript 
class Pizza{
	constructor(){
		this.size = "medium";
		this.crust = "original";
	}
	bake(){
		return console.log("Baking a pizza - "+ this.size, this.crust);
	}
}

const myPizza = new Pizza();
myPizza.bake();

```

