# Functions, Methods, and Objects

Enumerate the properties of an object
Starting with ECMAScript 5, there are three native ways to list/traverse object properties:

for...in loops
This method traverses all enumerable properties of an object and its prototype chain.
Object.keys(o)
This method returns an array with all the own (not in the prototype chain) enumerable properties' names ("keys") of an object o.
Object.getOwnPropertyNames(o)
This method returns an array containing all own properties' names (enumerable or not) of an object o.
Before ECMAScript 5, there was no native way to list all properties of an object. However, this can be achieved with the following function:

function listAllProperties(o) {
	var objectToInspect;
	var result = [];

	for(objectToInspect = o; objectToInspect !== null;
           objectToInspect = Object.getPrototypeOf(objectToInspect)) {
        result = result.concat(
            Object.getOwnPropertyNames(objectToInspect)
        );
    }

	return result;
}
______________________________________________________________________________________________________________________________________________
## Using the Object.create method
Objects can also be created using the Object.create() method. This method can be very useful, because it allows you to choose the prototype object for the object you want to create, without having to define a constructor function.

// Animal properties and method encapsulation
var Animal = {
  type: 'Invertebrates', // Default value of properties
  displayType: function() {  // Method which will display type of Animal
    console.log(this.type);
  }
};

// Create new animal type called animal1
var animal1 = Object.create(Animal);
animal1.displayType(); // Output:Invertebrates

// Create new animal type called Fishes
var fish = Object.create(Animal);
fish.type = 'Fishes';
fish.displayType(); // Output:Fishes
___________________________________________________________________________________________________________________________________

# Tabels 
# Active learning: Creating your first table
We've talked table theory enough, so, let's dive into a practical example and build up a simple table.

First of all, make a local copy of blank-template.html and minimal-table.css in a new directory on your local machine.
The content of every table is enclosed by these two tags : <table></table>. Add these inside the body of your HTML.
The smallest container inside a table is a table cell, which is created by a <td> element ('td' stands for 'table data'). Add the following inside your table tags:
<td>Hi, I'm your first cell.</td>
If we want a row of four cells, we need to copy these tags three times. Update the contents of your table to look like so:
<td>Hi, I'm your first cell.</td>
<td>I'm your second cell.</td>
<td>I'm your third cell.</td>
<td>I'm your fourth cell.</td>
As you will see, the cells are not placed underneath each other, rather they are automatically aligned with each other on the same row. Each <td> element creates a single cell and together they make up the first row. Every cell we add makes the row grow longer.

To stop this row from growing and start placing subsequent cells on a second row, we need to use the <tr> element ('tr' stands for 'table row'). Let's investigate this now.

Place the four cells you've already created inside <tr> tags, like so:
<tr>
  <td>Hi, I'm your first cell.</td>
  <td>I'm your second cell.</td>
  <td>I'm your third cell.</td>
  <td>I'm your fourth cell.</td>
</tr>

