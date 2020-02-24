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

### 6. What is JSX?

JSX is a XML-like syntax extension to ECMAScript (the acroym stands for JavaScript XML). This is a type of file used by React which utilizes the expressiveness of Javascript along with HTML like template syntax. This makes the HTML file really easy to understand. JSX syntax can be compiled by Babel.

### 7. Why can't browsers read JSX?

Browsers can only read JavaScript objects but JSX is not a regular JavaScript object. Thus to enbale a browser to read JSX, we need to transform JSX file into a JavaScript object like using Babel and then pass it to the broswer.

### 8. How is React different from Angular?

| TOPIC | REACT | ANGULAR |
| ----- | ----- | ------- |
| Architecture | Only the view of MVC | Complete MVC |
| Rendering | Server-side rendering | Client-side rendering |
| DOM | Uses virtual DOM | Uses real DOM |
| Data Binding | One-way data binding | Two-way data binding |
| Debugging | Compile time debugging | Runtime debugging |
| Author | Facebook | Google |

### 9. Stateful component (class component) VS Stateless component (functional component)

| Stateful component (class component) | stateless component (functional component) |
| ------------------------------------ | ------------------------------------------ |
| Stores info about component's state change in memory | Calculates the internal state of the components |
| Have authority to change state | Do not have authority to change state |
| Contains the knowledge of past, current and possible future changes in state | Contains no knowledge of past, current and possible future changes in state |
| Stateless components notify them about the requirement of the state change, then they send down the props to them | They receive the props from stateful components and treat them as callback functions |

### 10. What are the different phases of React component's lifecycle?

There are three different phases of React component's lifecycle:

1. *Initial Rendering Phase:* This is the phase when the component is about to start its life journey and make its way to the DOM.

2. *Updating Phase:* Once the component gets added to the DOM, it can potentially update and re-render only when a prop or state change occurs. That happens only in this phase.

3. *Unmounting phase:* This is the final phase of a component's life cycle in which the component is destroyed and removed from the DOM.

### 11. Explain the lifecycle methods of React components in detail.

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

### 12. What are Higher Order Components(HOC)?

Higher Order Component is an advanced way of resuing the component logic. Basically, it's a pattern that is derived from React's compositional nature. HOC are custom components which wrap another component within it. They can accept any dynamically provided child component but they won't modify or copy any behavior from their input components. You can say that HOC are `pure` component.
