# GIMP-change-icon-color
How to change a PNG file icon color using GIMP 

You will need to install the software GIMP 
https://www.gimp.org/downloads/

Open PNG file 
Create new layer called "color" and choose option "background color" 
* use cmd+shft+n to create new layer

![alt tag](/img/new-layer.png)

Fill new color layer with desired icon color
* go to Color > colorify > custom color

Create a new background color layer called "mask"
* move mask layer below the PNG icon layer

![alt tag](/img/mask-layer.png)

Select layer with imported icon and choose Color > Desaturate > lightness
* on same layer choose Color > invert

![alt tag](/img/desaturate.png)

Right click on icon layer and choose merge down

Select new mask layer and choose Colors > curves - drag middle of line straight to top

![alt tag](/img/adjust-color-curve.png)

Right click on color layer and choose: add layer mask > check black full transparency > check invert mask

Select mask layer cmd+a or Select > All

Copy mask layer onto color layer 

A new layer will be created called "floating selection"
* right click new layer and choose "anchor layer" 

Hide mask layer and show color layer

Export to format needed (I choose PNG)

Props to Ben Ramey and his tutorial on changing PNG icon colors 
http://www.benramey.com/2012/03/15/change-the-color-of-an-icon-with-gimp/

# Convert PNG file to SVG
A free option is to use the software Inkscape
Open PNG and make sure option "embed" is chosen 
click on the image
choose Path > tace bitmap
check options: color, stack scans, remove background 
  * scans should be colors in picture +1
 click ok and moce new icon to delete the old one below it



