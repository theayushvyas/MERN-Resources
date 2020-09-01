## Introduction 
React JS is a javascript library for front end web development. React is used to build single-page applications.

React allows us to create reusable UI components. It is created by Facebook and first deployed on facebook feeds in 2011 , and open source in 2013. ReactJS follows component based architecture and used virtual dom.

it is easy to learn ,highly Scalable and uses component based architecture.

**Installation**
`npm install -g create-react-app`  //create-react-app is the package to create and run react app

and then run

`create-react-app Myfirstapp`  

## Some Important concepts of ReactJS

- React JS used the concept of Virtual which makes it fast , efficient and highly productive for building single page application.
- The html like format we use inside react js components is actually JSX (JavaScript XML or Javascript Extention ).

## DOM(Document Object Model)
The Document Object Model is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure where in each node is an object representing a part of the document.
### Virtual Dom
The DOM in simple words represents the UI of your application .The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM. This process is called **reconciliation**.You can think of the virtual DOM like a blueprint. It contains all the details needed to construct the DOM, but because it doesn't require all the heavyweight parts that go into a real DOM, it can be created and changed much more easily and we dont need to change it in real dom every time.


### Problem with the Real Dom ?
As we know that Dom represents the UI of the application , and Dom is represented in **Tree Data Structure** because of which updates in Dom are faster but after the update , The updated elements and its childrens have to be re-render to update the UI this is what makes real dom slow.


### How virtual dom solve's this problem ?
React dom is much much faster then the virtual dom , Every time we update any thing Whole Virtual dom gets updated instead of the real dom,then Virtual dom compare itself to what it look like before update and figure out what is changed/updated after this virtual dom syncs with the real dom and only that updated part is changes in the real dom and this saving time.

**This whole process is called reconciliation**

**And the algorithm which is used to figure out what is changed in updated virtual dom and previous virtual is known as diffing algorithm**

### React Fiber
Fiber is the new reconciliation engine in React 16. Its main goal is to enable incremental rendering of the virtual DOM.


## Components 
Components is most important thing to remember while working with react. Every thing in react is a component ,We can say that a react UI is a combination of components .Just like a Puzzel

![A Puzzel Image](https://raw.githubusercontent.com/theayushvyas/MERN-Resources/master/ReactJS/Puzzel.jpg)
