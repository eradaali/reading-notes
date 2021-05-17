## CHART.JS
**Charts** are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. 
A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. 
how to use chart.js ?
- The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script.
- To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:
"<c anvas i d="buyers" w idth="600" h eight="400"></c anvas>"
- Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

-Inside the same script tags we need to create our data.
- Drawing a pie chart.
- Conclusion :You can view a demo of this in action here.

## Types charts :
 - line chart :A line chart is a way of plotting data points on a line. Often, it is used to show trend data, or the comparison of two data sets.
 ![imglinechart](https://www.excel-easy.com/examples/images/line-chart/line-chart.png)
 - Bar Chart :
A bar chart provides a way of showing data values represented as vertical bars. It is sometimes used to show trend data, and the comparison of multiple data sets side by side.
![barchart](https://images.squarespace-cdn.com/content/v1/55b6a6dce4b089e11621d3ed/1598373583669-2T51UP9OLLWDK4GXMXT1/ke17ZwdGBToddI8pDm48kJr_IgrJng_8BO3hFtkXDOd7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QHyNOqBUUEtDDsRWrJLTm5KLKmglmQrJ3HgLr6FItTejSvVsrnJzd3KFdstMGnV68V9HhiwqvhWZGXF9DPdyu/Investment+by+area+of+impact.png)

- Radar Chart
A radar chart is a way of showing multiple data points and the variation between them.
They are often useful for comparing the points of two or more different data sets.

- Doughnut and Pie ChartsPie and doughnut charts are probably the most commonly used charts. They are divided into segments, the arc of each segment shows the proportional value of each piece of data.

-Polar Area Chart
Polar area charts are similar to pie charts, but each segment has the same angle the radius of the segment differs depending on the value.

- Bubble Chart
A bubble chart is used to display three dimensions of data at the same time. The location of the bubble is determined by the first two dimensions and the corresponding horizontal and vertical axes.

- Scatter Chart
Scatter charts are based on basic line charts with the x axis changed to a linear axis. To use a scatter chart, data must be passed as objects containing X and Y properties.

- Area Chart
Both line and radar charts support a fill option on the dataset object which can be used to create space between two datasets or a dataset and a boundary.

- Mixed Chart Types
With Chart.js, it is possible to create mixed charts that are a combination of two or more different chart types. A common example is a bar chart that also includes a line dataset.

## Basic usage of canvas
 - *The < canvas> element*
 At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. 
- Fallback content
The < canvas> element differs from an < img> tag in that, like for < video>, < audio>, or < picture> elements.
- Required </ canvas> tag
As a consequence of the way fallback is provided, unlike the < img> element, the < canvas> element requires the closing tag (</ canvas>). 

## Drawing shapes with canvas
Now that we have set up our canvas environment, we can get into the details of how to draw on the canvas. By the end of this article, you will have learned how to draw rectangles, triangles, lines, arcs and curves, providing familiarity with some of the basic shapes. Working with paths is essential when drawing objects onto the canvas and we will see how that can be done.
**The grid**
Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. 

**Drawing rectangles**
Unlike SVG, <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

**Drawing paths**
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps.

**Lines**
For drawing straight lines, use the lineTo() method.

**Arcs**
To draw arcs or circles, we use the arc() or arcTo() methods.

## Applying styles and colors
You will learn how to add different colors, line styles, gradients, patterns and shadows to your drawings.
- Colors
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
**the strokeStyle property to change the colors of the shapes' outlines. We use the arc() method to draw circles instead of squares**
- Transparency
In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.
**Using rgba() gives you a little more control and flexibility because we can set the fill and stroke style individually.**
- The lineCap
 property determines how the end points of every line are drawn. There are three possible values for this property and those are: butt, round and square. By default this property is set to butt.
 - The lineJoin 
 property determines how two connecting segments (of lines, arcs or curves) with non-zero lengths in a shape are joined together (degenerate segments with zero lengths, whose specified endpoints and control points are exactly at the same position, are skipped).
 - Using line dashes
The setLineDash method and the lineDashOffset property specify the dash pattern for lines. The setLineDash method accepts a list of numbers that specifies distances to alternately draw a line and a gap and the lineDashOffset property sets an offset where to start the pattern.

## Drawing text
The canvas rendering context provides two methods to render text
**Styling text**
In the examples above we are already making use of the font property to make the text a bit larger than the default size.
**Gecko-specific notes**
In Gecko (the rendering engine of Firefox, Firefox OS and other Mozilla based applications), some prefixed APIs were implemented in earlier versions to draw text on a canvas. These are now deprecated and removed, and are no longer guaranteed to work.