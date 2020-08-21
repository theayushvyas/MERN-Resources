## INTRO
**Node JS is a javascript runtime to compile javascript code on the server side . it is not a framework or library .**

Earlier JS code can only be compiled on browser . different browser supports different JS Engine like IE used Chakra , Firefox uses Spider Monkey and Chrome has v8.

So in 2009 **Ryan Dhal** developed node JS.

Node JS is a JS runtime based on  Google Chrome's v8 Engine(Because it is the fastest among all js engine) and is written in c++.

Applications build with Node JS are fast,Responsive and highly Scalable because of its non blocking and asynchronous Nature or architechure.

Non blocking means it does'nt block other until the response of first request in completed.

It uses a **SINGLE THREAD** to take multiple request and Whenever the database result(response of request) is ready it puts a message in the **Event Queue** , Node is continously monitoring its event queue in background , and whenever it finds an Event Due in this Queue it takes it out and process(Serve) it. so It do not block anyone after taking a request else it takes all the request and process them.

Eg: In a Restaurent a Single waiter takes order from multiple customers and gives it to the chef to prepare and  then serve them as per their food gets ready

Earlier javascript was never meant to be run outside the browser ,and it does'nt come with any module system. So we have to the whole code in a single file,Which become very cubersome for large projects . Then CommonJS API comes to fill this gap by defining a module format Which allow users to breakup the code in multiple JS files and access them from anywhere. so Node JS provide user different modules which allow users to intergrate all the diferent file in a single file by simpluy we can say importing them.

NodeJS is Module Based.

## Types of Modules in Node JS.

1. File Based Modules
2. Core Modules(Build-in Modules)
3. External Node Modules
