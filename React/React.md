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


