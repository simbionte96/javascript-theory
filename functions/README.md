# Functions

The fuctions are the most basic entity of any program. In this section we are going to explore different ways they can appear.

## Statement Function

This is the classic way to define a function in JavaScript.

```javascript
function doSomething() {
	return "Doing something";
}

doSomething(); //"Doing something"
```

## Expression Function

An expression function has a similar syntax to statement function, but this is assigned to a variable and the function doesn't have name. The functions without name are called anonymous functions.

```javascript
const doSomething = function() {"Doing something"};

doSomething(); //"Doing something"
```

## Arrow Functions

This is the modern form to build a function, the standard. This syntax appears from ES6 as a simple way to write anonymous functions.

```javascript
//Whithout ES6
[1, 2, 3].map(function(i) {
	return i * 2;
	}
);
//With ES6
[1, 2, 3].map(n => n * 2);
```
