https://wala93.github.io/reading-notes201/read2 

# Basics of HTML, CSS & JS
X HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).
X They also provide semantic information (e.g. where
emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).

## some examples for semantic :
<strong>
The use of the <strong>
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.
By default, browsers will show
the contents of a <strong>
element in bold.

<dfn>
The first time you explain some
new terminology (perhaps an
academic concept or some
jargon) in a document, it is
known as the defining instance
of it.

<ins>
<del>
The <ins> element can be used
to show content that has been
inserted into a document

## Introducing CSS

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.


## <link>
The <link> element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the <head> element.
It should use three attributes:
href
This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).
type
This attribute specifies the type
of document being linked to. The
value should be text/css.
rel
This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.

CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.

ules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
CSS rules usually appear in a separate document,
although they may appear within an HTML page.

******************************************************************************************************************************************************

## Basic JavaScript Instructions

WHAT IS A VARIABLE?
A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables. 

Scripts contain very precise instructions. For example,
you might specify that a value must be remembered
before creating a calculation using that value. 

Expressions evaluate into a single value.
Expressions rely on operators to calculate a value. 

**********************************************************************************************************************************************************************

JavaScript Loops
Loops are handy, if you want to run the same code over and over again, each time with a different value.
Often this is the case when working with arrays

The For Loop
The for loop has the following syntax:
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
Statement 1 is executed (one time) before the execution of the code block.
Statement 2 defines the condition for executing the code block.
Statement 3 is executed (every time) after the code block has been executed.
The While Loop
The while loop loops through a block of code as long as a specified condition is true.
Syntax
while (condition) {
  // code block to be executed
}

Comparison Operators
Comparison operators are used in logical statements to determine equality or difference between variables or values.
Given that x = 5,
Logical Operators
Logical operators are used to determine the logic between variables or values.
Given that x = 6 and y = 3








