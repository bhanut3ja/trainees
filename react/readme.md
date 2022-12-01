# React
- ### Introduction to React JS
- ### What is React.js?
React is a JavaScript library created by Facebook
React is a User Interface (UI) library
React is a tool for building UI components
            
To use React in production, you need npm which is included with Node.js. ([Link](https://nodejs.org/en/))

- Setting up a React Environment
If you have npx and Node.js installed, you can create a React application by using create-react-app.
            
Run this command to create a React application named my-react-app:
            
        npx create-react-app your-app-name

The create-react-app will set up everything you need to run a React application.

-Run the React Application
Now you are ready to run your first real React application!
Run this command to move to the my-react-app directory:
            
        cd your-app-name

Run this command to run the React application my-react-app:
            
        npm start

Modify the React Application
So far so good, but how do I change the content?
Look in the `your-app-name` directory, and you will find a `src` folder. Inside the src folder there is a file called `App.js`, open it and and Replace all the content inside the `<div className="App">` with a `<h1>`element.
See the changes in the browser when you click Save.

        /src/App.js:

        function App() {
        return (
        <div className="App">
        <h1>Hello World!</h1>
        </div>
        );
        }

        export default App;

- ### Folder structure
Is there a recommended way to structure React projects?

React doesn’t have opinions on how you put files into folders. That said there are a few common approaches popular in the ecosystem you may want to consider.

Grouping by features or routes
One common way to structure projects is to locate CSS, JS, and tests together inside folders grouped by feature or route.

        common/
            Avatar.js
            Avatar.css
            APIUtils.js
            APIUtils.test.js
        feed/
            index.js
            Feed.js
            Feed.css
            FeedStory.js
            FeedStory.test.js
            FeedAPI.js
        profile/
            index.js
            Profile.js
    ProfileHeader.js
    ProfileHeader.css
    ProfileAPI.js

The definition of a “feature” is not universal, and it is up to you to choose the granularity. If you can’t come up with a list of top-level folders, you can ask the users of your product what major parts it consists of, and use their mental model as a blueprint.

- Grouping by file type
Another popular way to structure projects is to group similar files together, for example:

        api/
            APIUtils.js
            APIUtils.test.js
            ProfileAPI.js
            UserAPI.js
        components/
            Avatar.js
            Avatar.css
            Feed.js
            Feed.css
            FeedStory.js
            FeedStory.test.js
            Profile.js
            ProfileHeader.js
            ProfileHeader.css

Some people also prefer to go further, and separate components into different folders depending on their role in the application. For example, Atomic Design is a design methodology built on this principle. Remember that it’s often more productive to treat such methodologies as helpful examples rather than strict rules to follow.

- ### What is JSX?
JSX stands for JavaScript XML.
JSX allows us to write HTML in React.
JSX makes it easier to write and add HTML in React.
Coding JSX
JSX allows us to write HTML elements in JavaScript and place them in the DOM without any `createElement()`  and/or `appendChild()` methods.
JSX converts HTML tags into react elements.
> You are not required to use JSX, but JSX makes it easier to write React applications.

Here are two examples. The first uses JSX and the second does not:
            
Example 1
uses JSX:
            
        const myElement = <h1>I Love JSX!</h1>;

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(myElement);

Example 2
Without JSX:
            
        const myElement = React.createElement('h1', {}, 'I do not use JSX!');

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(myElement);


- ### CSS in JS
            
- Styled Components ([Link](https://styled-components.com/docs/basics))
- Emotion ([Link](https://emotion.sh/docs/introduction))

- ### Routing
- Query parameters
            
<img src="img/Picture1.png">

- What is a Query Parameter?
            
Query parameters are a defined set of parameters attached to the end of a url.
            
More simply, they are key=value pairs we can attach to a url, used as one of many ways to pass data to an application.
            
Some Pre-requisites
            
First this requires an additional dependency that you may be familiar with, react-router-dom.
            
To install: `npm i --save react-router-dom`
            
Step one: Wrap your project in a Router.

<img src="img/Picture2.png">

In your index.jsx file, when we are rendering our project to the DOM you will have to wrap the outer-most component in a Router tag. This will allow us to have scope of the query params for the next step.

Step two: Writing a function to parse the query params  
            
<img src="img/Picture3.png">

This snippet has a lot going on, so let’s step through it. Also I do want to note, for the snippet above I have used the useEffect method assuming we want to do something with the query params on mounting our component.


- Path parameters ([Link](https://ui.dev/react-router-url-parameters))

- ### Context
React Context is a way to manage state globally.

It can be used together with the useState Hook to share state between deeply nested components more easily than with useState alone.

    import { useState } from "react";
    import ReactDOM from "react-dom/client";

    function Component1() {
    const [user, setUser] = useState("Jesse Hall");

    return (
    <>
    <h1>{`Hello ${user}!`}</h1>
    <Component2 user={user} />
    </>
    );
    }

    function Component2({ user }) {
    return (
    <>
    <h1>Component 2</h1>
    <Component3 user={user} />
    </>
    );
    }

    function Component3({ user }) {
    return (
    <>
    <h1>Component 3</h1>
    <Component4 user={user} />
    </>
    );
    }

    function Component4({ user }) {
    return (
    <>
    <h1>Component 4</h1>
    <Component5 user={user} />
    </>
    );
    }

    function Component5({ user }) {
    return (
    <>
    <h1>Component 5</h1>
    <h2>{`Hello ${user} again!`}</h2>
    </>
    );
    }

    const root = ReactDOM.createRoot(document.getElementById('root'));
    root.render(<Component1 />);



- ### Hooks
- What is a Hook?
Hooks allow us to "hook" into React features such as state and lifecycle methods.

Example:
Here is an example of a Hook. Don't worry if it doesn't make sense.

    import React, { useState } from "react";
    import ReactDOM from "react-dom/client";

    function FavoriteColor() {
    const [color, setColor] = useState("red");

    return (
    <>
    <h1>My favorite color is {color}!</h1>
    <button
    type="button"
    onClick={() => setColor("blue")}
    >Blue</button>
    <button
    type="button"
    onClick={() => setColor("red")}
    >Red</button>
    <button
    type="button"
    onClick={() => setColor("pink")}
    >Pink</button>
    <button
    type="button"
    onClick={() => setColor("green")}
    >Green</button>
    </>
    );
    }

    const root = ReactDOM.createRoot(document.getElementById('root'));
    root.render(<FavoriteColor />);

You must `import` Hooks from `react`.

Here we are using the `useState` Hook to keep track of the application state.

State generally refers to application data or properties that need to be tracked.

Hook Rules
There are 3 rules for hooks:

- Hooks can only be called inside React function components.
- Hooks can only be called at the top level of a component.
- Hooks cannot be conditional

> Note: Hooks will not work in React class components.


- ### Components and Props
components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
Function and Class Components
The simplest way to define a component is to write a JavaScript function:

        function Welcome(props) {
        return <h1>Hello, {props.name}</h1>;
        }

This function is a valid React component because it accepts a single “props” (which stands for properties) object argument with data and returns a React element. We call such components “function components” because they are literally JavaScript functions.

You can also use an ES6 class to define a component:

        class Welcome extends React.Component {
        render() {
        return <h1>Hello, {this.props.name}</h1>;
        }
        }

The above two components are equivalent from React’s point of view.


  ### Parent and Child

- Passing Data From Parent to Child
When you need to pass data from a parent to child class component, you do this by using props.

For example, let’s say you have two class components, Parent and Child, and you want to pass a state in the parent to the child. You would do something like this:

    import React from 'react';

    class Parent extends React.Component{
    constructor(props){
    super(props);
    this.state = {
    data: 'Data from parent'
    }
    }

    render(){
    const {data} = this.state;
    return(
    <div>
    <Child dataParentToChild = {data}/>
    </div>
    )
    }
    }

    class Child extends React.Component{
    constructor(props){
    super(props);
    this.state = {
    data: this.props.dataParentToChild
    }
    }

    render(){
    const {data} = this.state;
    return(
    <div>
    {data}
    </div>
    )
    }
    }

    export default Parent;

As you can see, the parent component passes props to the child component and the child can then access the data from the parent via this.props.

For the same example, if you have two function components instead of class components, you don’t even need to use props. You can do something like the following:

    import React from 'react';

    function Parent(){
    const data = 'Data from parent';
    return(
    <div>
    <Child dataParentToChild = {data}/>
    </div>
    )
    }

    function Child ({dataParentToChild}){
    return(
    <div>
    {dataParentToChild}
    </div>
    )
    }

    export default Parent;
                                   
- ### Child to Parent

Passing the data from the child to parent component is a bit trickier. In order to do this, you need to do the following steps:

- Create a callback function in the parent component. This callback function will get the data from the child component.
- Pass the callback function in the parent as a prop to the child component.
- The child component calls the parent callback function using props.

Let’s see how these steps are implemented using an example. You have two class components, Parent and Child. The Child component has a form that can be submitted in order to send its data up to the Parent component. It would look something like this:

    import React from 'react';

    class Parent extends React.Component{
    constructor(props){
    super(props);
    this.state = {
    data: null
    }
    }

    handleCallback = (childData) =>{
    this.setState({data: childData})
    }

    render(){
    const {data} = this.state;
    return(
    <div>
    <Child parentCallback = {this.handleCallback}/>
    {data}
    </div>
    )
    }
    }

    class Child extends React.Component{
  
    onTrigger = (event) => {
    this.props.parentCallback("Data from child");
    event.preventDefault();
    }

    render(){
    return(
    <div>
    <form onSubmit = {this.onTrigger}>
    <input type = "submit" value = "Submit"/>
    </form>
    </div>
    )
    }
    }

    export default Parent;

As you can see, when the Child component is triggered, it will call the Parent component’s callback function with data it wants to pass to the parent. The Parent’s callback function will handle the data it received from the child.

We’ve gone over passing data between a parent and child components in React. Just as a recap, here’s the different methods we’ve covered:

- Passing data from parent to child class components
- Passing data from parent to child function components
- Passing data from child to parent



- Handling Events

•React events are named using camelCase, rather than lowercase.
            
•With JSX you pass a function as the event handler, rather than a string.
            
For example, the HTML:
            
        <button onclick="activateLasers()">
        Activate Lasers
        </button>
            
is slightly different in React:
            
        <button onClick={activateLasers}>  Activate Lasers
        </button>
            
Another difference is that you cannot return false to prevent default behavior in React. You must call preventDefault explicitly. For example, with plain HTML, to prevent the default form behavior of submitting, you can write:
            
        <form onsubmit="console.log('You clicked submit.'); return false">
        <button type="submit">Submit</button>
        </form>
In React, this could instead be:
            
        function Form() {
        function handleSubmit(e) {
        e.preventDefault();    console.log('You clicked submit.');
        }

        return (
        <form onSubmit={handleSubmit}>
        <button type="submit">Submit</button>
        </form>
        );
        }
            
Here, e is a synthetic event. React defines these synthetic events according to the W3C spec, so you don’t need to worry about cross-browser compatibility. React events do not work exactly the same as native events. See the SyntheticEvent reference guide to learn more.

When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created. Instead, just provide a listener when the element is initially rendered.

When you define a component using an ES6 class, a common pattern is for an event handler to be a method on the class. For example, this Toggle component renders a button that lets the user toggle between “ON” and “OFF” states:
            
        class Toggle extends React.Component {
        constructor(props) {
        super(props);
        this.state = {isToggleOn: true};

        // This binding is necessary to make `this` work in the callback    this.handleClick = this.handleClick.bind(this);  }

        handleClick() {    this.setState(prevState => ({      isToggleOn: !prevState.isToggleOn    }));  }
        render() {
        return (
        <button onClick={this.handleClick}>        {this.state.isToggleOn ? 'ON' : 'OFF'}
        </button>
        );
        }
        }



- Conditional Rendering
            
Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.
Consider these two components:
            
        function UserGreeting(props) {
        return <h1>Welcome back!</h1>;
        }

        function GuestGreeting(props) {
        return <h1>Please sign up.</h1>;
        }
            
We’ll create a Greeting component that displays either of these components depending on whether a user is logged in:
            
        function Greeting(props) {
        const isLoggedIn = props.isLoggedIn;
        if (isLoggedIn) {    return <UserGreeting />;  }  return <GuestGreeting />;}
        const root = ReactDOM.createRoot(document.getElementById('root')); 
        // Try changing to isLoggedIn={true}:
        root.render(<Greeting isLoggedIn={false} />);

- Lists and Keys
Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:
            
        const numbers = [1, 2, 3, 4, 5];
        const doubled = numbers.map((number) => number * 2);console.log(doubled);
            
This code logs [2, 4, 6, 8, 10] to the console.
In React, transforming arrays into lists of elements is nearly identical.
Rendering Multiple Components
You can build collections of elements and include them in JSX using curly braces {}.
Below, we loop through the numbers array using the JavaScript map() function. We return a < li> element for each item. Finally, we assign the resulting array of elements to listItems:
            
        const numbers = [1, 2, 3, 4, 5];
        const listItems = numbers.map((number) =>  <li>{number}</li>);
        Then, we can include the entire listItems array inside a <ul> element:
        <ul>{listItems}</ul>

- Forms
            
HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. For example, this form in plain HTML accepts a single name:
            
        <form>
        <label>
        Name:
        <input type="text" name="name" />
        </label>
        <input type="submit" value="Submit" />
        </form>
            
This form has the default HTML form behavior of browsing to a new page when the user submits the form. If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.
 

- Composition vs Inheritance
            
we will consider a few problems where developers new to React often reach for inheritance, and show how we can solve them with composition.
            
- Containment
            
Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”.
            
We recommend that such components use the special children prop to pass children elements directly into their output:
            
        function FancyBorder(props) {
        return (
        <div className={'FancyBorder FancyBorder-' + props.color}>
        {props.children}    </div>
        );
        }
            
This lets other components pass arbitrary children to them by nesting the JSX:
            
        function WelcomeDialog() {
        return (
        <FancyBorder color="blue">
        <h1 className="Dialog-title">        Welcome      </h1>      <p className="Dialog-message">        Thank you for visiting our spacecraft!      </p>    </FancyBorder>
        );
        }


- ### Routing
- Query parameters
            
<img src="img/Picture1.png">

- What is a Query Parameter?
            
Query parameters are a defined set of parameters attached to the end of a url.
            
More simply, they are key=value pairs we can attach to a url, used as one of many ways to pass data to an application.
            
Some Pre-requisites
            
First this requires an additional dependency that you may be familiar with, react-router-dom.
            
To install: `npm i --save react-router-dom`
            
Step one: Wrap your project in a Router.

<img src="img/Picture2.png">

In your index.jsx file, when we are rendering our project to the DOM you will have to wrap the outer-most component in a Router tag. This will allow us to have scope of the query params for the next step.

Step two: Writing a function to parse the query params  
            
<img src="img/Picture3.png">

This snippet has a lot going on, so let’s step through it. Also I do want to note, for the snippet above I have used the useEffect method assuming we want to do something with the query params on mounting our component.


- Path parameters ([Link](https://ui.dev/react-router-url-parameters))

- ### Context
React Context is a way to manage state globally.

It can be used together with the useState Hook to share state between deeply nested components more easily than with useState alone.

    import { useState } from "react";
    import ReactDOM from "react-dom/client";

    function Component1() {
    const [user, setUser] = useState("Jesse Hall");

    return (
    <>
    <h1>{`Hello ${user}!`}</h1>
    <Component2 user={user} />
    </>
    );
    }

    function Component2({ user }) {
    return (
    <>
    <h1>Component 2</h1>
    <Component3 user={user} />
    </>
    );
    }

    function Component3({ user }) {
    return (
    <>
    <h1>Component 3</h1>
    <Component4 user={user} />
    </>
    );
    }

    function Component4({ user }) {
    return (
    <>
    <h1>Component 4</h1>
    <Component5 user={user} />
    </>
    );
    }

    function Component5({ user }) {
    return (
    <>
    <h1>Component 5</h1>
    <h2>{`Hello ${user} again!`}</h2>
    </>
    );
    }

    const root = ReactDOM.createRoot(document.getElementById('root'));
    root.render(<Component1 />);

- ### Create Context
To create context, you must Import createContext and initialize it:


    import { useState, createContext } from "react";
    import ReactDOM from "react-dom/client";

    const UserContext = createContext()

Next we'll use the Context Provider to wrap the tree of components that need the state Context.

- ### Context Provider
Wrap child components in the Context Provider and supply the state value.

    function Component1() {
    const [user, setUser] = useState("Jesse Hall");

    return (
    <UserContext.Provider value={user}>
    <h1>{`Hello ${user}!`}</h1>
    <Component2 user={user} />
    </UserContext.Provider>
    );
    }

Now, all components in this tree will have access to the user Context.

- ### Use the useContext Hook
In order to use the Context in a child component, we need to access it using the useContext Hook.

First, include the useContext in the import statement:

    import { useState, createContext, useContext } from "react";

Then you can access the user Context in all components:

    function Component5() {
    const user = useContext(UserContext);

    return (
    <>
    <h1>Component 5</h1>
    <h2>{`Hello ${user} again!`}</h2>
    </>
    );
    }

- ### What is Prop Drilling?

Anyone who has worked in React would have faced this and if not then will face it definitely. Prop drilling is basically a situation when the same data is being sent at almost every level due to requirements in the final level. Here is a diagram to demonstrate it better. Data needed to be sent from Parent to ChildC. In this article different ways to do that are discussed.

Example 1: With using Prop Drilling

    import React, { useState } from "react";
  
    function Parent() {
    const [fName, setfName] = useState("firstName");
    const [lName, setlName] = useState("LastName");
    return (
    <>
    <div>This is a Parent component</div>
    <br />
    <ChildA fName={fName} lName={lName} />
    </>
    );
    }
  
    function ChildA({ fName, lName }) {
    return (
    <>
    This is ChildA Component.
    <br />
    <ChildB fName={fName} lName={lName} />
    </>
    );
    }
  
    function ChildB({ fName, lName }) {
    return (
    <>
    This is ChildB Component.
    <br />
    <ChildC fName={fName} lName={lName} />
    </>
    );
    }
  
    function ChildC({ fName, lName }) {
    return (
    <>
    This is ChildC component.
    <br />
    <h3> Data from Parent component is as follows:</h3>
    <h4>{fName}</h4>
    <h4>{lName}</h4>
    </>
    );
    }
  
    export default Parent;


- ### why key is importent in list
A “key” is a special string attribute you need to include when creating lists of elements in React. Keys are used in React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the lists.

    const numbers = [ 1, 2, 3, 4, 5 ];
 
    const updatedNums = numbers.map((number)=>{
    return <li key={index}>{number} </li>;
    });

You can also assign the array indexes as keys to the list items. The below example assigns array indexes as key to the elements. 

    const numbers = [ 1, 2, 3, 4, 5 ];
 
    const updatedNums = numbers.map((number, index)=>
    <li key = {index}>
    {number}
    </li>
    );

Assigning indexes as keys are highly discouraged because if the elements of the arrays get reordered in the future then it will get confusing for the developer as the keys for the elements will also change.

- ### What is an arrow function and how is it used in React?

     - An arrow function is a short way of writing a function to React.
     - It is unnecessary to bind ‘this’ inside the constructor when using an arrow function. This prevents bugs caused by the use of ‘this’ in React callbacks.

![image](https://user-images.githubusercontent.com/117704825/204689454-30eeeb3e-260a-447a-86ae-c3296f3b2724.png)

