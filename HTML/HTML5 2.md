Basic Structure of HTML:
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8" xmlns="http://www.w3.org/1999/xhtml"/>
    <title> </title>
</head>
<body>

</body
</html>

---------------------------------------------------------------------------------------------------------------------
<meta http-equiv="refresh" content="0"
<element> (tag) - this is tag. Element is inside the tag. TAG AND ELEMENT ARE THE SAME THING!
attribute="[value]" (attribute) - special modifier that can attach to some tags
Inline tag - inline elements do not force a new line to begin in the document flow. only takes up as much width as necessary.
Block tag - typically cause a line break to occur.

<!-- --> - one line/multi-line comment in HTML.
</br> - line break.
<hr /> - horizontal line.


Anchor:
<a> (anchor) -  linking a hyperlink.
attributes:
href="[link]" (hypertext reference) - indicates web adress/URLS or where it will go next.

Absolute Reference - links outside of your website. Usually begin with web protocol "http://
Relative Reference - links inside of your website. Same directory of main website.

Parts of the URL/URI (Uniform Resource Locators/Identifier):
Protocol - "http://"
Host name - "www"
Subdomain - http://www.("subdomain").com
Domain Name - ".com" ; 3-letters organization ".uk" ; 2-letters country
Page Name - http://www.facebook.com/index.html ("full web address")
Username - /"~fred"/index.html (name of the user of the web)

Lists:
<ul> (unordered list) - bulleted
<ol> (ordered list) - numbers
<li> (list item) - items on a lists.

<dl> (description list) - to create name and value
<dt> (description/definition term) - words or a phrase
<dd> (definition data) - description of definition

Table:
<table> (table) - to create a whole table
<tr> (table row) - row of cell in a table. Creating row
<th> (table header) - header of a table every row. Goes to Column
<td> (table data) - description inside the cell. Goes to Column
attributes:
rowspan="[numbers]" (row span) - how many row do you want to expand
colspan="[numbers]" (column span) - how many column do you want to expand

Image:
<img> (image) - allows you to grab an image file.
attributes:
src="[URL/file name with format]" (source) - allows you to indicate the URL of the image.
height="[numbers]" - for sizing.
weight="[numbers]" - for sizing
alt="[text]" (alternate text)- alternate text describing the image for easy searching. Required for all images.

Audio: (New feature on HTML5)
<audio> (audio) - indicates where an audio file will be placed
<source> (source) - indicates a file you will link to.
attributes:
controls="[controls]" (controls) - to show some control panel to the audio.
type="[format]" (type) - 
src="[file name with format]" (source) - indicate the file name of the audio file you wish to play.

Video:
<video> (video) - 
attributes:
src="[file name with format]" (source) - indicate the file name of the video file you wish to play.
controls="[controls]" (controls) - to show some control panel to the video.

Forms:
<form> (form) - container for form elements.
<input> (input) - the user types a data into these elements.
<fieldset> (fieldset) - for having layout for the form elements like having a container.
<legend> (legend) - allows you to specify a legend for the entire <fieldset>,
<label> (label) - allows you to specify a particular text as a label.
attributes of <label>:
for="#id of the checkbox" -  connects each label to the corresponding check box.

attributes:
action="[for programming languages]" (action) - don't have for the mean time.
type="[types of input]" (type) - indicates the type of input element this is.

type="text" (Text Field) - creating a text field input.
value for type="text":
id="[text]" (Identifier) - creates an identifier for the field. Use in programming language.
value="[text]" (value) - a placeholder/default value for an input element.
size="[number]" (size) - determines the number of characters that are displayed. The size of text field box.
maxlength="[number]" (maximum length) - the largest number of characters that are allowed.
pattern="[regular expressions]" - allows you to specify a regular expression used to validate the form.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.
placeholder="[text]" - allows you to add placeholder value in your text fields.

type="password" (Password Text Field) - creating a text field that inputs an asterisk.
value for type="password":
id="[text]" (Identifier) - creates an identifier for the field. Use in programming language.
value="[text]" (value) - a placeholder/default value for an input element.
size="[number]" (size) - determines the number of characters that are displayed. The size of text field box.
maxlength="[number]" (maximum length) - the largest number of characters that are allowed.
pattern="[regular expressions]" - allows you to specify a regular expression used to validate the form.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.
placeholder="[text]" - allows you to add placeholder value in your text fields.

type="hidden" (Hidden Text Field) - store information on the page without displaying that information to the user.
value for type="hidden":
id="[text]" (Identifier) - creates an identifier for the field. Use in programming language.
value="[text]" (value) - a placeholder/default value for an input element.
size="[number]" (size) - determines the number of characters that are displayed. The size of text field box.
maxlength="[number]" (maximum length) - the largest number of characters that are allowed.

<textarea> (text area) - contain a lot more information. A big text field. Anything placed inside <textarea> will be output.
value for <textarea>:
id="[text]" (Identifier) - This should be put in every <textarea>.
rows="[number]" (row) - specify the size.
cols="[number]" (column) - specify the size.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.
placeholder="[text]" - allows you to add placeholder value in your text fields.

<select> (selection) - indicate the entire list. Container for a list.
<option> (option list) - Each individual selection is housed in an <option></option> set.
value for <select>:
id="[text]" (Identifier) - This should be put in every <select> tag.
size="[number]" (size) - to specify how many rows to display and to make it a scrolling list.
value="[text]" (value) - reflects the value of the currently selected "option" in JavaScript.

type="checkbox" (Checkbox) - creating a checkbox rather than a text field.
value for type="checkbox":
id="[text]" (Identifier) - also require for writing a programming code.
value="[text]" (value) - it doesn't appear but only for the programmer.

type="radio" (Radio button) - let the user pick only one option from a group.
value for type="radio":
name="[text]" - indicates the group of a radio button is in. Same name on each member.
id="[text]" (Identifier) - require for writing a programming code.
value="[text]" (value) - it doesn't appear but only for the programmer.
checked="checked" - use if you want a radio button to be a default when the page appears.

Buttons: 
type="button" (Ordinary button) - make an ordinary button. Doesn't imply link. THIS TYPE OF BUTTON IS FOR CLIENT-SIDE PROGRAMMING!!
value for type="button":
value="[text]" (value) - to make a new caption for button.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.

type="submit" (Submit button) - make a submit button. Clicking it causes a link. THIS TYPE OF BUTTON IS FOR SERVER-SIDE PROGRAMMING!!
value for type="submit":
value="[text]" - to make a new caption for button. This is optional.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.

type="reset" (Reset button) - it resets all the elements of its form to their default values.
value for type="reset":
value="[text]" - to make a new caption for button. This is optional.
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.

<button> (Button) - Unlike the Input button, you can place <elements>, images or styled text inside a button.
value for <button>:
type="button" - also act like ordinary button. (But can place <element> inside.)
type="submit" - also act like submit button. (But can place <element> inside.)
type="reset" - also act like reset button. (But can place <element> inside.)
title="[text]" - specifies extra information. Shown as a tooltip text when the mouse moves over the element.

NEW FEATURES ON HTML5
New form of Input type: ALL THESE TYPES HAS SAME VALUE FROM THE OLDER TYPES ATTRIBUTE!!!

type="date" (Date) - indicates that you wish the user to enter a date value.
type="time" (Time) - allow the user to enter a time. 
type="datetime" (Date and time) - combines the date type and time type in single type.
type="datetime-local" (Date, Time, Local) - same as datetime type except does not include time zone.
type="week" (Week) - used to pick a week from a calendar control.
type="month" (Month) - generates a four-digit year followed by a two-digit month.
type="color" (Color) - allows the user to choose a color using standard web formats.
type="number" (Number) - This often consists of a text field followed by: say up and down arrows.
type="range" (Range) - user interface toolkits have some sort of slider or scrollbar mechanism for number.
type="search" (Search) - used to retrieve text that’s intended to be used as part of a search
type="email" (E-mail) -  it validates on an e-mail address.
type="tel" (Telephone) - used to input a telephone number.
type="url" (Web address) - indicate a web address.

mathematical equation:
<sup> (superscript) - characters that appear a little bit higher than normal text, like exponents and footnotes.
<sub> (subscript) - subscripts characters that appear lower, often used in mathematical notation.

Grouping:
<div> (Division) - A block-level element. Generally, you use div to group a series of paragraphs.
<span> (Span) - An inline element. Used to add some type of special formatting to an element that’s contained inside a block-level element.

Semantic Markup Tags: labeling things based on their meaning.
<header> (Header) - It denotes a chunk of the page that will contain a header for the page.
<nav> (Navigation) - This tag indicates some kind of navigation section. It has no particular style of its own.
<section> (Section) - A section is used to specify a generic part of the page.
<article> (Article) - Intended for use with external resources, when these pages integrate content from other sources
<footer> (Footer) - Intended to display footer contents at the bottom of a page. Typically a footer covers the bottom of a page.
<address> (Address) - Holds contact information.
<aside> (Aside) - Indicates a page fragment that is related to but separate from the main content.
<menu> (Menu) - Eventually, will allow a pop-up menu or toolbar. to be defined in the page.
<command> (Command) - It will be embedded inside that menu. Not supported yet.
<figure> (Figure) - Incorporates an image and a caption.
<figcaption> (Figure Caption) - Describes an image, normally enclosed in a figure tag.
<time> (Time) - Display dates or times.
<summary> (Summary) - A summary is visible at all times.
<detail> (Detail) -  When <summary is clicked on, the <detail> appears. Not supported yet.
<svg> (Scalable Vector Graphics) - Allows you to use the SVG language to describe a vector image through code.
<meter> (Meter) - Indicates a numeric value falling within a specific range.
<output> (Output) - Intended for output in interactive applications.
<progress> (Progress) - Should indicate progress of a task (but it doesn’t look like a progress bar yet).




some tags that not use anymore for problems that will occur:
<i> - replaced by <em>
<b> - replaced by <strong>
<s>
<blink>
<center>
<font>


The menu has internal links. A menu can contain links to external documents
or (like this one) links inside the current document. The <a href
= “#alpha”>Alpha</a> code means create a link to the element in
this page with the ID alpha.
