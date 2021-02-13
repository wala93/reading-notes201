# Understanding The Problem Domain Is The Hardest Part Of Programming


What is the hardest thing about writing code?

There are many common answers to this question:

Learning a new technology
Naming things
Testing your code
Debugging
Fixing bugs
Making software maintainable
The list goes on and on

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.

The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.
If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

* Make the problem domain easier
* Get better at understanding the problem domain
_________________________________________________________________________________________________________________________________________________________
# WHAT IS AN OBJECT?
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES 
IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS 

## You define (and create) a JavaScript object with an object literal:
   Example
var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
The name:values pairs in JavaScript objects are called properties:

## Accessing Object Properties
You can access object properties in two ways:

objectName.propertyName
or
objectName["propertyName"]

## Object Methods
Objects can also have methods.
Methods are actions that can be performed on objects.
Methods are stored in properties as function definitions.
>A method is a function stored as a property.

## Accessing Object Methods
You access an object method with the following syntax:

objectName.methodName()


______________________________________________________________________________________________________________________________________________________________________

# Document Object Model

The Document Object Model (DOM) specifies how browsers should create a model of an HTML
page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas: 

* MAKING A MODEL OF THE HTM L PAGE 
* ACCESSING AND CHANGING THE HTML PAGE 

## Accessing and updating the DOM tree involves two steps:
1: Locate the node that represents the element you want to work with.
2: Use its text content, child elements, and attributes. 

he Document method querySelectorAll() returns a static (not live) NodeList representing a list of the document's elements that match the specified group of selectors.
Note: This method is implemented based on the ParentNode mixin's querySelectorAll() method.

DOM queries may return one element, or they may return a Nodelist,which is a collection of nodes. 

get El ementByi d () allows you to select a single element node
by specifying the value of its id attribute.
This method has one parameter: the value of the id attribute on
the element you want to select.

This value is placed inside quote marks because it is a string. The
quotes can be single or double quotes, but they must match. 


There are two ways to select an element from a Nodelist:
The item() method and array syntax.
Both require the index number of the element you want.
THE ;tern{) METHOD 


## TRAVERSING THE DOM
When you have an element node, you can select
another element in relation to it using these five
properties. This is known as traversing the DOM. 

The NamedNodeMap Object
In the HTML DOM, the NamedNodeMap object represents an unordered collection of an elements attribute nodes.

Nodes in a NamedNodeMap can be accessed by name or by index (number).

>in older browsers, implementation of the DOM is
>inconsistent (and is a popular reason for using jQuery).
>Browsers offer tools for viewing the DOM tree . 



















__________________________________________________________________________________________________________________________________________________________________


