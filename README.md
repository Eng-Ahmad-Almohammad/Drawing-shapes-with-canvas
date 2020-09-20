# Drawing shapes with canvas
## The grid

### The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y).

## Drawing rectangles
### There are three functions that draw rectangles on the canvas:

1- fillRect(x, y, width, height) Draws a filled rectangle.

2- strokeRect(x, y, width, height) Draws a rectangular outline.

3- clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.

### Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.


## Drawing paths
### A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1- First, you create the path.

2- Then you use drawing commands to draw into the path.

3-Once the path has been created, you can stroke or fill the path to render it.

### Here are the functions used to perform these steps:

* beginPath(): Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

* Path methods: Methods to set different paths for objects.

* closePath(): Adds a straight line to the path, going to the start of the current sub-path.

* stroke(): Draws the shape by stroking its outline.

* fill(): Draws a solid shape by filling the path's content area.
