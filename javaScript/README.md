# Javascript
## Variables 
#### Create a variable
```js
// let
let name = "someName" ;

// const :
const CONSTANT = "";

// var :
//
var globalVar = 4000 ;
```

## Types 
* Javascript has 6 primitives data types, everything else is considered an object
* primitives are immutable

##### Check the type
```js
let n = 10 ; 
// we use the typeof function 
typeof(n); // this will return 'number'
typeof("ok"); // this will return 'string'
```
> *you can convert to numbers by preceding with the + operator*
## Numbers

## String
#### String interpolation
```js 
	let name = "Larry";
	console.log(`Hello, ${name}`);
```
#### includes
```js
``` 
## Arrays
#### Create an array
```js
let fruits = ["oranges","apples","kiwis"];
```
### Useful array methods
#### get the length of the array
```js
	// array.length

```
#### remove first of last element of the array 
```js
	// shift & pop
	
```

#### Map/Filter/Reduce

## Objects


### Objects/Array destructuring
 

### spread operator
```js
	let arr1 = [1,2,3];
	// can be used to create new arrays from old ones
	let newArr = [...arr1,4];
```


#### Create an object 
```js
let book = {
	title: "A song of ice and fire",
	author: "George RR martin"
}
```

#### Access a field

```js
let title = book.title;  // "A song of ice and fire"
```

## Conditionals
### If/Else
### Switch

## Loops
### While
### For loop
#### c-style-for
#### for-in
#### for-of

## Functions
#### Create a function

```js
function myfunction() {
	return "john doe"; 
}	

```
##### & then call it 
```js
myfunction();
```
#### Anonymous functions
```js
// anonymous functions can be passed as argument to some function
// or assigned to a variable to be called later
// or just be called instantly
const f = function(){
	console.log("anonymous function called");
}();
```

#### Arrow functions
```js
// arrow functions are small and consice
// they work the same way as the anonmymous functions
// can be assinged to any variable
// or passed as an argument to a function
// or called immediatly

(() => console.log("smallest function call in js"))() 

```
## Classes
#### Create a class
```js
class Person {

}
```

#### Create a constructor
```js
class Person {
	constructor(name){
	}
}
```

#### New instance a class

#### Getters & setters

## localStorage/sessionStorage

## Promises

## imports

%$^

## JS & the browser

## Server side JS
