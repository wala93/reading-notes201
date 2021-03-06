# forms
The HTML <form> element represents a document section containing interactive controls for submitting information.
  
  <form action="" method="get" class="form-example">

 It is possible to use the :valid and :invalid CSS pseudo-classes to style a <form> element based on 
  whether or not the elements inside the form are valid.
  
 ## accept-charset
Space-separated character encodings the server accepts. The browser uses them in the order in which they are listed. The default value means the same encoding as the page.
(In previous versions of HTML, character encodings could also be delimited by commas.)

## autocapitalize 
A nonstandard attribute used by iOS Safari that controls how textual form elements should be automatically capitalized. autocapitalize attributes on a form elements override it on <form>.
  
## Possible values:
none: No automatic capitalization.
sentences (default): Capitalize the first letter of each sentence.
words: Capitalize the first letter of each word.
characters: Capitalize all characters — that is, uppercase.
  
 ## autocomplete
Indicates whether input elements can by default have their values automatically completed by the browser. autocomplete attributes on form elements override it on <form>. 

## Possible values:
off: The browser may not automatically complete entries. (Browsers tend to ignore this for suspected login forms; see The autocomplete attribute and login fields.)
on: The browser may automatically complete entries.
  
## name
The name of the form. Deprecated as of HTML 4 (use id instead). It must be unique among the forms in a document and not an empty string as of HTML5.
  
## rel
Creates a hyperlink or annotation depending on the value, see the rel attribute for details.
  

## target
Indicates where to display the response after submitting the form. In HTML 4, this is the name/keyword for a frame. In HTML5, it is a name/keyword for a browsing context (for example, tab, window, or iframe). The following keywords have special meanings:
_self (default): Load into the same browsing context as the current one.
_blank: Load into a new unnamed browsing context.
_parent: Load into the parent browsing context of the current one. If no parent, behaves the same as _self.
_top: Load into the top-level browsing context (i.e., the browsing context that is an ancestor of the current one and has no parent). If no parent, behaves the same as _self.
This value can be overridden by a formtarget attribute on a <button>, <input type="submit">, or <input type="image"> element.
  ________________________________________________________________________________________________________________________________________
  
  
  
  # Lists, Tables and Forms

HTML Lists and CSS List Properties
In HTML, there are two main types of lists:

unordered lists (<ul>) - the list items are marked with bullets
ordered lists (<ol>) - the list items are marked with numbers or letters
The CSS list properties allow you to:

* Set different list item markers for ordered lists
* Set different list item markers for unordered lists
* Set an image as the list item marker 
* Add background colors to lists and list items

Different List Item Markers
The list-style-type property specifies the type of list item marker.

Position The List Item Markers
The list-style-position property specifies the position of the list-item markers (bullet points).

"list-style-position: outside;" means that the bullet points will be outside the list item.
The start of each line of a list item will be aligned vertically

# CSS Tables
The look of an HTML table can be greatly improved with CSS:

## Table Borders
To specify table borders in CSS, use the border property.
The example below specifies a black border for <table>, <th>, and <td> elements.
  
## Full-Width Table
The table above might seem small in some cases. If you need a table that should span the entire screen (full-width), add width: 100% to the <table> element.
  
 ## Collapse Table Borders
The border-collapse property sets whether the table borders should be collapsed into a single border.


***************************************************************************************************************************************************************************

  ___________________________________________________________________________________________________________________________________________________________
# Events

DIFFERENT EVENT TYPES
Here is a selection of the events that occur in the browser while you are
browsing the web. Any of these events can be used to trigger a function
in your JavaScript code.

HTML events are "things" that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can "react" on these events.


HTML Events
An HTML event can be something the browser does, or something a user does.

Here are some examples of HTML events:

An HTML web page has finished loading
An HTML input field was changed
An HTML button was clicked
Often, when events happen, you may want to do something.

JavaScript lets you execute code when events are detected.

HTML allows event handler attributes, with JavaScript code, to be added to HTML elements.

With single quotes:

<element event='some JavaScript'>
  
  In the following example, an onclick attribute (with code), is added to a <button> element:
  <button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
  
  In the example above, the JavaScript code changes the content of the element with id="demo".

In the next example, the code changes the content of its own element (using this.innerHTML):

Example
<button onclick="this.innerHTML = Date()">The time is?</button>

JavaScript code is often several lines long. It is more common to see event attributes calling functions:

Example
<button onclick="displayDate()">The time is?</button>

What can JavaScript Do?
Event handlers can be used to handle and verify user input, user actions, and browser actions:

Things that should be done every time a page loads
Things that should be done when the page is closed
Action that should be performed when a user clicks a button
Content that should be verified when a user inputs data
And more ...
Many different methods can be used to let JavaScript work with events:

HTML event attributes can execute JavaScript code directly
HTML event attributes can call JavaScript functions
You can assign your own event handler functions to HTML elements
You can prevent events from being sent or being handled
  
