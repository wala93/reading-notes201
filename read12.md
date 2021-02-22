# Chart.js

Creating a Chart
It's easy to get started with Chart.js. All that's required is the script included in your
page along with a single <canvas> node to render the chart.

In this example, we create a bar chart for a single dataset and render that in our page.
You can see all the ways to use Chart.js in the usage documentation.


_________________________________________________________________________________________________________________________________________
## The <canvas> element
<canvas id="tutorial" width="150" height="150"></canvas>

At first sight a <canvas> looks like the <img> element, with the only clear difference being that it doesn't have the src and alt attributes.
Indeed, the <canvas> element has only two attributes, width and height. 

## Fallback content
The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy to define some fallback content, 
to be displayed in older browsers not supporting it, like versions of Internet Explorer 
earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

Providing fallback content is very straightforward: just insert the alternate content inside the <canvas> element.
Browsers that don't support <canvas> will ignore the container and render the fallback content inside it. Browsers that do support <canvas> will ignore the content inside the container, and just render the canvas normally.

## The rendering context
The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES.

The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The <canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D.

var canvas = document.getElementById('tutorial');
var ctx = canvas.getContext('2d');

___________________________________________________________________________________________________________________


The grid
Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous
page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. 
Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at 
coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square 
becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can 
translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.

The fillRect() function draws a large black square 100 pixels on each side. The clearRect() function then erases a 60x60 pixel
square from the center, and then strokeRect() is called to create a rectangular outline 50x50 pixels within the cleared square.

In upcoming pages we'll see two alternative methods for clearRect(), and we'll also see how to change the color and stroke style of the rendered shapes.

Unlike the path functions we'll see in the next section, all three rectangle functions draw immediately to the canvas.

## Drawing paths
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes,
curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes 
using paths, we take some extra steps:

First, you create the path.
Then you use drawing commands to draw into the path.
Once the path has been created, you can stroke or fill the path to render it.

_________________________________________________________________________________________________________________________________________________

## Colors
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two 
important properties we can use: fillStyle and strokeStyle.

fillStyle = color
Sets the style used when filling shapes.
strokeStyle = color
Sets the style for shapes' outlines.
color is a string representing a CSS <color>, a gradient object, or a pattern object. We'll look at gradient
and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

Note: When you set the strokeStyle and/or fillStyle property, the new value becomes the default for all shapes
being drawn from then on. For every shape you want in a different color,
you will need to reassign the fillStyle or strokeStyle property.
_____________________________________________________________________________________________________________________________________

## Drawing text
The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
A fillText example
The text is filled using the current fillStyle.






















