*STRUCTURE OF JAVASCRIPT IN PAGE-LEVEL*
In <head> element:
<head>
	<script type="text/javascript"> </script>
</head>

In <body> element:
<body>
	<script type="text/javascript">

	</script>
</body>

*Structure of JavaScript in External Link:
<head>
	<script type="text/javascript" src="(name of the file)" />
</head>
-----------------------------------------------------------------------------------------

Syntax Punctuation:
// - one line comment.
/* */ - multi-line comment.
\n - new line.
; (semi-colon) - Each command must end with this. Indicates the end of a line.
"" (String data) - It refers to the word text. Text is stored in computer memory.
\ (Backslash) - Multi-line strings. Add to the end of a line.
+ (Concatenation) - Using the plus sign to combine text. Combining variables with literal text in one line. 
. (Period) - Object and a variable are connected by a period.


Conditional Operators:
== (Double equal sign) - used to represent equality.
< (Less than sign) 
> (Greater than sign)
<= (Less than or Equal sign) 
>= (Greater than or Equal sign) 
!= (Not Equal sign)


Definition of Terms:
Object - collection of properties. A property's value can be a function, in which case the property is known as a method.
Property - is an association between a name and a value. 
Method - are the actions that can be performed on objects.
Fuction - are simply a collection of code lines with a name.
Parameter - a value sent to a function.
Argument - text or variable inside the parentheses of a function/method.
Integers - whole number or number with no decimal part. Can be positive or negative.
Float - number with decimal part. Can be positive or negative.
String - values that usually enclosed in quotes
Boolean - can only be true or false.
Document Object Model (DOM) - special set of complex variables that encapsulates the entire contents of the web page.
Reference - an indicator where the specified object is in memory. You can store a reference in a variable.
Condition - an expression that can be evaluated as true or false. Conditions are often comparisons.
Global variable - available at the main level and inside each function. If you want to used in multiple functions.
Local variable - has meaning only inside the function.
Class - a pattern for generating objects.
Constructor Function - is a special method for creating and initializing an object created with a class .
JSON - comma-separated list of name-value pairs wrapped in curly braces.
Regular Expression - a powerful mini-language for searching and replacing text patterns.

Element/Keyword: 
var - simply places in memory for holding data. It store your information in it.
fuction - allows you to collect one or more commands and give them a name.
return - When you want a function to return some value to the main program.
if - If the condition is true, all of the code in the following set of braces is executed. 
else - indicate you will have a second code block that will execute only if the condition is false.
switch - useful alternative when you have a number of discrete values you want to compare against a single variable.
case - to indicate a case.
break - This indicates that you’re done thinking about cases, and it’s time to pop out of this data structure.
default - traps for any values of the variable that were not explicitly caught.
counter variable - controls the iterations of a loop.
for - special loop used to repeat something a certain number of times.
while - When the condition is true, the loop continues; if the condition is evaluated as false, the loop exits.
Array - groups of variables with a name.
Object - collection of properties.
new - creates an instance of a user-defined object type or of one of the built-in object types that has a constructor function. Creating new object.
this. - to access the properties of the object. It refers to the property of the current object. 


Modal Dialog Methods:
alert() - pops up a small dialog box containing text for the user to read.
prompt() - expects you to ask the user a question. To get data from the user


Data type Methods:
parseInt() - used to convert variable text data to an integer.
parseFloat() - converts variable text data to a floating-point value.
toString() takes any variable type and creates a string representation.
eval() - special method that accepts a string as input.


Strings Methods:
.toUpperCase() - makes an entirely uppercase copy of the string.
.toLowerCase() - makes an entirely lowercase copy of the string.
.substring() - returns a specific part of the string.
.indexOf() - determines whether one string occurs within another.
.match() -  searches a string for a match against a regular expression.


Floating Methods:
Math.ceil() - always rounds upward the floating number.
Math.floor() - always rounds downward the floating number.
Math.round() - always rounding number based on the decimal.


String Object Properties:
.length - returns the length of the string in characters.


Boolean Object Properties:
.selected - tells you whether the object on select element has been highlighted by the user. It's either true or false.
.checked - determine whether the check box is checked.

HTML Input fields Object Properties:
.value - You get the user input and assign it on a variable. You can read this value as an ordinary string variable.

Array Object Properties: 
.length -  returns the number of elements in an array.


DOM HTML properties:
.innerHTML - allows you to change the HTML code displayed by the html tags.


Objects:
window - has a huge number of subobjects, all listed in the DOM view.


DOM Variable of window Object:
document - Most commonly scripted element.
location - Change location.href to move to a new page
history - Access this to view previous pages
status - Change this to set a message in the status bar


DOM document methods:
document.getElementById() - This beauty searches through the DOM and returns a reference to an object with the requested ID.
document.getElementsByName() - returns a collection of all elements in the document with the same specified value of name attribute.
document.body.style.backgroundColor = "color" - Change the background color of the current element.


Event Handler on HTML Attribute:
<input type="button" onclick = "(js action/function)" /> - The action assigned will happen each time the button is clicked.
<body onload="(js function)"> - a function that will automatically run after the page load.
<select onchange="(js function)"> - automatically change the value of the selected element.














Fuction structure without parameters:
fuction variable () {
	//some commands;
}

Conditions Structure:
If Statement:
if (condition) {
   *statement*
}

If-else Statement:
if (conditionn) {
   *statement*
} else {
   *statement*	
}


else-if Statement:
if (condition) {
   *statement*
} else if (condition) {
   *statement*	
}


Switch Statement:
switch (variable) {
   case (condition):
     *statement*;
     break;
   default:
     *statement*;
}

Loops:
For loop:
for (initialization; condition; update) {
	*statements*
}

While loop:
while (condition) {
	*statements*
}

Array Kinds of Structure:
*Single-Dimensional Array
1. var nameOfVariable = new Array(3);

	nameOfVariable[0] = "String";
	nameOfVariable[1] = 12;
	nameOfVariable[2] = true; 

2. var nameOfVariable = new Array ();
	nameOfVariable[0] = "String";
	nameOfVariable[1] = 12;

3. var nameOfVariable = new Array("String", 12, true);

*Two-Dimensional Array
1. Array inside of an Array
var nameOfVariable = new Array(
	new Array = ("String", 12, true),
	new Array = (12, true, "String"),
	new Array = (true, "String", 12)
);

nameOfvariable[row][column];


Creating New Object:
var nameOfVariable = new Object();

Adding Properties to the Object:
var nameOfVariable = new Object();
nameOfVariable.name = "String";
nameOfVariable.age = 18;
nameOfVariable.bool = true;

Adding Methods to the Object():
var nameOfVariable = new Object();

namOfVariable.nameOfTheFunction = function () {
	this.nameOfProperty1 = "String";
	this.nameOfProperty2 = 18;
	this.nameOfProperty3 = true;
}


Creating JSON (JavaScript Object Notation):

var nameOfVariable = {
	property1: "String",
	property2: 18,
	property3: true
};

alert(nameOfVariable.property1.property3);
alert(nameOfVariable.["property1"]["property3"]);
alert(nameOfVariable.["property1"].property2);

Regular Expressions Format:
	*RESEARCH ABOUT IT FOR MORE INFO!!!!!*