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






