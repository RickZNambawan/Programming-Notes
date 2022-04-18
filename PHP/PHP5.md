*BASIC STRUCTURE OF PHP (PHP HYPERTEXT PRE-PROCESSOR)*
<?php 
   print "Hello World!";
   print 'Hello World!';
   print ("Hello World!");
   print ('Hello World!');
   // or
   echo "Hello World!";
   echo 'Hello World!';
   echo ("Hello World!");
   echo ('Hello World!');
?>

---------------------------------------------------------------------------------------------------------------------
Syntax Punctuation:
// - one line comment
<<< HERE (Multi-Line Quote) - you make your own custom quotation mark from any value that you want
"" (Double-Quote) - give PHP permission to analyze the text for special characters.
'' (Single-Quote) - do not allow double-qoute behavior, which is why they are rarely used in PHP programming.
$ (variable) - A variable in PHP always begins with a $.
. (Concatenation) - to join two strings.
+ (Addition) - attempts to perform mathematical addition.
.= (Append) - appending something to a string variable. 
= (Assignment) - assigning a value to a variable.
=> (Associative Relationship) - helps PHP recognize you’re talking about an associative array lookup:

Comparison Operators:
== (Double equal sign) - used to represent equality.
< (Less than sign) 
> (Greater than sign)
<= (Less than or Equal sign) 
>= (Greater than or Equal sign) 
!= (Not Equal sign)


Definition of Terms:
Server-side Programming - is what you use to create pages dynamically on the server before sending them to the client.
Client-side Programming - oes most of the work on the individual user’s machine. Can be interactive in real time.
Compiled languages - are typically very fast but not very flexible.
Interpreted languages - have to be interpreted on the spot by the server every time they’re called, which is slower but provides more flexibility.
Loose Typing - When creating variable. PHP automatically makes the variable whatever type it needs. 
Concatenation - is the process of joining smaller strings to form a larger string.
Interpolation - can freely put variables inside string values, it will automatically replace that variable with its value.
heredocs - a type of multiline quote, usually beginning and ending with the word HERE.
Condition - can be comparisons of one variable to another, they can be functions that return a true or false value.
Typecasting - forces variables to the type you want before comparing variables.
Associative Arrays - are used when you want to work with data that comes in name/value pairs.
Multi-dimensional Array - is an array that holds arrays.


Keywords/Elements:
print - returns a value. Can be used as part of a complex expression.
echo - doesn't return a value. Can't be used as part of a complex expression.
if - If the condition is true, all of the code in the following set of braces is executed. 
else - indicate you will have a second code block that will execute only if the condition is false.
switch - useful alternative when you have a number of discrete values you want to compare against a single variable.
case - to indicate a case.
break - This indicates that you’re done thinking about cases, and it’s time to pop out of this data structure.
default - traps for any values of the variable that were not explicitly caught.
if - If the condition is true, all of the code in the following set of braces is executed. 
else - indicate you will have a second code block that will execute only if the condition is false.
counter variable - controls the iterations of a loop.
for - special loop used to repeat something a certain number of times.
while - When the condition is true, the loop continues; if the condition is evaluated as false, the loop exits.
foreach - is a special version of the for loop that simplifies working with arrays.
fuction - allows you to collect one or more commands and give them a name.
return - When you want a function to return some value to the main program.
global - to let your program know you are accesing to variable outside the function.


Function:
date() - returns the current date with a specific format.
filter_input(INPUT_GET/INPUT_POST, "(name attribute)") - for GET method or POST method. Use for extracting the data from the form element.
filter_has_var(INPUT_GET/INPUT_POST, "(name attribute)") - determine whether a particular variable exists. It returns true if the variable exists and false if it doesn’t.
rand("beginning number", "end number") - creates a random integer between beginning and end number.
array() - is a variable that holds multiple values that are mapped to keys.
print_r($variable of an array) - It allows you to pass an entire array, and it prints out the array in an easy-to-read format.
sizeof() - returns the number of elements in an array.
explode("delimiter", $nameOfVariable) - splits the string into an array based upon that one parameter.
preg_ split("regularExpression", $nameOfVariable) - look for multiple different delimiters stored in a regular expression, and break it into an array based on the delimiters you specify.


HTML Form Attributes and Values:
name="(text)" - form element to be passed to the server. This will be used by the PHP program to extract the information from the form.
<form action="(php file)"> -  used to determine which program should receive the data transmitted by the form.
<form method="get"> - gathers the information in your form and appends it to the URL.
<form method="post"> - passes the data to the server through a mechanism called environment variables. It is more secured than get method. Not attached on URLs
<input type="submit"> - to ensure the button sends the data to the server.
<button type="submit"> - to ensure the button sends the data to the server.


Escape Sequences:
\n - creates a new line in the resulting HTML.
\t - creates a tab in the resulting HTML.
\$ - creates a dollar sign in the resulting HTML.
\" - creates a double quote in the resulting HTML.
\' - creates a single quote in the resulting HTML.
\\ - creates a backslash in the resulting HTML.


Standard PHP Filters:
FILTER_SANITIZE_STRING - Strips tags, encodes or removes special characters.
FILTER_SANITIZE_SPECIAL_CHARS - Converts HTML special characters (<>&) with ASCII equivalents.
FILTER_SANITIZE_EMAIL - Removes any characters not allowed in an e-mail address.
FILTER_SANITIZE_URL - Removes any characters not allowed in a URL.
FILTER_SANITIZE_NUMBER_INT - Removes all characters but numeric digits and sign (+/-) symbols.
FILTER_SANITIZE_NUMBER_INT - Removes all characters but numeric digits, periods, commas, and sign (+/-) symbols.
FILTER_VALIDATE_INT - True if input is an int.
FILTER_VALIDATE_FLOAT - True if input is a floating point value.
FILTER_VALIDATE_BOOLEAN - True if input can be read as a Boolean (true/false, on/off, yes/no, 1/0). Returns NULL if input is non-Boolean.
FILTER_VALIDATE_URL - True if input is a legal URL (doesn’t check the address).
FILTER_VALIDATE_EMAIL - True if input is a legal e-mail address (doesn’t check the address).
FILTER_VALIDATE_IP - True if input is a valid IP address (doesn’t check the address).
FILTER_VALIDATE_REGEXP - True if input matches a given regular expression.




print/echo Statement Structure:
   print "Hello World!";
   print 'Hello World!';
   print ("Hello World!");
   print ('Hello World!');

heredocs Structure:
<<< (Superquoute or any text symbol)
	*statements*
(Superquote);

date() Structure and Format Function:
date("m/d/y");

date() format function:
d - day of the month (numeric)
D - three character abbreviation of weekday (Wed)
m - month (numeric)
M - three-character abbreviation of month (Feb)
F - text representation of month (February)
y - two-digit representation of the year (08)
Y - four-digit representation of the year (2008)
h - hour (12 hours)
H - hour (24 hours)
i - minutes
s - seconds

Typecasting:
(integer) variable
(float) variable
(string) variable
(boolean) variable

Conditions Structure:
If Statement:
if (condition) {
   *statement*
}

If-else Statement:
if (condition) {
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

Foreach loop:
foreach($variableOfArray as $sentryVariable) {
	print $sentryVariable;
}

Array Structure:
1. $variable = array();
	$variable[0] = "zero";
	$variable[1] = "one";
	$variable[2] = "two"; 

2. $variable = array("zero", "one", "two", "three");


Associative Arrays Structure:
$variable = array();
	$variable["name"] = "fred";
	$variable["address"] = "Pasig City";
	$variable["email"] = "frederick_004@yahoo.com";
  print $variable["name"];

Associative Arrays with foreach Loop:
foreach($nameOfArray as $key => $value) {
	print "<dt> $key </dt>";
	print "<dd> $value </dd>";
}

Two-Dimensional Array:
$nameOfArray = (
    array(0, 1, 2, 3),
    array(0, 1, 2, 3),
    array(0, 1, 2, 3),
    array(0, 1, 2, 3)
);

Fuction structure without parameters:
fuction $nameOfVariable () {
	//some commands;
}