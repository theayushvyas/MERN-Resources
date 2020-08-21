## INTRO
**Node JS is a javascript runtime to compile javascript code on the server side . it is not a framework or library .**

Earlier JS code can only be compiled on browser . different browser supports different JS Engine like IE used Chakra , Firefox uses Spider Monkey and Chrome has v8.

So in 2009 **Ryan Dhal** developed node JS.

Node JS is a JS runtime based on  Google Chrome's v8 Engine(Because it is the fastest among all js engine) and written in c++.

Applications build with Node JS are fast,Responsive and highly Scalable because of its non blocking and asynchronous Nature or architechure.

Non blocking means after takinga request it does'nt block until the first request in completed.

It uses a **SINGLE THREAD** to take multiple request and serve them as per the response arrive. It do not block anyone after taking a request.
Eg: In a Restaurent a Single waiter takes order from multiple customers and give to the chef . and serve them as per their food gets ready
