# JavaScriptSampleStuff

==> Javascript is lightweight
==> Javascript is case sensitive
==> Javascript can accept string values like single or double quotes
==> JYou can place any number of scripts in an HTML document.
==> JScripts can be placed in the <body>, or in the <head> section of an HTML page, or in both.
==> By using the script tag we can implement the javascript code.
External scripts can be referenced with a full URL or with a path relative to the current web page.
// eg:- <script src="https://www.w3schools.com/js/myScript1.js"></script>
// <script src="/js/myScript1.js"></script>
==> JavaScript to program the behavior of web pages
==> Many desktop and server programs use JavaScript.
==> Node.js is the best known.
==> Some databases, like MongoDB and CouchDB, also use JavaScript as their programming language.

Operator	                        Description	                        Example
	( )		                          Expression grouping		              (3 + 4)
  .			                          Member			                      person.name
  []		                          Member		                        person["name"]
  ()			                        Function call			                myFunction()
  new		                         	Create			                       new Date()
  in	                         		Propery in Object		             	"PI" in Math
  instanceof                			Instance of Object	           		instanceof Array
  yield	               			      Pause Function	               			yield x
  // The remaining opeators are similar to java.
  
  // Debug the javascript use atom ide to change the script code.
  // Run the .html file in the chrome.
  // Right click empty space and select "Inspect" option
  // Left side box we can select the "Sources" and select the .html file
  ===> put debug point (By left click on margin) on perticular line
  ===> Run the .html (By refresh the code run) 
  ===> Select the "Watch" option ===> select the "+" button ==> give your expression ==> it can print output
  ===> Right side panel we can the output
  ===> Below we can see the console output.
  
  typeof Operator
  ===> JavaScript typeof operator to find the type of a JavaScript variable
  ===> typeof operator returns the type of a variable or an expression
  typeof "John"; // o/p :- String 
  typeof 1;      // o/p :- Number
  typeof (3 + 4); // o/p :- Number
  typeof undefined           // undefined
  typeof null                // object

  null === undefined         // false
  null == undefined          // true
  Undefined and null are equal in value but different in type:
   ===> typeof operator can return one of these primitive types:
    string
    number
    boolean
    undefined

  ===> JavaScript objects are containers for named values called properties or methods.
  
  JavaScript variables can hold many data types: numbers, strings, objects and more:
  var length = 16;                               // Number
  var lastName = "Johnson";                      // String
  var x = {firstName:"John", lastName:"Doe"};    // Object
  var cars = ["Saab", "Volvo", "BMW"];           // JavaScript arrays are written with square brackets.
  // JavaScript objects are written with curly braces.
  var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
  The object (person) in the example above has 4 properties: firstName, lastName, age, and eyeColor.

When a JavaScript variable is declared with the keyword "new", the variable is created as an object:
var x = new String();        // Declares x as a String object
var y = new Number();        // Declares y as a Number object
var z = new Boolean();       // Declares z as a Boolean object
Avoid String, Number, and Boolean objects. They complicate your code and slow down execution speed.

  
  
Function calling ways:
==> When an event occurs (when a user clicks a button)
==> When it is invoked (called) from JavaScript code
==> Automatically (self invoked)
==> The var keyword tells the browser to create variables
// eg:- var x, y;
// create sample function
function myFunction(p1, p2) {
    return p1 * p2;
}
document.getElementById("demo").innerHTML = myFunction(4, 3); // o/p is "12"

Keyword                   	     Description
break	                 	==>      Terminates a switch or a loop
continue               	==>      Jumps out of a loop and starts at the top
debugger               	==>      Stops the execution of JavaScript, and calls (if available) the debugging function
do ... while	         	==>      Executes a block of statements, and repeats the block, while a condition is true
for	                  	==>      Marks a block of statements to be executed, as long as a condition is true
function	            	==>      Declares a function
if ... else	            ==>      Marks a block of statements to be executed, depending on a condition
return	               	==>      Exits a function
switch	               	==>      Marks a block of statements to be executed, depending on different cases
try ... catch	          ==>      Implements error handling to a block of statements
var	                  	==>      Declares a variable

Explicit Function Binding
==> The call() and apply() methods are predefined JavaScript methods.
call() and apply() are using to call the object method with another object as argument.

var employee = {
 name: function() {
  return this.firstName+" "+this.lastName;
 }
}

var employeeDetails = {
	firstName: "Niranjan",
    lastName: "Narendra"
}
// Here fist variable or argument method name .(dot) inside first variable avilable function .(dot) use call method of 
// second variable
var employeeDetailName = employee.name.call(employeeDetails);
document.getElementById("demo").innerHTML = employeeDetailName; 

// Create an object:
var car = {
type   :"Fiat",
model  :"sports car", 
color  :"Red",
weight :"400kgs", 
details: function() { // function declaration and returns color and weight values. Here "this" means current object reference.
return this.color+" "+this.weight;
}
};

// The object can call two ways i.e 
// car["weight"]
// car.model
// Display some data from the object:
document.getElementById("demo").innerHTML = car.details()+" "+ car.type+" "+car.model+" "+car["weight"]+" "+car["color"];

let keyword
==> Varables declared with the let keyword can have Block Scope. 
===> let keyword means local variable we can use both var and let inside the function.
var x = 10;
// Here x is 10
{ 
    let x = 2;
    // Here x is 2
}

==> debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.







