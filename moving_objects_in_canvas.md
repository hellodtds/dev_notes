# Moving Objects in a Canvas

Drawing everything using exact coordinates is fine for a couple shapes, but breaks down if you need to draw a bunch of objects.

_Canvas2D_ allows you to translate (move), rotate, or scale objects.

## Scaling
`scale(x,y)` multiplies the x and y values by a given factor so

`ctx.scale(2,3);`

will make all values twice as large on the x axis and three times as large on the y axis.

## Translation
`translate(x,y)` moves all subsequent draw commands by x number of pixels on horizontally and y pixels vertically.

`ctx.translate(20,40)` moves all elements drawn after it 20 pixels to the rights and 40 pixels down.

## Rotation
`ctx.rotate(angleRadians)` rotates an object a certain number of radians (generally) about its center. You may have learned about radians in school but here's a handy formula to convert a value from degrees to radians.

`radians = degrees * (Math.PI/180)`

Don't ask us why everything in Computer Graphics uses radians. We have no idea. :)

Here is more on [Math.PI from MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/PI)

## Order of operations
You should generally scale objects first, rotate them next, and then finally translate last. There are times when you'd want to rotate around an arbitrary point instead of an object's center, that's out of scope for this lesson.

It’s important to note that whatever transformations apply for all subsequent objects until you reverse them.