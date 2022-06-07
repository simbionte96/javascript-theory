# Hoisting

In JavaScript the statements of the variables and functions are allocated in memory in compile time. On a practical level it's like an interpreter moved such statements to the beginning of their scope. This behaviour is known as **hoisting**.

Example

`greet(); //"Hello world"
function greet() {
	let greeting = "Helo world";
	console.log(greeting);
}`

When allocate the statement in memory it's like "going up" the function to the beginning of their scope.

Example

`function greet() { 
	let greeting = "Helo world"; 
	console.log(greeting);  
}  
greet(); //"Hello world"  
`

