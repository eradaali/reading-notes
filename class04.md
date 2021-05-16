## Writing Links
**Links** are created using the < a> element. Users can click on anything between the opening < a> tag and the closing </ a> tag. 

## Directory Structure
*On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder*
- Structure: he diagram on the right shows the directory structure  
for fictional entertainment listings website.
- Relationships :he relationship between files and folders on a website.
- Homepages:The main homepage of a site written in HTML.


*Every page and every image on a website has a URL*
![img](https://moz-static.s3.amazonaws.com/learn/seo/Domains-page/_large/domain-description-image.png?mtime=20170320080539)

**Relative URLs** can be used when linking to pages within your own 
website.
Relative Link Type:
 - Parent
The examplearts folder is a parent of the music folder.
- Grandparent
The examplearts folder is a grandparent of the dvd folder
- Grandchild
The dvd folder is a grandchild of the examplearts folder.
- Child
The music folder is a child of the examplearts folder.


mailto:
To create a link that starts up the user's email program and 
addresses an email to a specified email address.
pening Links in a New Window :target

## Layout
- Building Blocks
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
   1. Block-level elements start on a new line
   2. Inline elements flow in between surrounding text.


CSS has the following positioning schemes that allow you to control 
the layout of a page: normal flow, relative positioning, and absolute 
positioning. 
- Normal flow
- Relative Positioning
- bsolute positioning


To indicate where a box should be positioned, you may also need to use 
box offset properties to tell the browser how far from the top or bottom and left or right it should be placed. (You will meet these 
when we introduce the positioning schemes.

*Screen size*:Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.
*Screen Resolution* Resolution refers to the number of dots a screen shows per inch.
*Page Sizes*:Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide .
*Liquid layout* designs stretch and contract as the user increases 
or decreases the size of their browser window.

FUNCTIONS &  METHODS

 Functions let you group a series of statements together to perform a 
specific task. If different parts of a script repeat the same task, you can 
reuse the function (rather than repeating the same set of statements).

![method](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1587882057-1.png)


**Functions can return more than one value using an array. For example, this function calculates the area and volume of a box.**

## ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS

Expressions produce a value. They can be used where values are expected. 
If a function is placed where a browser expects to see an expression, 
(e.g., as an argument to a function), then it gets treated as an expression.

- FUNCTION DECLARATION

A function declaration creates a function that you 
can call later in your code
 
- FUNCTION EXPRESSION

If you put a function where the interpreter would 
expect to see an expression, then it is treated as an 
expression, and it is known as a function expression. 

### IMMEDIATELY INVOKED FUNCTION EXPRESSIONS

*This way of writing a function is used in several different situations. 
Often functions are used to ensure that the variable names do not conflict 
with each other (especially if the page uses more than one script).*

- IMMEDIATELY INVOKED FUNCTION EXPRESSIONS (llFE)

Pronounced "iffy," these functions are not given 
a name. Instead, they are executed once as the 
interpreter comes across them. 

- WHEN TO USE ANONYMOUS FUNCTIONS AND llFES 
1.As an argument when a function is called (to calculate a value for that function). 
2.n event handlers and listeners (see Chapter 6) to perform a task when an event occurs. 
3.to prevent conflicts between two scripts that might use the same variable name

**VARIABLE SCOPE**
The location where you declare a variable will affect where it can be used 
within your code. If you declare it within a function, it can only be used 
within that function. This is known as the variable's scope. 

- LOCAL VARIABLES

When a variable is created inside a function using the 
var keyword, it can only be used in that function. 
It is called a local variable or function-level variable. 
It is said to have local scope or function-level scope

- GLOBAL VARIABLES

If you create a variable outside of a function, then it 
can be used anywhere within the script. It is called a 
global variable and has global scope. In the example 
shown, wa 11 Size is a global variable

## HOW MEMORY & VARIABLES WORK 

Global variables use more memory. The browser has to remember them 
for as long as the web page using them is loaded. Local variables are only 
remembered during the period of time that a function is being executed.

- CREATING THE VARIABLES IN CODE
Each variable that you declare takes up memory. 
The more variables a browser has to remember, 
the more memory your script requires to run

- NAMING COLLISIONS
You might think you would avoid naming collisions; 
after all you know which variables you are using. 
But many sites use scripts written by several people.