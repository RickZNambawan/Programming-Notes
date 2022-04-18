The three geometry managers are as follows:
• pack: This is the one that we have used so far. It is simple to use for simpler
layouts, but it may get very complex for slightly complex layouts.
• grid: This is the most commonly used geometry manager that provides a
table-like layout of management features for easy layout management.
• place: This is the least popular, but it provides the best control for the
absolute positioning of widgets.

*********************************************************************************
When packing the child widgets, the pack manager distinguishes between the
following three kinds of space:
• The unclaimed space
• The claimed but unused space
• The claimed and used space
*********************************************************************************
The most commonly used options in pack include the following:
• side: LEFT, TOP, RIGHT, and BOTTOM (these decide the alignment of the widget)
• fill: X, Y, BOTH, and NONE (these decide whether the widget can grow in size)
• expand: Boolean values such as tkinter.YES/tkinter.NO, 1/0, True/False
• anchor: NW, N, NE, E, SE, S, SW, W, and CENTER (corresponding to thecardinal directions)
• ipadx and ipady: (Internal padding) for the padding inside widgets and
•  padx and pady:  (External padding) which all default to a value of zero
*********************************************************************************
The pack manager is ideally suited for the following two kinds of situation:
• Placing widgets in a top-down manner
• Placing widgets side by side
*********************************************************************************
For a complete pack reference, type the following command in the Python shell:
>>> import tkinter
>>> help(tkinter.Pack)
*********************************************************************************
For Grid()
•row
•column
•rowspan
•columnspan
•padx
•pady
•ipadx
•ipady
•sticky = N,S,E,W
*********************************************************************************
Another grid option that you can sometimes use is the widget.grid_forget()
method. This method can be used to hide a widget from the screen. When you use
this option, the widget still exists at its former location, but it becomes invisible.
The hidden widget may be made visible again, but the grid options that you had
originally assigned to the widget will be lost.

Similarly, there is a widget.grid_remove() method that removes the widget, except
that in this case, when you make the widget visible again, all of its grid options will
be restored.
*********************************************************************************
>>> import tkinter
>>> help(tkinter.Grid)
*********************************************************************************
For place()
The important options for place geometry include the following:
• Absolute positioning (specified in terms of x=N or y=N)
• Relative positioning (the key options include relx, rely, relwidth, and relheight)
*********************************************************************************
>>> import tkinter
>>> help(tkinter.Place)
*********************************************************************************
Passing arguments to callbacks
If a callback does not take any argument, it can be handled with a simple function,
such as the one shown in the preceding code. However, if a callback needs to take
arguments, we can use the lambda function, as shown in the following code snippet:
	def my_callback (argument)
		#do something with argument
Then, somewhere else in the code, we define a button with a command callback
that takes some arguments, as follows:
Button(root,text="Click", command=lambda: my_callback('some argument'))
*********************************************************************************
square = lambda x: x**2
Now, we can call the square method, as follows:
>>> print(square(5)) ## prints 25 to the console
*********************************************************************************
An event type: Some common event types include Button, ButtonRelease,
KeyRelease, Keypress, FocusIn, FocusOut, Leave (when the mouse leaves
the widget), and MouseWheel. For a complete list of event types, refer to the
The event types section at http://www.tcl.tk/man/tcl8.6/TkCmd/bind.
htm#M7.
*********************************************************************************
An event modifier (optional): Some common event modifiers include Alt,
Any (used like <Any-KeyPress>), Control, Double (used like <Double-
Button-1> to denote a double-click of the left mouse button), Lock, and
Shift. For a complete list of event modifiers, refer to the The event modifiers
section at http://www.tcl.tk/man/tcl8.6/TkCmd/bind.htm#M6.
*********************************************************************************
The event detail (optional): The mouse event detail is captured by the
number 1 for a left-click and the number 2 for a right-click. Similarly,
each key press on the keyboard is either represented by the key letter itself
(say, B in <KeyPress-B>) or by using a key symbol abbreviated as keysym.
For example, the up arrow key on the keyboard is represented by the keysym
value of KP_Up. For a complete keysym mapping, refer to https://www.tcl.
tk/man/tcl8.6/TkCmd/bind.htm.
*********************************************************************************
widget.bind("<Button-1>", callback) #bind widget to left mouse click
widget.bind("<Button-2>", callback) # bind to right mouse click
widget.bind("<Return>", callback)# bind to Return(Enter) Key
widget.bind("<FocusIn>", callback) #bind to Focus in Event
widget.bind("<KeyPress-A>", callback)# bind to keypress A
widget.bind("<KeyPress-Caps_Lock>", callback)# bind to CapsLock keysym
widget.bind("<KeyPress-F1>", callback)# bind widget to F1 keysym
widget.bind("<KeyPress-KP_5>", callback)# bind to keypad number 5
widget.bind("<Motion>", callback) # bind to motion over widget
widget.bind("<Any-KeyPress>", callback) # bind to any keypress
*********************************************************************************
instance-level binding:
• Application-level binding: Application-level bindings let you use the same
binding across all windows and widgets of an application as long as any one
window of the application is in focus.
The syntax for application-level bindings is as follows:
widget.bind(event, callback, add=None)
The typical usage pattern is as follows:
root.bind_all('<F1>', show_help)
An application-level binding here means that irrespective of the widget
that is currently under focus, pressing the F1 key will always trigger the
show_help callback as long as the application is in focus.

• Class-level binding: You can also bind events at a particular class level.
This is normally used to set the same behavior for all instances of a particular
widget class.
The syntax for class-level binding is as follows:
w.bind_class(class_name, event, callback, add=None)
The typical usage pattern is as follows:
my_entry.bind_class('Entry', '<Control-V>', paste)
*********************************************************************************
Creating a Tkinter variable is simple. You simply have to call the constructor:
my_string = StringVar()
ticked_yes = BooleanVar()
group_choice = IntVar()
volume = DoubleVar()
*********************************************************************************
This concludes our brief discussion on events and callbacks. Here's a brief summary
of the things that we discussed:
• The command binding, which is used to bind simple widgets to
certain functions
• The use of the lambda function in case you need to process arguments
• Event binding using the widget.bind(event, callback, add=None)
method to bind keyboard and mouse events to your widgets and invoke
callbacks when certain events occur
• The passing of extra arguments to a callback
• The binding of events to an entire application or to a particular class of
widget by using bind_all() and bind_class()
• Using the Tkinter variable class to set and get the values of widget-specific
variables
*********************************************************************************
Event unbinding and virtual events:
unbind: Tkinter provides the unbind option to undo the effect of an earlier
binding. The syntax is as follows:
widget.unbind(event)

Virtual events: Tkinter also lets you create your own events. You can give
these virtual events any name that you want.
For example, let's suppose that you want to create a new event called
<<commit>>, which is triggered by the F9 key. To create this virtual
event on a given widget, use the following syntax:
widget.event_add('<<commit>>', '<KeyRelease-F9>')

You can then bind <<commit>> to a callback by using a normal bind()
method, as follows:
widget.bind('<<commit>>', callback)
*********************************************************************************
>>> import tkinter
>>> help(tkinter.Event)
*********************************************************************************
Specifying styles
Under the purview of styling, we will cover how to apply different colors, fonts,
border widths, reliefs, cursors, and bitmap icons to widgets.
*********************************************************************************
First, let's see how to specify the color options for a widget. You can specify the
following two types of color for most widgets:
• The background color
• The foreground color
*********************************************************************************
You can specify the color by using hexadecimal color codes for the proportion of red,
green, and blue. The commonly used representations are #rgb (4 bits), #rrggbb (8
bits), and #rrrgggbbb (12 bits).
For example, #fff is white, #000000 is black, #f00 is red (R=0xf, G=0x0, B=0x0),
#00ff00 is green (R=0x00, G=0xff, B=0x00), and #000000fff is blue (R=0x000,
G=0x000, B=0xfff).

*********************************************************************************
The elements of the preceding syntax can be explained as follows:
• font family: This is the complete font family long name. It should
preferably be in lowercase, such as font="{nimbus roman} 36 bold
italic".
• fontsize: This is in a printer's point unit (pt) or pixel unit (px).
• fontstyle: This is a mix of normal/bold/italic and underline/
overstrike.
The following are the examples that illustrate the method of specifying fonts:
widget.configure (font='Times 8')
widget.configure(font='Helvetica 24 bold italic')
*********************************************************************************
The default border width for most Tkinter widgets is 2 px. You can change the border
width of the widgets by specifying it explicitly, as shown in the following line:
button.configure(borderwidth=5)
*********************************************************************************
The relief style of a widget refers to the difference between the highest and lowest
elevations in a widget. Tkinter offers six possible relief styles—flat, raised, sunken,
groove, solid, and ridge:
button.configure(relief='raised')
*********************************************************************************
Tkinter lets you change the style of the mouse cursor when you hover over a
particular widget. This is done by using the option cursor, as follows:
button.configure(cursor='cross')
*********************************************************************************
external option database
A typical option database text file looks like this:
*background: AntiqueWhite1
*Text*background: #454545
*Button*foreground: gray55
*Button*relief: raised
*Button*width: 3
In its simplest use, the asterisk (*) symbol here means that the particular style is
applied to all the instances of the given widget. For a more complex usage of the
asterisk in styling, refer to http://infohost.nmt.edu/tcc/help/pubs/tkinter/
web/resource-lines.html.
*********************************************************************************
root.option_readfile('optionDB.txt')
*********************************************************************************
*root.geometry('142x280+150+200') - You can specify the size and location of
a root window by using a string of the
widthxheight + xoffset + yoffset form.
*********************************************************************************
self.root.iconbitmap('mynewicon.ico ') - This changes the title bar icon to something
that is different from the default Tk icon.
*********************************************************************************
root.overrideredirect(1) - This removes the root border frame. It
hides the frame that contains the minimize,
maximize, and close buttons.
*********************************************************************************
import tkFont
myFont = tkFont.Font(family="Helvetica", size=36, weight="bold")

font=myFont
*********************************************************************************
*********************************************************************************
*********************************************************************************
*********************************************************************************
*********************************************************************************
*********************************************************************************
