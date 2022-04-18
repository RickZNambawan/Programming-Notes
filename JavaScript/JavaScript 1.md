JavaScipt

FORMAT:
<!doctype.html>

<html>
<head>
</head>
<body>

<script type="text/javascript">


</script>

</body>
</html>
----------------------------------------------------------------------------------------
*INTRODUCTION IN JAVASCRIPT
<script type="text/javascript"> - code that must use for the web to read that you will be using to start java script
document.write("TEXT/NUMBER"); - (TEXT) that you can be written in text/number, with qoutation mark. ("")
<!--
	(CODES) - for making sure that your browser is updated and not old for the javascript to read by the browser. "CHECK"
//-->

// (text) - (SPECIAL COMMENT OR NOTE) - text that ignore by the browser or hidden text that is not shown by the browser.
--------------------------------------------------------------------------------------------------------------
*MATH OPERATORS
% - (PERCENTAGE) if you want to get the remainder in division.Example: 4/3 = 1.8888 ... so 4%3 = 2.
++ - if you want to add 1 in your variable. Example: var lol = 7; so lol++; = 8
-- - if you want to subtract 1 in your variable. Example var lol = 7; so lol--; = 6
--------------------------------------------------------------------------------------------------------------
*COMMENTS AND STATEMENTS
/*
(text) - (SPECIAL COMMENT) - text that ignore by the browser. Text that too long.
*/
--------------------------------------------------------------------------------------------------------------
*VARIABLES
var (variable) = ("value/number/can be negative/text"); - (VARIABLE)
Example: var x = "29";
	 document.write (x);
--------------------------------------------------------------------------------------------------------------
*DIFFERENT TYPES OF VARIABLES
var (variable) = ("\"(text)/""); - para mabasa ng browser na hindi value ang isa pang quotation mark sa text na value mo.
Example: var love = "hahahaha\ "laftrip nga men \"";
	document.write(love);
--------------------------------------------------------------------------------------------------------------
*USING VARIABLES WITH STRINGS
var (variable) = "(text/number)";
var (variable) = "(text/number)";
document.write((variable) + "(text)" + (variable))
Example: var love = "Fred";
	 var age = "17";
	 document.write(love + " is my name and my age is " + age);

Example: var pogi = "Fred";
	 var cute = "RickZ";
	 var macho = "Castaneda";
	 document.write(pogi+cute+macho);
--------------------------------------------------------------s------------------------------------------------
*FUNCTIONS
function (variable)() {
	 alert("(TEXT)");}
Example: function pogi() {
	 alert("WARNING: OMG!! ANG POGI NI FREDERICK CASTANEDA JR.!!!!!! ANG MACHO!");}
--------------------------------------------------------------------------------------------------------------
*USING PARAMETERS WITH FUNCTIONS
function (variable) (value/text){
	 alert("TEXT " + (variable));
}
	 (variable) ("(text)");
	 (variable) ("(text)");	
	 (variable) ("(text)");
Example: function pogi(x){
	 alert("HANDSOME " + x);
}
	 pogi("NGONGI");
	 pogi("Nhahaha");	
	 pogi("NYEK!");
--------------------------------------------------------------------------------------------------------------
*FUNCTIONS WITH MULTIPLE PARAMETERS
function (variable) (value,value) 
	 document.write ((value) + " (TEXT) " + (value) + "(html codes)");
}

	(variable) ("(value)","(value)");
	(variable) ("(value)","(value)");
	(variable) ("(value)","(value)");
Example: function pogi(one, two){
	 document.write(one + " is better than " + two + "<br/>");
}

	pogi("fred","castaneda");
	pogi("ngongi","shunga");
	pogi("atup","ogag");
--------------------------------------------------------------------------------------------------------------
*THE RETURN STATEMENT
function (variable) ((value,value)){
	var (another value) = (value+value);
	return "(value in "var")";
}
	document.write(variable (value,value,));
Example: function addnumbers (a,b){
	var c = a+b;
	return c;
}
	document.write(addnumbers(3,6));
--------------------------------------------------------------------------------------------------------------
*CALLING A FUNCTION FROM ANOTHER FUNCTION
function (variable)(){
	document.write(" (TEXT) ");
}
function (another variable)(){
	document.write(" (TEXT) ");
}

function (LAST VARIABLE)(){
	(1st variable)();
	(2nd variable)();
}

(LAST VARIABLE)();
Example: function doFirst(){
  	 document.write(" first! ");
}
	 function doSecond(){
	 document.write(" second! ");
}
	

	 function start(){
	 doFirst();
	 doSecond();
}
	
start();
--------------------------------------------------------------------------------------------------------------
*GLOBAL VARIABLES
var (variable) ="(value)";

function (variable)(){
	document.write(variable in the var);
}

(Variable in the function)(){
	document.write(variable in the var);
Example: var boy = " FRED ";
	
	 function lol(){
	 document.write(boy);
}

	 lol();
	 document.write(boy);
--------------------------------------------------------------------------------------------------------------
*LOCAL VARIABLES
function (variable){
	var (variable) ="(value)";
	document.write (variable in var);

}

	(variable in function);

	document.write(variable in var);
Example: function lol(){
	var boy = " FRED ";
	document.write(boy);
}
	
	lol();
	document.write(boy);
--------------------------------------------------------------------------------------------------------------
*MATH OPERATORS
	var (variable) = (value/number);
	(variable)(sign);

	document.write(variable);
% - (PERCENTAGE) if you want to get the remainder in division.
var lol = 4/3;
	lol;
	document.write(lol);
Example: 4/3 = 1.8888 ... so 4%3 = 2.

++ - if you want to add 1 in your variable.
var lol = 7;
	lol++;
	document.write(lol); 
Example: var lol = 7; so lol++; = 8

-- - if you want to subtract 1 in your variable.
var lol = 7;
	lol--;
	document.write(lol);
Example var lol = 7; so lol--; = 6
--------------------------------------------------------------------------------------------------------------
*ASSIGNMENT OPERATORS
	var (variable) = (value/number);
	(variable) (sign)= (another value);

	document.write(variable);
Example: var fred = 29;
	 fred -= 3;

	document.write(fred)
Another Example: var lol = 7;
	lol += 31;
	lol -= 12;
	lol *= 4;
	lol /= 5;
	
	document.write(lol);
so it = 20.8
--------------------------------------------------------------------------------------------------------------
*IF STATEMENTS
var (variable) = (value/number);
var (another variable) = (value/number);

if (first variable==second variable){
	document.write ("(TEXT)");
}
Example:var pogi = 26;
 	var fred = 262;
	
	if (pogi!==fred){
	document.write("LAFTRIP HAHAH");
}
Example:var pogi = 26;
	var fred = 262;
	
	if (pogi!+=fred){
		document.write("LAFTRIP HAHAH");
	}
! - (IF NOT EQUAL TO)
Note: All signs can be use in " (sign)= ". If less than sign or greater than sign is used, the equal sign need to delete.
--------------------------------------------------------------------------------------------------------------
*IF/ELSE STATEMENTS
var (variable) = (value/number);
var (another variable) = (value/number);

if ((first variable)==(second variable)) {
	document.write("text");
}
else { 
	document.write("text");
}
Example:var pogi = 22;
	var fred = 22;
	
if (pogi==fred) {
	document.write("SUCCESS");
}
else {
	document.write("FAILED");
}
Example: if (2!=2) {
	document.write("SUCCESS");
}
else {
	document.write("FAILED");
}
--------------------------------------------------------------------------------------------------------------
*NESTING
var (variable) = "(value)";
var (another variable) = "(value)";

if (1st variable=="(1st value)"){
	if (2nd variable=="(2nd value)"){
	document.write("(TEXT)");
}else{
	document.write("(TEXT)");
   }
}
Example: var firstname = "frederick";
	 var lastname = "castaneda";

if (firstname=="frederick"){
	if (lastname=="castaneda") {
		document.write("hahahaha ansaya lang");
	}else{
		document.write("hahahaha ansaya lang tlga hahaa");
    }
}
--------------------------------------------------------------------------------------------------------------
*COMPLEX CONDITIONS
var (variable) = "(value)";
var (another variable) = "(value)";

if ( ((variable=="(first value)") && OR || ((another variable=="(second value)" ){
	document.write("(TEXT)");
}

Example of &&: (ALL MUST BE TRUE)
var first = "frederick";
var last = "castaneda";

if (first=="frederick") && (last=="castaneda") ){
	document.write("hahahahahaah");
}

Example of ||: (ONE CAN ONLY BE TRUE)
var first = "frederick";
var last = "castaneda";

if (first=="pogi") && (last=="castaneda") ){
	document.write("hahahahahaah");
}
--------------------------------------------------------------------------------------------------------------
*SWITCH
var (variable) = "(value)";

switch(value){
	case "(value)":
		document.write("(TEXT)");
		break;
	case "(value)":
		document.write("(TEXT)");
		break;
	default:
		document.write("(TEXT)");
	}
Example: var girl = "lyka";

   	 switch(girl){
		case "lyka":
			document.write("she's so perfect");
			break;
		case "liza seberano":
			document.write("my ex hahaaha");
			break;
		default:
			document.write("hahahahaha laftrip");
	}
--------------------------------------------------------------------------------------------------------------
*for LOOP
for((VARIABLE)=(VALUE);(VARIABLE AGAIN)<(VALUE);(VARIABLE AGAIN AND AGAIN)++){
	document.write("(TEXT) <br />");
}
Example: for(x=5;x<350;x++){
 		document.write("hahahahahahahaha <br />");
	}
--------------------------------------------------------------------------------------------------------------
*while LOOP
var (VARIABLE) = (VALUE);
	
while((VARIABLE)<(VALUE)){
	document.write( (VARIABLE) +  "	(TEXT) <br />");
	x++;
}
EXAMPLE:var x = 1;
	
	while(x<10){
		document.write(x +  "	cute is me <br />");
		x++;
	}
--------------------------------------------------------------------------------------------------------------
*do WHILE
var (VARIABLE) = (VALUE);
				
do{		
	document.write( (VARIABLE) + "(TEXT) <br />");
	x++;
}while( (VARIABLE) <= (VALUE));
Example: var x = 10;
				
do{		
	document.write(x + "haha <br />");
	x++;
}while(x<=20);
--------------------------------------------------------------------------------------------------------------
*EVENT HANDLERS
<form>
	<input type="button" value="(VALUE)" onClick="alert('(TEXT)');
	alert('(TEXT)');"/>
</form>
Example: 
<form>
	<input type="button" value="LOL me" onClick="alert('hahahaha');
	alert('lol');"/>
</form>
--------------------------------------------------------------------------------------------------------------
*OnMouseOver
<a href="(WEBSITE)" onMouseOver="alert('(TEXT)')";> (TEXT) </a>
Example:
<a href="http://facebook.com" onMouseOver="alert('rak na')";> CLICK ME </a>
--------------------------------------------------------------------------------------------------------------
*onUnload
<body onUnload="alert('(TEXT)');">
Example: 
<body onUnload="alert('GOODBYE FUCKERS');">
--------------------------------------------------------------------------------------------------------------
*OBJECTS
	var (PROPERTIES) = "(TEXT)";
	document.write ((PROPERTIES).(METHOD));
Example:
	var fred = "hahahahahahaha";
	document.write (fred.length);
--------------------------------------------------------------------------------------------------------------
*Creating own OBJECTS/CONSTRUCTOR FUNCTION
<html>
<head>
<script>
	function pogi(name, age){
		this.name = name;
		this.age = age;	
	}
	
	var fred = new pogi("Frederick Castaneda", 17);
	var lyka = new pogi("Mary Lyka Gomez Agad", 16);
</script>
</head>
<body>
<script>
	document.write(fred.name);
	document.write(lyka.name);
</script>
</body>
</html>
--------------------------------------------------------------------------------------------------------------
*OBJECT INITIALIZERS
<html>
<head>
<script>
	fred = {name:"FREDERICK CASTANEDA", age:17};
	lyka = {name:"MARY LYKA AGAD", age: 16};
</script>
</head>
<body>
<script>
	document.write (fred.name + " LOVES " + lyka.name + " BECAUSE OF " + lyka.age);
</script>
</body>
</html>
--------------------------------------------------------------------------------------------------------------
*Adding METHODS to OBJECTS
<html>
<head>
<script>
	function animals(name, age){
		this.name = name;
		this.age = age;	
		this.calculation = livingyears;
	}
	
	function livingyears(){
	var SUBTRACTION = 200 - this.age;
	return SUBTRACTION;
	}
	
	var dog = new animals("SHITZU", 28);
	var fred = new animals("LOL", 32);
	
</script>
</head>
<body>
<script>
	
	document.write(fred.calculation());
	
</script>
</body>
</html>
--------------------------------------------------------------------------------------------------------------