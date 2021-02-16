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


  
  
