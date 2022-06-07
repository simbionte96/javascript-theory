# Hoisting

In JavaScript the statements of the variables and functions are allocated in memory in compile time. On a practical level it's like an interpreter moved such statements to the beginning of their scope. This behaviour is known as **hoisting**.

Example

```javascript
greet(); //"Hello world"
function greet() {
	let greeting = "Helo world";
	console.log(greeting);
}
```

When allocate the statement in memory it's like "going up" the function to the beginning of their scope.

Example

```javascript
function greet() { 
	let greeting = "Helo world"; 
	console.log(greeting);  
}  
greet(); //"Hello world"  
```

In the case of the variables, the hoisting can generate unexpected behaviours. The hoisting afects the statements not assignments.

Example

```javascript
var greet = "Hi";
function() {
	console.log(greet); //"Undefined"
	var greet = "Hello";
	console.log(greet); //"Hello"
} 
```

What really happened?

```javascript
var greet;
var greet = "Hi";
function() {
	var greet;
	console.log(greet); //"Undefined"
	var greet = "Hello";
	console.log(greet); //"Hello"
} 
```

