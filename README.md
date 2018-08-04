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

==> .then() function has been included to pure javascript.
==> The then() method returns a Promise. It takes two arguments: callback functions for the success and failure cases of the Promise.
==> then is a method used to solve Asynchronous callbacks

==> We need to write "document.write()" javascript file starting line.
document.write("someone learn");
==> Need to show one alert dialog with ok button use ==> "alert("")"

==> Function call and taken value from edit text when button click
<script type="text/javascript">
function greetUser(){
    var userInput = document.getElementById('userName').value;
    document.getElementById('greeting').innerHTML = 'Hello, ' + userInput;
}

function getCouseName() {
  var welcomeText = document.getElementById("courseName").value;
  document.getElementById("p_welcome_text").innerHTML = welcomeText;
}
</script>
==> HTML code for the creation of edit text and button functionality.
<p id='greeting'>Welcome</p>
<p id="p_welcome_text" > Welcome Java Script </p>
<input type="text" id="courseName" value="Enter course name" />
<input type='text' id='userName' value='Enter Your Name' />
<input type='button' onclick='greetUser();' value='Say Hello'/>
<input type="button" onclick="getCouseName()" value="Say course name" />

==> Try to place the comments for every line or function to make it as clear.
==> 1. In the above script we have taken two textviews and two edit texts and two buttons.
==> 2. when we click the button we need to take the edit text value and assign to the textview (or) p tag --> paragraph tag

==> Try to compare the Javascript with android to get more clarity on it.
==> In android we can take one button in XML and with onClick() attribute and implenting the functionality in the .java file and taking the edit text values and all form the unique ids after that user entered value can assign to the textview.

==> Creating super class Animal and extracting into the sub class. Super class will be called by call.
<script type="text/javascript">
function useStringObject() {
    var strObject = new String("Narendra");
    // document.write("Employee name is > " + strObject + " Name length is > "+strObject.length
    // +" Upper case letter are > "+strObject.toUpperCase());
    alert("Employee name is > " + strObject + " Name length is > "+strObject.length
    +" Upper case letter are > "+strObject.toUpperCase());
}

function useDateObject() {
  var dateObject = new Date();
  alert(dateObject.getDate()+" "+dateObject.getMonth()+" "+dateObject.getFullYear());
}

// When click on "Create Animal Object" button this createAnimalObject method called.
function createAnimalObject() {
	var animalObject = new Animal("Different Sound"); // creating Animal object
	animalObject.talk("wow !", "Some One");			  // calling talk method with animal object
	animalObject.walk();							  // calling walk method with animal object
}

// creating the Animal object constructor with one parameter
// In java or other classes we can create class and its methods but in javascript it is different.
// When new Animal("") ==> is called --> The animal object created with parameter.
function Animal( animalName ) {
	this.name = animalName; 			// taking the constructor parameter to local variable
	this.talk = sayAnimalInformation;   // Here <sayAnimalInformation> means function assigning to 
										// the this.talk method. Here this is object talk is method. 				 
}

// Animal object standard alone function declaration.
function sayAnimalInformation(animalSound, animalName) {
	alert(animalSound+" "+"Animal name is > "+animalName);
}

// Animal object prototype function declaratioin.
Animal.prototype.walk = function() {
	alert("walk can fast");
}

// =========== sub class creating and accessing the super class methods and properties. ==========

function createDogObject() {
	var dogObject = new Dog("Fidda");   // creating Dog object with name parameter inside constructor.
	dogObject.talk("Woww! ", dogObject.name);          // calling talk method with dog object. 
	dogObject.eat();
}

function Dog(dogName) {
	Animal.call(this, dogName); // Calling super class object by using the call method.
	this.eat = dogEatFood;      // Calling the dogEatFood() method.
}

function dogEatFood() {
	alert("Dog eat bisckets >> ");
}


function createCatObject() {
	var catObject = new Cat("Pinki");
	catObject.talkSound("Meyavuu > ", catObject.name, "Brown");
	catObject.catEatFood();
}

function Cat(catName) {
	this.name = catName;
	this.talkSound = catSoundFunction;
}

function catSoundFunction(catSound, catName, catColor) {
	var result = catSound;
	alert(result +" "+ "Cat name is > "+ catName + " Cat color is > "+catColor);
}

Cat.prototype.catEatFood = function() {
	alert("cat eats milk rice > ");
}
</script>

<input type='button' onclick='useStringObject();' value='Create String Object'/>
<input type="button" onclick="useDateObject()" value="Create Date Object" />
<input type='button' onclick='createAnimalObject();' value='Create Animal Object'/>
<input type="button" onclick="createDogObject()" value="Create Dog Object" />
<input type="button" onclick="createCatObject()" value="Create Cat Object" />








