# JavaScript Notes by Pramod Boda
## Core JavaScript
1) Introduction
2) Lexical Structure
	- Character Set
	- Comments
	- Literals
	- Identifiers
	- Reserved Words
3) Types
	- `Numbers`
	- `String`(Text)
	- `Boolean` Values
	- `null`
	- `undefined`
	- `Object`
4) Variables
	- Variable Declaration
	- Variable Scope
5) Expressions
6) Operators
	- Assignment Operators
	- Comparison Operators
	- Arithmetic Operators
	- Bitwise Operators
	- Logical Operators
	- String Operators
	- Conditional Operators
	- Comma Operators
	- Unary Operators
	- Relational Operators
7) Statements
	- Expresstion Statements
	- Compound & Empty Statements
	- Declaration Statements
	- Conditional Statements
		- `if`
		- `else if`
		- `switch`
	- Loop Statements 
		- while
		- do/while
		- for 
		- for in
	- Jumps
		- Labeled Statements 
		- `break`
		- `continue`
		- `return`
		- `throw`
		- `try` / `catch` / `finally`
	- Miscellaneous Statements
		- `with`
		- `debugger`
		- `"use strict"`

	- Summary of JavaScript Statements

8) Functions
9) Objects
10) Arrays

11) Class & Modules
12) Pattern Matching with Regular Expressions



<a id="jsIntroduction"></a>
## Introduction
### What is JavaScript?
- JavaScript is the Programming language of the **Web**
- JavaScript is part of the triad of technologies that all developers must learn

Language  |  Role  |  Description
------  |  ---------  | ----------
HTML  | Content  |  to specify the content of the web pages.
CSS  |  Presentation  |  to specify the presentation of the web pages.
JS  |  Behavior  |  to specify the behavior of the web pages.

- JavaScript is a high-level programming language.
- JavaScript is a case-sensitive language.
	- This means that language `keywords`, `variables`, `function` names, and other `identifiers` must always be typed with a consistent capitalization of letters.

		```javascript
		 var name = "Pramod Boda"; //initiated variable 'name'
		 Name; // will not be same as 'name'
		 NAME; // will not be same as 'name'
		 name; => "Pramod Boda"
		```

- All web browsers support it without the need for plug-ind by means of a built-in JavaScript engine.
- JavaScript is used on desktops, games consoles, tablets, and smart phones.
- Including JavaScript interpreters, making JavaScript the most ubiquitous programming language in history.
- JavaScript well-suited to object-oriented and functional programming style.
- The overwhelming majority of modern websites use JavaScript, and all web browsers.
- JavaScript has long since out grown its scripting - language roots to become a robust and efficient general - purpose language.

[<img src="images/toc.png" width="24" height="24" style="float: right;"/>](#toc)

<a id="jsLexicalStructure"></a>
## Lexical Structure

- The lexical structure of a programming language is the set of elementary rules that specifies how you write programs in that language.

### Character Set
- JavaScript programs are writing using the Unicode character set.
- Unicode is a superset of ASCII and Latin-1 and supports virtually every written language currently used on the planet.

### Case sensitivity
- JavaScript is a case-sensitive language. This means that language `keywords`, `variables`, `function` names, and other `identifies` must always be typed with consistent capitalization of letters.
```javascript
 var name = "Pramod Boda"; //initiated variable 'name'
 Name; // will not be same as 'name'
 NAME; // will not be same as 'name'
 name; => "Pramod Boda"
```

> Note: however, thet HTML is not case-sensitive(althought XHTML is).

- Many client-side JavaScript objects and properties have the same names as the HTML tags and attributes they represent. 
- While these tags and attributes names can be typed in any case in HTML, In JavaScript they typically must be all lowercase.

> The HTML onclick event handler attribute is sometimes specified as onClick in HTML, but it must be specified as onclick in JavaScript code(or in XHTML documents).

### Comments
- JavaScript supports two style of comments.
- Any text between a // and the end of a line is treated as a comment. and is ignored by JavaScript.
- Single comment example:
```javascript
 // This is a Single line comment.
```

- Any text between the characters /* and */ is also treated as a comment; These comments may span mutiple lines but may not be nested.
- Multi-Line comment example:
```javascript
 /* 
 * This is a
 * Multiple lines
 * comment.
 */
```

### Literals 

- A literals is a data that appears directly in a program.
```javascript
 46 // The Number forty six.
 4.6 // The Number four point six.
 "Hylo World" // A String of text.
 'Hi' // Another String.
 true // A Boolean value.
 false // another Booleans value.
 /javascript/gi // A regular expression literal (for pattern matching)
 null // Absence of object.
```

```javascript
 x:3, y:5 // An object initializer
 [1,2,3,a,b,c,4,5] // An array initializer.
```

### Identifiers
- An identifiers is simple a name. In JavaScript, identifiers are used to name variables and functions and to provide labels for certain loops in JavaScript code.
- These are all legal identifiers: 
```javascript
 var trueVar // variable initialization
 my_variable_name() // function name
 var v143 // variable initialization
 _trueVariable() // function name
 var $strVariable // variable initialization
```

#### Mathematical symbols
```javascript
 var si = true;
 var π = 3.14;
```

### Reserved Words

- You cannot use these words as `identifiers` in your programs.

| * | * | * | * | * |
| -------- | ----- | ----- | ----- | ----- |
| `break` | `delete` | `function` | `return` | `typeof` |
| `case` | `do` | `if` | `switch` | `var` |
| `catch` | `else` | `in`  | `this` | `void` |
| `continue` | `false` | `instanceof` | `throw` | `while` |
| `debugger` | `finally` | `new` | `true` | `with` |
| `default` | `for` | `null` | `try` |  |

**Non-reserved words that act like reserved words**
- The `NaN`, `Infinity`, `undefined` properties of the global ogject are immutable or read-only properties in ES5. So even though `var NaN = 42;` in the global scope wouldn't throw an error, it wouldn't actually do anything
- To avoid confusion, I'd suggest you to avoiding the use of these `variable` names.
```javascript
 //In the global scope
 var NaN = 42;
 console.log(NaN); // NaN
 
 //...but elsewhere
 (function(){
	 var NaN = 42;
	 console.log(NaN); // 42
 }());
```

### Dynamic Typing
JavaScript is a loosely typed or a dynamic language.


## Statements 
- `Statements` are JavaScript sentences or commands. 
- Just as English sentences are terminated and separated from each other with periods, JavaScript statements are terminated with semicolons. 
- `Expressions` are *evaluated* to produce a `value`, but `statements` are *executed* to make something happen.


### Numbers 
Percentage Calculator App:
```javascript
let empScore = 7757;
let maxVPay =  8497;

let empPercentage = (empScore / maxVPay) * 100;
console.log(empPercentage);
output=> 91.29104389784631
```

### Boolean Conditions 
```javascript
//Boolean Variable
let isAccountLocked = false;
//String Variable
let userRole = "admin";

//Boolean Conditions
if(isAccountLocked){
	console.log("Is acount loacked");
}else if(userRole === "admin"){
	console.log("Welcome Admin!");
}else{
	console.log("Welcome User!");
}
```

```javascript
let temp = 45;

if(temp<32){
 console.log("It is freezing outside!")
}
if(temp>=110){
	console.log("It is hot outside!");
}else{
	console.log("Go for it. It is pretty nice.")
}

```
### Difference between  `null`  and  `undefined`


`null`| `undefined`
-------- | -----
null is an assigned value. It means _nothing._ | undefined means a variable has been declared but not defined yet.
null is an object.   | undefined is of type undefined.
null !== undefined | but  null == undefined.
Unassigned variables are initialized by JavaScript with a default value of undefined. | JavaScript never sets a value to null. That must be done programmatically.



### Logical `AND(&&)` and `OR(||)` operators
```javascript
let temp = 100;

// AND(&&) operator - All condition should be true, Not enough with any one true, it should be all true.
if(temp>=60 && temp<=90){
	console.log("Go for it. It is pretty nice.");
}
// OR(||) operator - Any one should be true.
else if(temp<=0 || temp>=120){
	console.log("Dont go outsie!");
}else {
	console.log("Eh, Do what you want");
}
```

## 8. Functions

There are 3 important parts to a function: 

Function - input(Arguments), code(Statements), output(Return value)

```javascript
let square = function(num){
	let result = num * num;
	return result;
}

let value1 = square(6);
let value2 = square(30);

console.log(value1);
console.log(value2);
```
```javascript
let calVariablePayPercentage  = function(scoredVariablePay, maxVariablePay){
	let result = scoredVariablePay / maxVariablePay * 100;
	return result;
}

let pramodVPayPercentage = calVariablePayPercentage(7500,8500);
console.log(pramodVPayPercentage);
```


## 10. Arrays
### List of Array properties
- constructor
- length
- prototype

### List of Array methods
- ### Manipulating Arrays with Methods - To Add or Remove elements
	- `push(...items)` - adds item to the end.
	- `unshift(...items)` - adds item from the beginning.
	- `pop()` - extracts/ removes an item from the end.
	- `shift()` - extracts/ removes an item from the beginning.
	- `splice(pos, deleteCount, ...items)` - at index `pos` delete `deleteCount` elements and insert `items`.
```javascript
var  todo  =  ['HTML5',  'CSS3',  'JS',  'ES6/ES7',  'jQuery','React',  'TypeScript','Angular',  'Node'];
```
Add element to the end.
```javascript
todo.push('Less');
console.log('You have ' + todo.length + ' todos');
console.log(todo);
```
  Add element from the beginning.
```javascript
todo.unshift('Semantic UI');
console.log('You have ' + todo.length + ' todos');
console.log(todo);
```
  Remove element from the end.
```javascript
todo.pop();
console.log('You have ' + todo.length + ' todos');
console.log(todo);
```
  Remove element from the beginning.
```javascript
todo.shift();
console.log('You have ' + todo.length + ' todos');
console.log(todo);
```
Not deleting any element from the array, But just adding a element to array.
```javascript
todo.splice(3, 0, 'Bootstrap');
console.log('You have '  +  todo.length  +' todos');
console.log(todo);
//Output => You have 10 todos
//Output => (10) ["HTML5", "CSS3", "JS", "Bootstrap", "ES6/ES7", "jQuery", "React", "TypeScript", "Angular", "Node"]
```
Now we want to delete the element and replace the element in the same place.
```javascript
todo.splice(4, 1, 'ES6+');
console.log('You have '  +  todo.length  +' todos');
console.log(todo);
//Output => You have 10 todos
//Output => (10) ["HTML5", "CSS3", "JS", "Bootstrap", "ES6+", "jQuery", "React", "TypeScript", "Angular", "Node"]
```
### Looping over Array

**`forEach(func)`** - Calls `func` for every element, does not return anything.

```javascript
const  todo2  =  ['Make Art','Develop Website','Learn Web Development',  'Do Exercises',  'Earn Money','Save Money'];

console.log('You have '  +todo2.length+  ' todos');
todo2.forEach(function(item, index){
	console.log(index+' : '+item);
});

// Now we will little extened our code for perfect numbering display.
console.log('You have '  +todo2.length+  ' todos');
todo2.forEach(function(todo2, index){
	var  numInc  =  index + 1;
	console.log(numInc+' : '+todo2);
});
```

Alternate Method

The **for statement** creates a loop that consists of three optional expressions, enclosed in parentheses and separated by semicolons, followed by a statement (usually a [block statement](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/block)) to be executed in the loop.

Syntax
```javascript
for ([_initialization_]; [_condition_]; [_final-expression_]){
	statement
}
```

`forEach(func)` only counts from beginning to end.

You have an array now you want to count in order, than stick to` forEach(func)` method.

`for()` loop statement has bit more flexibility, you can count reverse too.

If you don't have an array and count in different order than stick to `for()` loop statements.

  
```javascript
console.log('You have '  +  todo2.length  +' todos');
	for(var  count=0; count<todo2.length; count++){
	var  num  =  count+1;
	var  todos  =  todo2[count]
	console.log(num+  ' : '  +todos);
}
```

**Count Reverse to an Array**
```javascript
console.log('You have '  +  todo2.length  +' todos');
	for(var  count=todo2.length-1; count>=0; count--){
	var  num  =  count+1;
	var  todos  =  todo2[count]
	console.log(num+  ' : '  +todos);
}
```


		-  `concat(...items)` - Joins two or more arrays, and returns a copy of the joined arrays

		-  `copyWithin()` - Copies array elements within the array, to and from specified positions.
			> Note: The `copyWithin()` method is not supported in IE 11 (and earlier versions).

		-  `every()` - checks if every element in an array pass a test.

		-  `fill()` - Fill the elements in an array with a static value.

		> Note: The `fill()` method is not supported in IE 11 (and earlier versions).

		-  `filter()` - Creates a new array with every element in an array that pass a test.

		> Note: The `filter()` method is not supported in IE 11 (and earlier versions).

		-  `find()` - Returns the value of the first element in an array that pass a test.

		> Note: The `find()` method is not supported in IE 11 (and earlier versions).

		-  `findIndex()` - Returns the index of the first element in an array that pass a test. `findIndex()` is like `find()`, but returns the index instead of a value.

		> Note: The `findIndex()` method is not supported in IE 11 (and earlier versions).

  

- To iterate over elements:

-  `forEach(func)` - Calls a function for each array element, does not return anything.

  

- To transform the array:

-  `map(func)` - creates a new array from result of calling `func` for every element.

-  `sort(func)` - sorts the array in-place, then returns it.

-  `reverse()` - reverses the array in-place, then returns it.
- `split/join` - convert a string to array and back.
- `reduce(func, initial)` - calculate a single value over the array by calling `func` for each element and passing an intermediate result between the calls.







