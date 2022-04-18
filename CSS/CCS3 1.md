CSS - CASCADE STYLE SHEETS
REAL FORMAT FOR CREATING WERBSITE:
<head>
	<link rel="stylesheet" type="text/css" href="(NAME OF THE CSS FILE)"/>

		<style type="text/css"> 
    (SELECTOR/TAGS/ELEMENTS) {(PROPERTY):(VALUE);(YOU CAN ADD MORE);}
		</style>
</head>

FORMAT FOR CSS ONLY:
	<style type="text/css"> 
    (SELECTOR/TAGS/ELEMENTS) {(PROPERTY):(VALUE);(YOU CAN ADD MORE);}
	</style>
</head>

(BIG NOTE! YOU CAN CREATE A FILE THAT ONLY USE CSS FOR THE WHOLE WEBSITE)
EXTERNAL STYLE SHEET (YOU CAN SEPERATE HTML FROM CSS)

JUST CREATE NEW FILE AND SAVE AS .CSS FILE

FORMAT IN HTML ONLY IN THE <head>:
<head>
	<link rel="stylesheet" type="text/css" href="(NAME OF THE CSS FILE)"/>
</head>



TAGS:
 (NOTE: YOU CAN ADD MORE TAGS FOR YOU TO MAKE THE EFFECT OF THAT ELEMENT)
 (ELEMENTS) {color:(any color/can be RGB color);}
 (ELEMENTS) {font-family:(font style);}
 (ELEMENTS) {line-height:(amount/numbers/percentage);}
 (ELEMENTS) {font-weight:(font style);}
 (ELEMENTS) {font-style:(font style);}
 (ELEMENTS) {text-align:(position);}
 (ELEMENTS) {text-indent:(Number of pixels);}
 (ELEMENTS) {background-color:(color/can be RGB color;}
 (ELEMENTS) {background-image:(picture file);}
 (ELEMENTS) {background-repeat:(position);}
 (ELEMENTS) {background-position:(pixel/can be percentage);} (FIRST NUMBER LEFT AND RIGHT 2ND IS UP AND DOWN)
 (ELEMENTS) {padding:(Number of Pixel);}
 (ELEMENTS) {padding-top:(Number of Pixel);}
 (ELEMENTS) {padding-bottom:(Number of Pixel);}
 (ELEMENTS) {border-color:(color);}
 (ELEMENTS) {border-width:(pixel);}
 (ELEMENTS) {border-style:(style);}
 (ELEMENTS) {border-top-color:(color);}
 (ELEMENTS) {border-top-style:(style);}
 (ELEMENTS) {border-width:(pixel);}
 (ELEMENTS) {margin:(pixel);}
 (ELEMENTS) {margin-top:(pixel);}
 (ELEMENTS) {margin-bottom:(pixel);}
 (ELEMENTS) {width:(pixel);}
 (ELEMENTS) {height:(pixel);}
 (ELEMENTS) {border:(pixel w/color);}
 (ELEMENTS) {text-decoration:(decoration);}
 (ELEMENTS) {border:(pixel with style of border and color;}
 (ELEMENTS) {background-color:(color);}
 (ELEMENTS) {list-style-type:(stle of bullet);}
 (ELEMENTS) {list-style-image:url((FILE OF THE IMAGE));}
 (ELEMENTS) {list-style-type:none;}
 (ELEMENTS) {top:(pixel);}
 (ELEMENTS) {max-height:(pixel);}
 (ELEMENTS) {max-width:(pixel);}
(Before and After) (ELEMENTS):(WHAT TEXT YOU WANT TO CHANGE) {PROPERTY:VALUE;}

Format:
# (NAME OF THE ID) {border:(pixel) solid (color);
		    position:(POSITION);
    		    top:(pixel);
  		    left:(pixel);}
 #(NAME OF THE ID) {position:absolute;} - CAN BE OVERLAP WITH THE OTHER ELEMENT.
 #(NAME OF THE ID) {position:relative;} - WHAT ACTUALLY THE POSITION THAT BE.
 #(NAME OF THE ID) {position:fixed;} - Stay in place and doesn't move whether you scroll down/up.

DIFFERENT STATES OF A LINK:
 a:link   {(PROPERTY):(VALUE);}
 a:visted {(PROPERTY):(VALUE);}
 a:hover  {(PROPERTY):(VALUE);}
 a:active {(PROPERTY):(VALUE);}