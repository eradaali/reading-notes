## Error Handling and Debugging
The JavaScript interpreter uses the concept of execution contexts.
- EXECUTION CONTEXT JavaScript:
Every statement in a script lives in one of three 
execution contexts: 
 1. GLOBAL CONTEXT :Code that is in the script, but not in a function,There is only one global context in any page
 2. EVAL CONTEXT (NOT SHOWN) :Text is executed like code in an internal function called eval()

-VARIABLE SCOPE 

 1. GLOBAL SCOPE 
If a variable is declared outside a function, it can be used anywhere because it has global scope.

## EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases of activity: 
- PREPARE 
• The new scope is created 
• Variables, functions, and arguments are created 
• The value of the this keyword is determined 
- EXECUTE 
• Now it can assign values to variables 
• Reference functions and run their code 
• Execute statements 

## UNDERSTANDING SCOPE
In the interpreter, each execution context has its own va ri ables object. 
It holds the variables, functions, and parameters available within it. 
Each execution context can also access its parent's v a ri ables object. 

## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception. 
At that point, the interpreter stops and looks for exception-handl ing code.

## ERROR OBJECTS 
Error objects can help you find where your mistakes are and browsers have tools to help you read them. 
When an Error object is created, it will contain the 
following properties: 
**PROPERTY DESCRIPTION** 
1. name Type of execution 
2. message Description 
3. Number Name of the JavaScript file 
4. Number Line number of error

There are seven types of built-in error objects in 
JavaScript.
Error  :Generic error - the other errors are all based upon this error 
Syntax Error: Syntax has not been followed 
Ref erenceError :Tried to reference a variable that is not declared/within scope 
TypeError :An unexpected data type that cannot be coerced 
Range Error :Numbers not in acceptable range .
URI Error :encodeURI ().decodeURI(),and similar methods used incorrectly
EvalError :eva l () function used incorrectly

## A DEBUGGING WORKFLOW
*Debugging is about deduction: eliminating potential causes of an error. 
Here is a workflow for techniques you will meet over the next 20 pages*

## BREAKPOINTS:
You can pause the execution of a script on any line using breakpoints. Then you can check the 
values stored in variables at that point in time. 
*line using breakpoints. Then you can check the*
If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur.

## HANDLING EXCEPTIONS
If you know your code might fail, use try, catch, and finally. 
![trycatch](https://ar.javascript.info/article/try-catch/try-catch-flow.svg)

## THROWING ERRORS
If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.
## COMMON ERRORS:
- GO BACK TO BASICS 
- MISSED/ EXTRA CHARACTERS
- DATA TYPE ISSUES
