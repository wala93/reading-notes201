# Transforms


With CSS3 came new ways to position and alter elements. Now general layouttechniques
can be revisited with alternative ways to size, position, and change elements.
All of these new techniques are made possible by the transform property.

## Transform Syntax

The actual syntax for the transform property is quite simple, including the transform
property followed by the value. The value specifies the transform type followed by 
a specific amount inside parentheses.
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}


2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane.

2D Rotate
The transform property accepts a handful of different values. The rotate value provides the ability 
to rotate an element from 0 to 360 degrees.

.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

2D Scale
Using the scale value within the transform property allows you to change the appeared size of an element. 
.box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: scale(1.25);
}

              
2D Translate
The translate value works a bit like that of relative positioning, pushing and pulling an 
element in different directions without interrupting the normal flow of the document.
.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}

Perspective Depth Value
The perspective value can be set as none or a length measurement. The none value turns off any perspective, 
while the length value will set the depth of the perspective. The higher the value, the further away the 
perspective appears, thus creating a fairly low intensity perspective and a small three-dimensional change.
The lower the value the closer the perspective appears, thus creating a high intensity perspective 
and a large three-dimensional change.


## 3D Transforms
Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes, however
there is another axis along which we can transform elements. Using three-dimensional transforms we can 
change elements on the z axis, giving us control of depth as well as length and width.

3D Rotate
So far we’ve discussed how to rotate an object either clockwise or counterclockwise on a flat plane.
With three-dimensional transforms we can rotate an element around any axes. To do so, 
we use three new transform values, including rotateX, rotateY, and rotateZ.


.box-1 {
  transform: perspective(200px) rotateX(45deg);
}
.box-2 {
  transform: perspective(200px) rotateY(45deg);
}
.box-3 {
  transform: perspective(200px) rotateZ(45deg);
}
___________________________________________________________________________________________________________________________________________________

CSS3 has introduced countless possibilities for UX designers, and the best thing about them is that the coolest parts are really simple to implement.

Just a couple of lines of code will give you an awesome transition effect that will excite your users, increase engagement and ultimately, when used well, 
increase your conversions. What’s more, these effects are hardware accelerated, and a progressive enhancement that you can use right now.

like : 
fade 
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
growth and shrink
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}

swing 
3d shadow
.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}

____________________________________________________________________________________________________________________________________________________________



















































