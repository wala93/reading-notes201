# images 
You can specify the dimensions of images using CSS.
This is very helpful when you use the same sized
images on several pages of your site.

 Images can be aligned both horizontally and vertically
using CSS.

You can use a background image behind the box
created by any element on a page.

Background images can appear just once or be
repeated across the background of the box.

You can create image rollover effects by moving the
background position of an image.

To reduce the number of images your browser has to
load, you can create image sprites.

> The <image> CSS data type represents a two-dimensional image.

> Syntax
> The <image> data type can be represented with any of the following:

> An image denoted by the <url>() data type
> <gradient> data type
>  part of the webpage, defined by the element() function
> An image, image fragment or solid patch of color, defined by the image()() function
> A blending of two or more images defined by the cross-fade() function.
> A selection of images chosen based on resolution defined by the image-set() function.
> ______________________________________________________________________________________________________________________________________________________________________
# Practical Information

In every page of your website there are seven key places where keywords
(the words people might search on to find your site) can appear in order
to improve its findability.

1: Page Title

The page title appears at the top of the browser window or on the
tab of a browser. It is specified in the <title> element which lives
inside the <head> element.
 
2: URL / Web Address

The name of the file is part of the URL. Where possible, use
keywords in the file name.

3: Headings

If the keywords are in a heading <hn> element then a search
engine will know that this page is all about that subject and give it
greater weight than other text.
 
4: Text
 Where possible, it helps to repeat the keywords in the main
body of the text at least 2-3 times. Do not, however, over-use
these terms, because the text must be easy for a human to read.


5: Link Text
Use keywords in the text that create links between pages
(rather than using generic

6: Image Alt Text
Search engines rely on you providing accurate descriptions
of images in the alt text. This will also help your images show
up in the results of image-based searches.

7: Page Descriptions
The description also lives inside the <head> element and is
specified using a <meta> tag. It should be a sentence that
describes the content of the page. (These are not shown in
the browser window but they may be displayed in the results
pages of search engines.)
 
 
> Determining which keywords to use on your site can be one of the
> hardest tasks when you start to think about SEO. Here are six steps that
> will help you identify the right keywords and phrases for your site.
> 


The content link on the left-hand side allows you to learn more about what the visitors are
looking at when they come to your site.



**Many companies provide platforms for blogging, email**
**newsletters, e-commerce and other popular website**
**tools (to save you writing them from scratch).**

____________________________________________________________________________________________________________________________________________________________

# video and audio

The <video> and <audio> elements allow us to embed video and audio into web pages. As we showed in Video and audio content, a typical implementation looks like this:

<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>


The HTMLMediaElement API
Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play(), HTMLMediaElement.pause(), etc. This interface is available to both <audio> and <video> elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.
 
 
 
 
 
 Here are some suggestions for ways you could enhance the existing example we've built up:

The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

Because <audio> elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an <audio> element too. Try doing so.

Can you work out a way to turn the timer inner <div> element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object. For example:

document.onclick = function(e) {
  console.log(e.x) + ',' + console.log(e.y)
}























