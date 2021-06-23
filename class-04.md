## Forms I want to know more about
## Forms
*HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.*

![img](https://www.concretepage.com/angular-2/images/angular-2-formcontrol-example-2.jpg)



**In React** 
 If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.



 ## **Controlled Components**
   In React, mutable state is typically kept in the state property of components, and only updated with setState( ).


## **The < FormControl >**
 component renders a form control with Bootstrap styling. The < FormGroup > component wraps a form control with proper spacing, along with support for a label, help text, and validation state. To ensure accessibility, set controlId on < FormGroup >, and use < FormLabel > for the label.

**handleChange** runs on every keystroke to update the React state


**< textarea >**  uses a value attribute instead.

## Handling Multiple Inputs
handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of "event. target. name".


##  The Conditional (Ternary) Operator Explained
Shorten your if statements into one line of code with the conditional operator


Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

## what you need to know about the if conditinal :

- The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.

- A ? separates our conditional from our true value. Anything between the ? and - the : is what is executed if the condition evaluates to true.

- Finally a : colon. If your condition evaluates to false, any code after the colon is executed.