# links :
You will commonly come across the following types of links:
● Links from one website to another
● Links from one page to another on the same website
● Links from one part of a web page to another part of the
same page
● Links that open in a new browser window
● Links that start up your email program and address a new
email to someone

When you link to a different website, the value of the href 
attribute will be the full web address for the site, which is
known as an absolute URL.

When you are linking to other pages within the same site,
you do not need to specify the domain name in the URL. You
can use a shorthand known as a relative URL.

mailto: 
To create a link that starts up the user's email program and
addresses an email to a specified email address, you use the <a>
element. However, this time the value of the href attribute starts
with mailto: and is followed by the email address you want the
email to be sent to.

Opening Links in a New Window use target - blank  in href .


You can use the id attribute to target elements within
a page that can be linked to.
________________________________________________________________________________________________________________________________________
# “Layout”

Controlling the Position of Elements :

CSS has the following positioning schemes that allow you to control the layout of a page: 
normal flow, relative positioning, and absolutepositioning. You specify the positioning
scheme using the position property in CSS. You can also float elements using the float property.

When you use relative, fixed, or absolute positioning, boxes can
overlap. If boxes do overlap, the elements that appear later in the
HTML code sit on top of those that are earlier in the page.
If you want to control which element sits on top, you can use
the z-index property. Its value is a number, and the higher the
number the closer that element is to the front. For example, an
element with a z-index of 10 will appear over the top of one
with a z-index of 5.

## Screen Sizes
Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

## Page Sizes
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).


## Fixed Width Layouts
Fixed width layout designs do not change size as the  user increases
or decreases the size of their browser window.
Measurements tend to be given in pixels.

## Liquid Layouts
Liquid layout designs stretch and contract as the user increases or decreases the
size of their browser window. They tend to use percentages.

_______________________________________________________________________________________________________________________

# Functions, Methods, and Objects

Functions let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements).

## Function Invocation
The code inside the function will execute when "something" invokes (calls) the function:

When an event occurs (when a user clicks a button) 
When it is invoked (called) from JavaScript code
Automatically (self invoked)


## Function Return

When JavaScript reaches a return statement, the function will stop executing.
If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.
Functions often compute a return value. The return value is "returned" back to the "caller":
You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.
___________________________________________________________________________________________________________________________________________________
# why pair programming ?

Expected Benefits
increased code quality: “programming out loud” leads to clearer articulation of the complexities
and hidden details in coding tasks, reducing the risk of error or going down blind alleys
better diffusion of knowledge among the team, in particular when a developer unfamiliar with
a component is pairing with one who knows it much better better transfer of skills, as junior developers
pick up micro-techniques or broader skills from more experienced team members
large reduction in coordination efforts, since there are N/2 pairs to coordinate instead of
N individual developers improved resiliency of a pair to interruptions, compared to
an individual developer: when one member of the pair must attend to an external prompt,
the other can remains focused on the task and can assist in regaining focus afterwards.





