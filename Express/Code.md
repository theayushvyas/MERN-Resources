## Hello-World in Express

install Express From `npm install -g express`

```
const express =  require('express');    //First of all we need to require Express like this or we can say we are importing express package in a const named express.
var app = express();                    //Now after importing it here we are letting our app to use express. just like after importing scanner in java we create an object for scanner function
to use it.

app.get('/',function(req,res){
res.send('Hello World');
});
app.listen(3000, (req,res) => {
console.log("Server Started Successfully on port 3000 !! ");
});
```
