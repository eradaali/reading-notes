## Component-Based Architecture
*Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties.*


**component reusability:** A component encapsulates functionality and behaviors of a software element into a reusable and self-deployable binary unit.
 There are many standard component frameworks such as COM/DCOM, JavaBean, EJB, CORBA, .NET, web services, and grid services.

## What is a Component?
A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

**Views of a Component**
- Object-oriented view
A component is viewed as a set of one or more cooperating classes.
- Conventional view
It is viewed as a functional element or a module of a program that integrates the processing logic, the internal data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data to be passed to it.
- Process-related view
In this view, instead of creating each component from scratch, the system is building from existing components maintained in a library.


## Characteristics of Components
- **Reusability** Components are usually designed to be reused in different situations in different applications.
- **Replaceable** Components may be freely substituted with other similar components.

- **Not context specific** Components are designed to operate in different environments and contexts.

- **Extensible** A component can be extended from existing components to provide new behavior.

- **Encapsulated** A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

## Principles of Component−Based Design
![img](https://www.tutorialspoint.com/software_architecture_design/images/principles_of_component_based_design.jpg)

**Advantages**
- Ease of deployment: As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

- Reduced cost : The use of third-party components allows you to spread the cost of development and maintenance.

- Ease of development :Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

- Reusable:The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

- Modification of technical complexity ;A component modifies the complexity through the use of a component container and its services.

- Reliability: The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

- System maintenance and evolution: Easy to change and update the implementation without affecting the rest of the system.

- Independent :Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.




## What is Props?
React is a component-based library which divides the UI into little reusable pieces.

**Using Props in React**

- Firstly, define an attribute and its value(data)
-  pass it to child component(s) by using Props
-  render the Props Data

**Notes**
Props stand for properties and is a special keyword in React
Props are being passed to components like function arguments
Props can only be passed to components in one-way (parent to child)
Props data is immutable (read-only)


## Intro to React

Setup for the Tutorial of React
There are two ways to complete this tutorial: 
- you can either write the code in your browser
- you can set up a local development environment on your computer.
-  Write Code in the Browser
First, open this Starter Code in a new tab. The new tab should display an empty tic-tac-toe game board and React code. We will be editing the React code in this tutorial.
- Local Development Environment

## What Is React?
React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.


## The smallest React example looks like this:
![img](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSOgw5PHoCPJxIvMF6XMuL4VWMF7X-PEIY0bRPKWst0JHiepUa0kHLRnYiLPyGTNNuBZ64&usqp=CAU)

**Why JSX?**
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

## React Only Updates What’s Necessary
React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.


## Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components.

## Composing Components
Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as componen

## Extracting Components
Don’t be afraid to split components into smaller components.

## Props are Read-Only
Whether you declare a component as a function or a class, it must never modify its own props.

**All React components must act like pure functions with respect to their props.**