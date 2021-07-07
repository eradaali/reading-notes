## Project Kickoff

## How can you make a website ?

## Firstly :
  - HTML Basics: Elements, Tags, and Document Structure
    - **Elements (Tags):** 
        -  A text header, denoted using the < h1> , < h2> , < h3> , < h4> , < h5> , < h6> tags.
         - A paragraph, denoted using the <p > tag.
         - A horizontal ruler, denoted using the <hr> tag.
         - A link, denoted using the < a> (anchor) tag.
         - A list, denoted using the < ul> (unordered list), <ol> (ordered list) and < li> (list element) tags.
         - An image, denoted using the < img> tag
         - A divider, denoted using the < div> tag
         - A text span, denoted using the < span> tag


    - **Document Structure**


      ![img](https://stuyhsdesign.files.wordpress.com/2015/09/basic-structure.png)  



## HTML
 The HyperText Markup Language, or HTML is the standard markup language for documents designed to be displayed in a web browser. It can be assisted by technologies such as Cascading Style Sheets (CSS) and scripting languages such as JavaScript.

Web browsers receive HTML documents from a web server or from local storage and render the documents into multimedia web pages. HTML describes the structure of a web page semantically and originally included cues for the appearance of the document.


## React: Component Lifecycle Events

**What are component lifecycle events?**
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

![img](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)


## Mounting
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

## Updating
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps .

## Unmounting
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.


## constructor()
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance. Let’s take a look at some example code.


## React 

![img]()
 React.Component :This page contains a detailed API reference for the React component class definition. It assumes you’re familiar with fundamental React concepts, such as Components and Props, as well as State and Lifecycle. 
- Forms
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.


## What are React controlled components and uncontrolled components?
This relates to stateful DOM components (form elements) and the React docs explain the difference:

 - A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. You could also call this a "dumb component".
 - A Uncontrolled Component is one that stores its own state internally, and you query the DOM using a ref to find its current value when you need it. This is a bit more like traditional HTML.


 ## Node.js 
 is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Consequently, Node.js represents a "JavaScript everywhere" paradigm,[6] unifying web-application development around a single programming language, rather than different languages for server-side and client-side scripts.

 ![img](https://uploads.toptal.io/blog/image/53/toptal-blog-3_B.png)

 ## What is OAuth? Definition and How it Works ?
 OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password. This minimizes risk in a major way: In the event ESPN suffers a breach, your Facebook password remains safe.

