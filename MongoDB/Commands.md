## MERN Resources
MERN stack resources - code snippets and general commands

### MongoDB

#### General Commands

1. `show dbs`
- To show all the databases . database must have atleast 1 collection in it to get it Shown . database without collection will not be visible using this or any command.


2. `use <Database Name>` eg: `use Project`
- To switch database. if database does'nt exist it will create one of same name and Switch to it. as switching and creating is with same command in mongo.


3. `db.dropDatabase()`
- To delete the current Database.


4. `show collection`
- To view all the collections in the Database.


5. `db.createCollection("Collection Name")` eg: `db.createCollection("Name")`
- To create a new collection inside database.


6. `db.<collectionName>.insertOne({<key> : <value>, <key> : <value>})`  
Eg: `db.Qualifications.insertOne({id:1 ,"Name":"Ayush","Age":21,"Degree":"B.Tech"})`
- To Insert Record In a Collection.


7. `db.<Collection Name>.insertMany([{Data 1},{data 2},{Data n}])`
Eg: `db.Qualification.insertMany([{id:2 ,"Name":"Vyas","Age":21,"Degree":"B.Tech"},{id:3,"Name":"Pratyaksh","Age":22,"Degree":"BA"}])`
- Use insertMany() to insert more than one data in a single go.
 
8.  `db.<Source Name>.copyTo("Target Name")`
Eg: `db.Name.copyTo("Qualifications")`
- To Copy all the data from one collection to anathor withing SAME DATABASE.

9.   `db.<Collection Name>.updateOne({Ref of what value to be updated},{$set:{Updated Value}})`
Eg: `db.Qualifications.update({"Name":"Gajju"},{$set:{"Degree":"ITUS"}})`
- To Update an Existing Value 
**Use updateMany() to Update More than One Value at once**


10.   `db.<Collection Name>.drop()`
- Will Delete that Collection.
