HTML - HYPER TEXT MARKUP LANGUAGE

<doctype html> - (VALID) Unang tag sa pag gawa ng website. Lalo kung ito ay document
<html> - Para makagawa ng WEBSITE.
</> - (END TAG) 
<head> - Mga bagay na hindi makikita sa surface ng Website.
<title> - (TITLE) Pamagat ng website na hindi makikita sa surface ng website kundi sa itaas lamang.
<style> - (STYLE) Use only for Creating CSS.
<style type="(CODE FOR CSS)"> - A code for starting CSS.
<body> - (BODY) Ito na ang makikita sa surface ng website.
<h1> - (HEADER) o title na makikita sa surface ng website. (LARGE TEXT)  (BOLD)
<h2> - (HEADER) o title na makikita sa surface ng website. (MEDIUM TEXT) (BOLD)
<h3> - (HEADER) o title na makikita sa surface ng website. (SMALL TEXT)  (BOLD)
<p> - (PARAGRAPH) Para makapag sulat ng mga text sa body ng topic.
<br /> - (LINE BREAK) Space down para sa next line. 
<hr /> - (HORIZONTAL ROW) LINE BELOW NG TOPIC.
<strong> - (BOLD TEXT) Pagpapalaki ng font sa text ng paragraph.
<em> - (EMPHASIS) pagiging italic font ang text.
<i-- "text" --> - (SPECIAL COMMENT) Walang makakakita at hindi makikita sa site. "Note"
<a> (ANCHOR) - LINK or HYPERLINK
<a href="(website)"> - (HYPERLINK REFERENCE) the location of the website that you wanted to locate.
<a name="(SOMEWHERE OF YOUR SITE)"> - (HYPERLINK REFERENCE) the location of the topic that you wanted to locate or the target location.
<a href="#(SOMEWHERE OF YOUR SITE)"> - (HYPERLINK REFERENCE) the link of the topic that you wanted to locate.
<a href="mailto:(EMAIL ADDRESS)"> - link to someone's email address. (WILL POP UP THE EMAIL APP)
<a href="(WEBSITE)" title="(TEXT)" - Add tool tip to the link.
<img src="(NAME OF THE PHOTO FILE"/> - (IMAGE SOURCE) Image you want to see on your website.
<img src="(NAME OF THE PHOTO FILE" height="(NUMBERS)"/> - to resize and adjust the image.
<table> - (TABLE) CREATE TABLE
<tr> - (TABLE ROW) CREATE TABLE ROW
<td> - (TABLE DATA) CREATE COLUMN
<table border="(NUMBERS)"> - border of your table/ how thick the stroke.
<table border="(NUMBERS)" width="(NUMBERS)"> - can adjust the width of table./CAN ALSO ADJUST IN PERCENTAGE (%)
<table border="(NUMBERS)" cellpadding="(NUMBERS)"> - Can give you space between a text and a border.
<table border="(NUMBERS)" cellspacing="(NUMBERS)"> - Can have space between the cells themselves.
(NOTE: YOU CAN ADD IMAGE IN THE TABLE)
<th> - (TABLE HEADER) Your Title in your table AND can be bold font.
<th colspan="(NUMBERS)"> - (COLUMN SPAN) You can expand in 1 column the text.
<ul> - (UNORDER LIST) make your paragraph or text bulleted.
<ol> - (ORDER LIST) make your paragraph or text numbered.
<li> - (LIST ITEM) Item on your list.
<span> - (SPAN) is the key word for you to select specific text that you only want to affect.
<div> - (DIVISION) You can position specific element using this keyword.
# - use for ID only.
<(ELEMENT) id="(NAME OF THE POUND (#) IN YOUR CSS)"> - (ID) You can position ANY elements in your site.
<(ELEMENT) class="(NAME OF THE DOT (.) IN YOUR CSS)"> - (CLASS) You can select specific ELEMENT that you only want to affect.
. - use for the CLASS only.
ON CSS or <style>:
(ELEMENT) > (ELEMENT) - (PARENT TO CHILD) You can change the effect of the CHILD in the PARENT element.

---------------------------------------------------------------------------------------------
SPECIAL CODE:
<form> - YOU CAN CREATE FILL UP FORM OR LOGGING SHEET.
---------------------------------------------------------------------------------------------
SPECIAL CODE: 
<form>
(TEXT): <input type="type" name="(text)" size="(NUMBERS/PIXEL)" maxlength="(NUMBERS)" value="(Text)"/>
</form>

EXAMPLE:
<form>
  USERNAME: <input type="type" name="text" size="30" maxlength="20" value="ENTER NAME HERE"/>
</form>
---------------------------------------------------------------------------------------------------
SPECIAL CODE: 
<form>
(TEXT): <input type="radio" name="(text)" value="(text)"/>
</form>

EXAMPLE:	  
<form>
  Male: <input type="radio" name="sex" value="male"/>
  Female: <input type="radio" name="sex" value="female"/>
</form>	
---------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
(TEXT) <input type="checkbox" name"(text)" value="(text)"/>
</form>

EXAMPLE:
<form>	
               <p> BASTA ALAM MO NA YAN ZZZZ! -_- </p>
	POGI <input type="checkbox" name="food" value="pogi"/>
	LOVE <input type="checkbox" name="food" value="love"/>
	HART <input type="checkbox" name="food" value="hart"/>
	HURT <input type="checkbox" name="food" value="hurt"/>
</form>
----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
(TEXT): <input type="password" name="(text)"/>
</form>

EXAMPLE: 
<form>
Password: <input type="password" name="Pword"/>
</form>
----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
<select name="(text)">
	<option value="(text)"> (TEXT) </option>
</select>
</form>

EXAMPLE:
 What are your hobbies in your useless life?
	<select name="activities">
		<option value="play"> PLAYING DOTA 2 </option>
		<option value="study"> STUDYING </option>
		<option value="website"> MAKING WEBSITE </option>
		<option value="laftrip"> LAFTRIP ALWAYS </option>
	</Select>
</form>
----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
<textarea name="(text)"
	  rows="(numbers)"
	  cols="(numbers)">
(TEXT)
</textarea>

EXAMPLE:
<form>
Make a 3 paragraph that answers why you love me very much?
<br/>
 <textarea name="bio"
	   rows="20"
	   cols="50">
 WHAT'S ON YOUR FUCKING MIND?
 </textarea>
</form>
----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
	<input type="file" name="(text)"/>
</form>

EXAMPLE:
<form>
	<p> NOW SUBMIT A FILE! </p>
	<input type="file" name="FRED FILE"/>
</form>
-----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
	<input type="submit" value="(text)"/>
</form>

EXAMPLE:
<form>
	<input type="submit" value="SUMBIT HERE!"/>
</form>
-----------------------------------------------------------------------------------------------------
SPECIAL CODE:
<form>
	input type="button" value="(text)"/>
</form>

EXAMPLE:
<form>
	input type="button" value="CLICK ME"/>
</form>
EXAMPLE ONLY FOR JAVASCRIPT:
<form>
	<input type="button" value="(TEXT)" onclick="(VARIABLE)()"/>
</form>
-----------------------------------------------------------------------------------------------------
SPECIAL CODE FOR PHP:
<form action="dosomething" method="post">
-----------------------------------------------------------------------------------------------------