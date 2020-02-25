# React Interview Questions

### 1. What is React?

* React is front-end JavaScript library developed by facebook in 2011.
* It follows the component based approach which helps in building **resuable UI components**
* It is used for developing complex and interactive web and mobile UI.

### 2. What are the features of React?

* It uses the **virtual DOM** instead of the real DOM.
* It uses **server-side rendering**.
* it follows **uni-directional data flow** or **data binding**.

### 3. List some of the major advantages of React.

* It increases the application's performance.
* It can be conveniently used on the client as well as server side.
* Because of JSX, code readability increases.
* React is easy to integrate with other framework like Meteor, Angular, etc.

### 4. What are the limitations of React?

* React is just a library, not a full-blown framework
* Its library is very large and takes time to understand
* It can be difficult for the novice programmers to understand
* Coding gets complex as it uses inline templating and JSX

### 5. What is the difference between Real DOM and Virtual DOM?

| Virual DOM | Real DOM |
| ---------- | -------- |
| It updates slow | It updates faster |
| Can directly update HTML | Can't directly update the HTML |
| Create a new DOM if element updates | Updates JSX if element updates |
| DOM manipulations is very expensive | DOM manipulation is very easy |
| Too much of memory wastage | No memory wastage |

### 6. What do you understand by Virtual DOM? Explain how it works.

A virtual DOM is a **lightWeight JavaScript object** which originally is just **the copy of the real DOM**. it is node tree that lists the elements, their attributes and content as Objects and their properties. React's render function creates a node tree out of the React components. It then updates this tree in response to the mutations in the data model which is caused by various actions done by the user or by the system.

The Virtual DOM works in three simple steps.

1. Whenever any underlying data changes, the entire UI is re-rendered in Virtual DOM representation.

2. Then the difference between the previous DOM representation and the new one is calculated.

3. Once the calculations are done, the real DOM will be updated with only the things that have actually changed.

### 7. What is JSX?

JSX is a XML-like syntax extension to ECMAScript (the acroym stands for JavaScript XML). This is a type of file used by React which utilizes the expressiveness of Javascript along with HTML like template syntax. This makes the HTML file really easy to understand. JSX syntax can be compiled by Babel.

### 8. Why can't browsers read JSX?

Browsers can only read JavaScript objects but JSX is not a regular JavaScript object. Thus to enbale a browser to read JSX, we need to transform JSX file into a JavaScript object like using Babel and then pass it to the broswer.

### 9. How is React different from Angular?

| TOPIC | REACT | ANGULAR |
| ----- | ----- | ------- |
| Architecture | Only the view of MVC | Complete MVC |
| Rendering | Server-side rendering | Client-side rendering |
| DOM | Uses virtual DOM | Uses real DOM |
| Data Binding | One-way data binding | Two-way data binding |
| Debugging | Compile time debugging | Runtime debugging |
| Author | Facebook | Google |

### 10. Stateful component (class component) VS Stateless component (functional component)

| Stateful component (class component) | stateless component (functional component) |
| ------------------------------------ | ------------------------------------------ |
| Stores info about component's state change in memory | Calculates the internal state of the components |
| Have authority to change state | Do not have authority to change state |
| Contains the knowledge of past, current and possible future changes in state | Contains no knowledge of past, current and possible future changes in state |
| Stateless components notify them about the requirement of the state change, then they send down the props to them | They receive the props from stateful components and treat them as callback functions |

### 11. What are the different phases of React component's lifecycle?

There are three different phases of React component's lifecycle:

1. *Initial Rendering Phase:* This is the phase when the component is about to start its life journey and make its way to the DOM.

2. *Updating Phase:* Once the component gets added to the DOM, it can potentially update and re-render only when a prop or state change occurs. That happens only in this phase.

3. *Unmounting phase:* This is the final phase of a component's life cycle in which the component is destroyed and removed from the DOM.

### 12. Explain the lifecycle methods of React components in detail.

* Mounting
  * **constructor()**
  * static getDerivedStateFromProps()
  * **render()**
  * **componentDidMount()**

* Updating
  * static getDerivedStateFromProps()
  * shouldComponentUpdate()
  * **render()**
  * getSnapshotBeforeUpdate()
  * **componentDidUpdate()**

### 13. What are Higher Order Components(HOC)?

Higher Order Component is an advanced way of resuing the component logic. Basically, it's a pattern that is derived from React's compositional nature. HOC are custom components which wrap another component within it. They can accept any dynamically provided child component but they won't modify or copy any behavior from their input components. You can say that HOC are `pure` component.

### 14. What do you understand from "In React, everything is a component".

Components are the building blocks of a React application's UI. These components split up the entire UI into small independent and reusable pieces. Then it renders each of these components independent of each other without affecting the rest of the UI.

### 15. What is Props?

Props is the shorthand for Properties in React. They are read-only components which must be kept pure i.e. immutable. They are always passed down from the parent to the child components throughout the application. A child component can never send a prop back to parent component. This help in maintaining the unidirectional 

### 16. What is a state in React and how is it used?

States are the heart of React components. States are the source of data and must be kept as simple as possible. Basically, states are the objects which determine components rendering and behavior. States are the objects which determine components rendering and behavior. They are mutable unlike the props and create dynamic and interactive components.

### 17.What is ref in React?

Ref is the shorthand for Reference in React. It is an attribute which helps to store a reference to a particular React element or component, which will be returned by the components render configuration function. It is used to return references to a particular element or component returned by render(). They come in handy when we need DOM measurements or to add methods to the components.

### 18. List some of the cases when you should use Ref.

Following are the cases when ref should be used:

* When you need to manage focus, select text or media playback
* To trigger imperative animations
* Integrate with thrid-party DOM libraries.


