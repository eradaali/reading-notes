## React I want to know more about

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript.

How process of building a searchable product data table using React?
- Start With A Mock
Imagine that we already have a JSON API and a mock from our designer.
- Break The UI Into A Component Hierarchy
draw boxes around every component (and subcomponent) in the mock and give them all names.
how do you know what should be its own component? Use the same techniques for deciding if you should create a new function or object. One such technique is the **single responsibility principle**, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.
![img](https://reactjs.org/static/eb8bda25806a89ebdc838813bdfa3601/6b2ea/thinking-in-react-components.png)
- Build A Static Version in React
-  Identify The Minimal (but complete) Representation Of UI State
To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.
 **when you want to render the TODO count, take the length of the TODO items array.**
    **Think of all the pieces of data in our example application. We have:**

     - The original list of products
     - The search text the user has entered
     - The value of the checkbox
     - The filtered list of products

**What are the three questions you can ask to determine if something is state?**
    - Is it passed in from a parent via props? If so, it probably isn’t state.
    - Does it remain unchanged over time? If so, it probably isn’t state.
    - Can you compute it based on any other state or props in your component? If so, it isn’t state.

- Identify Where Your State Should Live  
React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. 
This is often the most challenging part for newcomers to understand, so follow these steps to figure it out:
For each piece of state in your application:
  - Identify every component that renders something based on that state.
  - Find a common owner component (a single component above all the components that need the state in the hierarchy).
  - Either the common owner or another component higher up in the hierarchy should own the state.
  - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
- Add Inverse Data Flow   