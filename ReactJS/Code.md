## Components
Components , In React JS every thing is a component ,every part you see or e can say that a React JS web page is a made up of joining many small components.
**To return more than one element we need to use `<div>`element  or react fragments **
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
