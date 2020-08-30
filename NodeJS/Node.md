## INTRO
**Node JS is a javascript runtime to compile javascript code on the server side . it is not a framework or library .**

Earlier JS code can only be compiled on browser . different browser supports different JS Engine like IE used Chakra , Firefox uses Spider Monkey and Chrome has v8.

So in 2009 **Ryan Dhal** developed node JS.

Node JS is a JS runtime based on  Google Chrome's v8 Engine(Because it is the fastest among all js engine) and is written in c++.

Applications build with Node JS are fast,Responsive and highly Scalable because of its non blocking and asynchronous Nature or architechure.

Non blocking means it does'nt block other until the response of first request in completed.

It uses a **SINGLE THREAD** to take multiple request and Whenever the database result(response of request) is ready it puts a message in the **Event Queue** , Node is continously monitoring its event queue in background , and whenever it finds an Event Due in this Queue it takes it out and process(Serve) it. so It do not block anyone after taking a request else it takes all the request and process them.

Eg: In a Restaurent a Single waiter takes order from multiple customers and gives it to the chef to prepare and  then serve them as per their food gets ready
## Event Driven Programming

Event driven programming means that building our application respond to a certain event , like a click or key press .When an event is occur we are calling a **Callback Function** which is registered with the element that event . In short it is based on the certain Events ,**One Real life Example is our Smartphone's Finger Print Sensor it responds every time we touch it , or it runs a callback which unlocks the phone if the finger print matches**

## Event Loop and Event Queue
Event loop is what makes Nodejs Fast , scalable and Non Buffereing .Being using single threaded structure ,Node JS achieve concurrency via Event loop and event handles, Event Loop allow Node JS to  perform non blocking operation despite being single threaded. So how NodeJS achieve Non-Blocking and async architechture is it asks the OS or the threadpool to achieve the task for the , as our OS is multi threaded it execute all the tasks asynchronously and whenever the task is achieved the callback function attached to it is fired.

## Callback Function
Callback function is very important concept in Node JS. Every Event is attached to a callback function and whenever an event is completed then the call back function is call, Which help us know which task is completed first.

**Imp points to remember**
- Callback Function is the last parameter of any function , it is executed after the task is completed.

- First parameter of any callback funcation is by default **error** , If any error occurs it will let us know.

- Second Parameter is Data. Data to be returened.

**Non-Blocking and Callback example**
```
fs.readFile('/random.txt'),function(err,data){
if(err) return console.log(err);
console.log(data);
	
}
console.log(Reading File);
```
   **output** 

 Reading File

 File Data

 This Example shows that the program does not wait for file reading and proceeds to print "Reading File" and at the same time, the program without blocking continues reading the file and when the file data is ready , the callback function attached to it gets fired and print the data of the file Or error(If Any) .

## Callback Hell
Callback Hell is pyramid like unmanagable structure of Nested callback Functions , if any one function  gets an error it will effect all the function , it is very complex and unmanagable loop of callbacks that is why it is known as Callback Hell

## REPl
REPL Provides Shell like or cmd like enevironment .REPL in Node.js stands for Read, Eval, Print, and Loop. It represents a computer environment such as a window console or Unix/Linux shell where any command can be entered and then the system can respond with an output. Node.js comes bundled with a REPL environment by default. REPL can perform the below-listed tasks

   - Read: Reads the user’s input, parses it into JavaScript data-structure and then stores it in the memory.
   - Eval: Receives and evaluates the data structure.
   - Print: Prints the final result.
   - Loop: Loops the provided command until CTRL+C is pressed twice.

## Modules
Earlier javascript was never meant to be run outside the browser ,and it does'nt come with any module system. So we have to the whole code in a single file,Which become very cubersome for large projects . Then CommonJS API comes to fill this gap by defining a module format Which allow users to breakup the code in multiple JS files and access them from anywhere. so Node JS provide user different modules which allow users to intergrate all the diferent file in a single file by simpluy we can say importing them.

NodeJS is Module Based.

## Types of Modules in Node JS.

- File Based Modules
  
- Core Modules(Build-in Modules)

- External Node Modules

For more in-depth Knowledge with code Snippets of Node JS Modules Visit Here : - [Modules Code Snippet](./Code.md)
