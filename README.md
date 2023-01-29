# canvas-context

## Table of Contents
1. [What is Canvas](#what-is-canvas)
2. [How does Canvas work](#how-does-canvas-work)
3. [Drawing in Canvas](#drawing-in-canvas)

### What is Canvas
`Canvas` is an HTML element used to draw graphics, on the fly, via scripting. It is used to draw shapes, such as paths, circles, rectangles, and even complex imagery, such as photo and animation. Canvas can be used in tandem with other HTML elements, such as video and audio, to create a user experience that is more interactive and engaging than traditional webpages.

### How does Canvas work
Canvas is rendered as an HTML element and works within an HTML file. When the page is opened, the browser looks for the `<canvas>` element and parses it. It then creates a context, which is like a drawing surface on which developers draw vector graphics, raster graphics and text. The context is the child of the `<canvas>` element.\
JavaScript is then used to manipulate the canvas context. Developers write code to draw shapes, images, and text on the canvas. When a command is issued, the browser immediately draws the object on the canvas and continues to render the page.\
Canvas APIs are available for controlling the canvas element. This includes methods for setting the width and height, setting the style attributes, manipulating line width or type, drawing lines and shapes, and adding event handlers for user interactions.

### Drawing in Canvas
To draw shapes in Canvas, we use:
1. `rect()` - to draw a rectangle;
2. `arc()` - to draw a circle;
3. `moveTo()` and `lineTo()` - to draw a triangle;

**To draw a rectangle**\
*Canvas Context Rect* is a built-in method in the canvas 2D rendering context that allows you to draw a rectangle onto the canvas. It is invoked by calling the `rect()` method in the canvas context. This method takes four required parameters indicating:
- the `x` and `y` coordinates of the top-left corner of the rectangle;
- followed by the `width` and `height` of the rectangle, respectively.

It also takes an optional sixth parameter that indicates whether the rectangle should be filled with a color or not. The rect() method returns a Path2D instance that can be further manipulated by other canvas commands.

**To draw a circle**\
*Canvas context arc()* is a method used in the HTML5 canvas element to draw an arc or circle. It takes 6 parameters: 
- x, y - determine the coordinates of the center point of the arc. 
- radius - defines the radius of the arc.
- startAngle, endAngle - determine the starting and ending angles of the arc in radians.
- anticlockwise (true or false) - a boolean that defines whether the arc should be drawn in a clockwise or counterclockwise direction.

**To draw a trianle**
1. To draw a triangle, use the canvas context's `beginPath()` method to tell the canvas context to begin drawing.
2. Use the canvas context's `moveTo()` method to move the pencil to the first point of your triangle.
3. Use the canvas context's `lineTo()` method to draw a line from the first point to the second.
4. Draw another `lineTo()` from the second point to the third point of the triangle.
5. Connect the last point to the first point of the triangle to complete the shape using `lineTo()`.
6. Use the canvas context's `stroke()` method to draw the triangle shape.
7. Use the canvas context's `fill()` method to give the triangle its color.
