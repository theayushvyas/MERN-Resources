## File Based Module
File system Modules are installed locally in your Node JS application , and the are for the purpose on interconnecting different files
 Eg: In this eg we will print Hello World But using two different Files .
 
 
 There are two ways to export any module 
 **Way 1**
 **Example.js**
 ```
 export.exp= "World";  //Exporting and assigning value at same time.
 
 ```
 **File 2**
 ```
 Const example = require('./example.js');  //Importing that file in const named exp
 console.log("Hello" + example.exp)          //Calling exp from Example  
 ```
 
 **2nd WAY**
 
 **calc.js**
 ```
 add = (a,b) =>(a+b);  //Assigning the Value
 
 export.add = add;  //No Exporting it.
 ```
 **Index.js**
 ```
 const calc = require('./Calc.js');
 
 console.log(calc.add(5,3));  //This is first Way we can use the exported file
 
 Const add = (a,b) =>{      //The second way is by creating a function.
 console.log(calc.add(a,b))
 }
 add(5,6);   //Calling the add funcatuion to put the value of a,b
 ```


## Core Modules
Core Modules are the build in modules are those who come along with Node.


eg(http,fs,path)

```
const http = require('http');

const server = http.createServer((req,res) => {
	res.end("Connection Successfull")
	})
    
    server.listen(3030, ()=>{
		console.log('Running Successfull on 3030')  //Callback 
	})
```


## External Modules
External are third party modules we need to first download and install them on our project using npm install
Eg : We will install  super heroes , a module which prints out random super heroes name.


first we need to do  

`npm install superheroes`


```
const hero = require('superheroes');

console.log(hero.random());     //any one random name
console.log(hero.all());       //Prints out all the names

```

