## Components
Components , In React JS every thing is a component ,every part you see or e can say that a React JS web page is a made up of joining many small components.
**To return more than one element we need to use** `<div>`**element  or react fragments **

### Types of components.

- Functional Components
- Class Components


### Functional Components
  - Functional Components are just normal javascript functions that simply accepts some data and display them or renders the UI element . 
  - Functional components are also known as Stateless Components because they dont have any states , or we can't use {this.State} inside functional components but 
    Functional components can accepts {props} Properties and we can use them inside functional Components.
  - Their is no render() method inside functional Components
  - These are mainly responsible for UI and are typically presentational only (For example, a Button component).
  - Functional components should be favored if you do not need to make use of React state.
  
  
  We can use both regular and arrow function.
  Eg:
  ```
  function Hello(props){
  return(
  <div>
  <h1>Hello {props.name}</h1>  
  <p>Hope you are Doing Good !!</p>
  <div>
  )
  };
  
  ```
  **Using Arrow Function**
  ```
  const Hello = ({name}) => 
  <div>
  Hello {name}
  </div>
  ```
  
### Class Components
Class Components on the other way are a bit complex. It has states , Lifecycle components 
Class Components make use of ES6 class and extends components and by extending components react will know that this is a class components and render() function is available inside components. We can use state in class components
```
class Hello extends components{
render(){
return(
<div>
<h1>Hello</h1>
</div>
)}}
```

### How to return more than one element ?
- We can return more than one element inside `<div></div>` or simply using react fragments `<></>`. When returining only one element we can ignore these and directly return without using these tags.

###  Why returning more than one element is not allowed in React JS ?
 - React implementation relies on constructing a tree like structure which it uses to for reconcilation. When you return multiple elements from React elements from the render method, the assumtion that the tree will have one root node for the Component will not longer hold, hence making it difficult to process reconcilation algorithm.

Thus react gives you a limitation to provide a root node. If you return an array of elements from v16 onwards, react will internally create a dummy node as the parent. 
