Structure of CSS in Page-Level:
<style type="text/css">
    (selector) {
	(attribute):(value);
}
</style>

Structure of CSS in Local Style:
<element style="attribute:value;"> </element>


Structure of CSS in External Style:
<head>
	<link rel="stylesheet" type="text/css" href="name of the stylesheet" />
</head>
-----------------------------------------------------------------------------------------

/* */ - one line/multi-line comment in CSS.

attribute/rule:

color: (color name/hex/HSL/RGB) - refers to the foreground color of any text in the element.
background-color:(color name/hex/HSL/RGB) -  The background color of the element.

font:(font-style, font-variant, font-weight, font-size, font-family) - shortcut for fonts. Order must follow.
font-family:(fonts) - name of the font you want to add on your web.
font-size: (numbers/name) - to change the size of the font.
font-style: ("italic", "normal", "oblique") - to change the style of the font NOT THE FONT FAMILY.
font-weight: (100-900) - to make your text bold.

text-decoration: (decorations) - used to add a couple other interesting formats to your text, underline, strikethrough, overline, etc.
text-align: (direction) - to center, left-align, or right-align text.
text-shadow:  (horizontal, vertical, blur, color) - creates a shadow only on the text.

border: (border-color, border-width, border-style) - shortcute for borders. Order doesn't matter.
border-color: (color name/hex/HSL/RGB) - color used to display the border. 
border-width: (measurements) - the width of the border.
border-style: ("double", "dotted", etc.) - use to style the border.
border-left: (border-color, border-width, border-style) - show a border on the left only.
border-right: (border-color, border-width, border-style) - show a border on the right only.
border-top: (border-color, border-width, border-style) - show a border on the top only.
border-bottom: (border-color, border-width, border-style) - show a border on the bottom only.
border-image: (url"name of file", width, repeat) - use an image for an element border.
border-radius: (measurements) - creates rounded corners for the border.
box-shadow: (horizontal, vertical, blur, spread, color) - creates shadow behind the element.
display: (block/inline) - makes an element act like a block-level/inline element inside its container.

padding: (top, right, bottom, left) - shortcut for 4 values.
padding: (top, right and left, bottom) - shortcut for 3 values.
padding: (top and bottom, right and left) - shortcut for 2 values.
padding: (top and bottom and right and left) - shortcut for 1 values.
padding-left: (measurements) - create space on the left only.
padding-right: (measurements) - create space on the right only.
padding-top: (measurements) - create space on the top only.
padding-bottom: (measurements) - create space on the bottom only.

margin: (top, right, bottom, left) - shortcut for 4 values.
margin: (top, right and left, bottom) - shortcut for 3 values.
margin: (top and bottom, right and left) - shortcut for 2 values.
margin: (top and bottom and right and left) - shortcut for 1 values.
margin-left: (measurements) - create a margin on the left only.
margin-right: (measurements) - create a margin on the right only.
margin-top: (measurements) - create a margin on the top only.
margin-bottom: (measurements) - create a margin on the bottom only.
margin: auto - for centering an element.

background: () - 
background-image: (url("name of the file") - add a background image to the page or specific element.
background-repeat: (no-repeat) - to turn off the automatic repetition of an image.
background-size: (measurements) - to resize the background image.

list-style-image: url("name of the file") - make the bullet an image.
list-style-type: (styles) - to style a list to the default css.

Special Effects: vendor prefixes needed.
opacity: (0-1) - to adjust transparency of an any element.
-webkit-box-reflect: (direction, gap from the element) - to create reflection to the element. Works only on Chrome and Safari.
-webkit-text-stroke: (size, color) - create a stroke for text.
text-shadow: (x-axis, y-axis, blur, color) - to create a shadow for text.

Transformation: vendor prefixes needed.
perspective: (measurements) - Change the perspective of the parent element that will contain your transformed elements.
transform: () - allows you to apply mathematical transformation to any div.
transform: translate/translateX/translateY (x-axis, y-axis) - moves the object from its default position.	 
transform: rotate/rotateX/rotateY (angle/deg) - rotate the image around its center value.
transform: scale/scaleX/scaleY (number without unit) - changes the size of the object.
transform: skew/skewX/skewY (deg unit) - allows you to tilt the element by some angle.
transform: translate3d (x-axis, y-axis, z-axis, angle/deg) - allows you to translate along multiple axes at the same time.
transform: rotate3d (x-axis, y-axis, z-axis, angle/deg) - allows you to translate along multiple axes at the same time.
transform: scale3d (x-axis, y-axis, z-axis, angle/deg) - allows you to translate along multiple axes at the same time.

Transitions: vendor prefixes needed.
transition: (property, duration, timing, delay) - can cause transitions to happen over time.
transition-property (any attribute that has the element) - to choose what attribute will transition.
transition-duration (seconds) - the length of the animation in seconds.
transition-timing (linear, ease, ease-in, ease-out, ease-in-out) - how animation occur at the time phase.
transition-delay (seconds) - the animation will not begin until after the delay.

Animations: vendor prefixes needed.
@keyframes [name you want] - it’s used to generate a keyframe set and mini style sheet. You can use any element inside the braces.
{
	0% {any attribute:(value);}
	25% {any attributes:(value);}
	50% {any attributes:(value);}
	75% {any attributes:(value);}
	100% {any attributes:(value);}
	to {any attributes:(value);}
	from{any attributes:(value);}
}
-prefix-@keyframes ("name you want") {} - still requires browser-specific prefixes
animation: (keyframe name, duration, timing, repetition, delay) - creates an animation.
animation-fill-mode: ()

Floating Layout:
float: (left/right) - The float CSS property specifies that an element should be placed along the left or right side of its container, allowing text and inline elements to wrap around it.
clear: (left) - you want nothing to the left of this element. The element should be on the left margin of its container.
clear: (right) - you want nothing to the right of this element. The element should be on the right margin of its container.
clear: (both) - It should have no elements to the left or the right. It should occupy a line all its own. 
width: (measurements) - to adjust the width of a block/element.
height: (measurements) - to adjust the height of a block/element.
min-height: (measurements) - minimum height for an element. Use this property to force all columns to be the same height.
overflow: (auto/scroll/visible/hidden) - shrnking the space if it cannot place the text in the indicated space.

position: (fixed) - Use fixed position when you want an element to stay in the same place, even when the page is scrolled.
postion: (absolute) - used to determine exactly (more or less) where the element will be placed on the screen.
position: (relative) - when you want to move an element from its default position.
z-index: (numeric) - when you have elements that you want to appear over the top of other elements.

top: (measurements) - indicates where the top of the element will go.
bottom: (measurements)
left: (measurements) -  determines where the left edge of the element will go.
right: (measurements)

Flexible Box Layout: (BEST FOR LAYOUT! NOT YET SUPPORTED! Use vendor-specific prefixes.
display: (box) - makes it capable of holding other elements with the flexible box mechanism.
box-orient: (horizontal/vertical) - to determine if the child elements of the current element will be placed vertically or horizontally inside the main element.
box-flex: (numeric) - The weight determines how much space that element takes up.
box-ordinal-group: (numeric) - to adjust the placement order.

vendor specific prefixes:
-webkit-(attribute): (same value) - rendering image using Chrome and Safari.
-moz-(attribute): (same value) - rendering image using Firefox.
-o-(attribute): (same value) - rendering image using Opera.
-ms-(attribute): (same value) - rendering image using Internet Explorer.

Rarely used attributes:
font-variant: - set to small-caps to make your text use only capital letters. Lowercase letters are shown in a smaller font size.
Letter-spacing: (measurements) - Adjusts the spacing between letters. It’s usually measured in Ems (em). 
Word-spacing: (measurements) -  Allows you to adjust the spacing between words.
Text-indent: (measurements) - Lets you adjust the indentation of the first line of an element.
Vertical-align: (directions) - Used when you have an element with a lot of vertical space (often a table cell). 
Text-transform: (text cases) - Helps you convert text into uppercase, lowercase, or capitalized (first letter uppercase) forms.
Line-height: (measurements) - Indicates the vertical spacing between lines in the element.

Pseudo-classes:
a:visited - when the user visits a link and and returns to the current page.
(selector):hover - when the user's mouse is hovering on the element.
(selector):focus - activated when an element is ready to receive keyboard input.
(selector):active - active when it is currently being used. Button has been pressed but not yet released.
(selector):not(element) - for not including the effect on the element.
(selector):nth-child(numbers/formula/word) - allows you to select on or more elements in a group.
(selector):nth-of-type(numbers/formula/word) - it filters to a specific type and ignores any elements that are not of exactly the same type of element.
(selector):nth-last-child(numbers/formula/word) - Works just like nth-child, excepts counts from the end of the group of elements rather than the beginning.
(selector):last-nth-of-type(numbers/formula/word): Works like nth-of-type, but from the end of the group.
(selector):first-child - Grabs the first element.
(selector):last-child - selects the last child element.
:invalid - allows you to select <input> elements that do not contain valid content.
:required - selects form elements which are required.

Red, Blue, Green - Color Names
#98ffc9 - Hex Value
#FFCC33 - Web-Safe Pallete
RGB (0-256, 0-256, 0-256) - RGB (Red, Green, Blue)
RGBA (0-256, 0-256, 0-256, 0-1) - RGBA (Red, Green, Blue, Transparency)
HSL (180, 75%, 25%) - HSL (Hue, Saturation, Lightness)

HEXADECIMAL VALUE COLOR SCHEME:
16 color names with Hex Value -
Color          Hex Value
Black           #000000
White           #FFFFFF
Silver          #C0C0C0
Gray            #808080
Maroon          #800000
Red             #FF0000
Purple          #800080
Fuchsia         #FF00FF
Green           #008800
Lime            #00FF00
Olive 		#808000
Yellow 		#FFFF00
Navy 		#000080
Blue 		#0000FF
Teal 		#008080
Aqua 		#00FFFF



HEX VALUE Format:
RED  GREEN  BLUE
#00    00    00 - 00 up to ff each color.
it is 00 to ff or 09 or 0f or f2 

WEB-SAFE PALLETE Format:
#33 66 99 cc ff - (very dark, semi dark, dark, bright very bright)
it can be short as it the same:
#fff means ffffff
#fc9 means ffcc99

HSL color model scheme:
HUE SATURATION LIGHTNESS

HSL VALUE Format:
color: HSL (180, 75%, 25%); - (Hue, Saturation, Lightness)
Hue - 0 to 360 degrees (without degree sign) red at top, blue at bottom.
Saturation - 0% - 100% percentage (with % sign) grayscale to fully colored.
Lightness - 0% - 100% percentage (with % sign) black to white.

Font Equivalents:
Windows 	     Mac 		Linux
Arial 	            Arial               Nimbus Sans L
Arial Black   	    Arial Black
Comic Sans MS       Comic Sans MS       TSCu_Comic
Courier New         Courier New         Nimbus Mono L
Georgia             Georgia 		Nimbus Roman No9 L
Lucida Console      Monaco
Palatino            Palatino 		FreeSerif
Tahoma 		    Geneva 		Kalimati
Times New Roman     Times 		FreeSerif
Trebuchet MS        Helvetica 		FreeSans
Verdana             Verdana 		Kalimati

Font format for font-family attribute:
font-family:"quotes with two+ words", withOutQuotesOnOneWord, fontOption3, fontOption4;
or
font-family: Default Font, Windows Font, Mac Font, Linux Font;

REMEMBER!!!: <font> <i> <b> <center> are not use anymore for styling a HTML web.

FONT-FACE FORMAT: @font-face - css tag to add an embedded font file. To create/customize your own font and import to your web page.
@font-face {

	font-family:"[your own name of font]"; 
	src: url("name and format of font")
}  


Font-Size:

2 Different Types of Measurements Unit:
Absolute measurements - attempt to describe a particular size, as in the real world. Not useful in web but in print.
Relative measurements - are about changes to some default value. 

Absolute Measurements Unit:
Point (pt) - Absolute measurement, not useful for web pages but useful in print media.
Pixel (px) - refer to the small dots on the screen.
Inches (in) and Centimeter (cm) - Real-life measurement units aren’t meaningful for the web. Use it on print.

Relative Measurements Unit:
Percentage (%) - a relative measurement used to specify the font in relationship to its normal size.
Em (em) - a unit of measurement equivalent to the width of the “m” character in that font.
Named Size - wiser choice in web development. The following are:
xx-small
x-small
small
medium - Default size of the paragraph page.
large
x-large
xx-large - are usually the size of <h1> tag.

id attribute/selector - when you have a style you want to apply to only one element on the page. Add (#) sign before the name of selector.
REMINDER FOR ID: TWO DIFFERENT ELEMENTS CAN'T HAVE THE SAME ID. ONLY ON ONE ELEMENT.

Format for Id:

in HTML:
<element id="[name you want]"> </element>

in CSS style sheet:
#name of id {
      attribute:value;
}

class attribute/selector - can be applied to all things. Useful than Id attribute when you have two or more elements. Add (.) before name.
REMINDER FOR CLASS: IT CAN COMBINE CLASSES ON ELEMENTS AND ADD MORE CLASSES ON ONE ELEMENT.

Format for one class on one element:

in HTML:
<element class="[name you want]"> </element>

in CSS style sheet:
.name of the id {
	attribute:value;
}

Format for two or more class on one element:

in HTML:
<element class="[first class] [second class]"> </element>

in CSS style sheet:
.first class {
	attribute:value;
}

.second class {
	attribute:value;
}

Nested Element Format: 

in HTML: 
<element id="nameOfTheId">

	<newElement> </newElement>

<element>

in CSS:
#nameOfTheId newElement {
	attribute:value;
}

Multiple Element Format:

in HTML:
<firstElement>    </firstElement>
<secondElement>   </secondElement>
<thirdElement>    </thirdElement>

in CSS: 
firstElement, secondElement, thirdElement {
	attribute:value;
}

REMEMBER!!!: If you have multiple elements in a selector rule, it makes a huge difference
whether you use commas. If you separate elements with spaces (but no
commas), CSS looks for an element nested within another element. If you
include commas, CSS applies the rule to all the listed elements.


New CSS3 Selectors:

Attribute Selection
in CSS: You can now apply a style to any element with a specific attribute value.
input[type="text"] {
	attribute:value;
}

Element to Element Selector
in CSS: used to select elements with a specific parent.
parentElement > childElement {
	attribute:value;
}

Box Model Format:
Block-level Element - always describe their own space on the screen.
Inline Element - allowed only within the context of a block-level element.

Block-Level Element has a several layers of space arount it such as.
Padding - The space between the content and the border.
Border - Goes around the padding.
Margin - Space outside the border between the border and the parent element.

Gradients:
Linear - changes colors along a straight line.
Radial - outward from a center point.

background-image: linear-gradient(direction/s, beginning color, end color)
background-image: linear-gradient(angle degrees, color/s as many as you want)
background-image: radial-gradient(direction/s, beginning color, end color)
background-image: radial-gradient(angle degrees, color/s as many as you want)
ex. 
background-image: linear-gradient(left, red, white);
background-image: linear-gradient(blue, red, white);
background-image: linear-gradient(75deg, red, white 33%, white 66%, blue);

Managing Levels of Style:
Local Styles - Defined by specifying a style within an HTML element’s attributes.
Page-level styles - Defined in the page's header area. 
External styles - Defined on a separate document and linked to the page.

Local Styles:
<element style="attribute:value;"> </element>

Page-level Style:
<head>
    <style type="text/css">
    
    </style>
</head>

External Style:
<head>
	<link rel="stylesheet" type="text/css" href="name of the stylesheet" />
</head>

Hierarchy of Styles:
An element will display any style rules you define for it, but certain rules are also passed on from other places. Generally, this is how style rules cascade through the page:

The body defines overall styles for the page - Any style rules that you
want the entire page to share should be defined in the body. Any element in the body begins with the style of the page. This makes it easy to define an overall page style.

A block-level element passes its style to its children - If you define a div with a particular style, any elements inside that div will inherit the div ’s
style attributes. Likewise, defining a list will also define the list items.

You can always override inherited styles - Of course, if you don’t want paragraphs to have a particular style inherited from the body, you can just change them.


Overriding Styles:
Here’s the precedence (from highest to lowest precedence):

1. User preference: The user always has the final choice about what styles are used. Users aren’t required to use any styles at all and can always change the style sheet for 
their own local copy of the page. If a user needs to apply a special style (for example, high contrast for people with visual disabilities), he should always have that option.

2. Local style: A local style (defined with the style attribute in the HTML) has the highest precedence of developer-defined styles. It overrules any other styles.

3. id : A style attached to an element id has a great deal of weight because it overrides any other styles defined in the style sheet.

4. Class: Styles attached to a class override the style of the object’s element. So, if you have a paragraph with a color green that belongs to a
class colored blue, the element will be blue because class styles outrank element styles.

5. Element: The element style takes precedence over any of its containers. For example, if a paragraph is inside a div, the paragraph style has the
potential to override both the div and the body.
 
6. Container element: divs, tables, lists, and other elements used as containers pass their styles on. If an element is inside one or more of these containers, 
it can inherit style attributes from them.

7. Body: Anything defined in the body style is an overall page default, but it will be overridden by any other styles.


Precedence of Style Definition:
(From Highest to Lowest Rank)
Local Styles - should avoided. Use class or id if you need to override the page-level style.
Page-level Style - This can override external styles.
External Style - Weakest rank, you can write a page-level style to override an external style.

Conditional Comment only for Internet Explorer:
If the style doesn't appear on your IE browser, you can put conditional comment
to have an option for your IE browser to appear.

Format: 
<!--[if IE]>
	codes
<![endif]-->

Designing the page:

Draw the sketch first so you have some idea what you’re aiming for. Your
sketch should include the following information:

1. Overall page flow: How many columns do you want? Will it have a
header and footer?

2. Section names: Each section needs an ID, which will be used in both the
HTML and the CSS.

3. Width indicators: How wide will each column be? (Of course, these
widths should add up to 100 percent or less.)

4. Fixed or percentage widths: Are the widths measured in percentages
(of the browser size) or in a fixed measurement (pixels)? This has
important implications. For this example, I’m using a dynamic width
with percentage measurements.

5. Font considerations: Do any of the sections require any specific font
styles, faces, or colors?