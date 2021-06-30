## The JavaScript Call Stack 
*The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.*

is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the **call stack is synchronous**.

## What is the call stack?
a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

**LIFO**
Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.
![img](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)


## Manage function invocation (call): 
The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). 

## What causes a stack overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. 



## JavaScript error messages && debugging

**Types of error messages**
- Reference errors :This is as simple as when you try to use a variable that is not yet declared you get this type os errors, also a common thing when using const and let and the fact that this happens to let and const is called Temporal Dead Zone (TDZ).
- Syntax errors :when you have something that cannot be parsed in terms of syntax.
- Range errors : Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
- Type errors :ike the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible

## debugging
console.log( ) the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug


##  Handling errors
when we do not handle errors properly, meaning that anything after that error will not be executed. To avoid this we usually try to catch the errors so we can gracefully fallback to a default state of our application in case of an error (this fallback can be a 404 page which is normally not that graceful but is better than a page to just stop working).


