## Component Lifecycle Events


### What are component lifecycle events?
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. 

**React Lifecycle Events**
![img](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)

*The three phases of the component lifecycle*
- Mounting
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.
- Updating
Anytime a component is updated or state changes then it is rerendered.
- Unmounting
The final phase of the lifecycle if called when a component is being removed from the DOM.
**componentWillUnmount is the only lifecycle event during this phase**

**constructor( )**
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. 
**static getDerivedStateFromProps( )**
This method exists for rare cases where the state relies on changes in props over time.
**render( )**
Render is the only required method in a class component.
**componentDidMount( )**
This method is invoked immediately after a component is mounted. 
**shouldComponentUpdate( )**
The default behavior in react is to rerender after every state change. 
**getSnapshotBeforeUpdate( )**
This is another rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM.
**componentDidUpdate( )**
This method is useful for performing network requests after a change has occurred.
**componentWillUnmount( )**
This method allows you to clean up the DOM and netwrok requests/ subscriptions.


## State and Lifecycle
 **Steps to Converting a Function to a Class**
You can convert a function component like Clock to a class in five steps:
 - Create an ES6 class, with the same name, that extends React.Component.
 - Add a single empty method to it called render().
 - Move the body of the function into the render() method.
 - Replace props with this.props in the render() body.
 - Delete the remaining empty function declaration.

Using State :
- Do Not Modify State Directly
- State Updates May Be Asynchronous
- State Updates are Merged


## Handling Events
Handling events with React elements is very similar to handling events on DOM elements.
 **There are some syntax differences:**
- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.