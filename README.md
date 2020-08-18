# MongoDB-
MongoDB Commands

**General Commands**

1)show dbs.
--> To show all the databases . database must have atleast 1 collection in it to get it Shown . database without collection will not be visible using this or any command.


2) use <Database Name> eg:use Project
--> To switch database. if database does'nt exist it will create one of same name and Switch to it. as switching and creating is with same command in mongo.


3) db.dropDatabase()
--> To delete Current Database.


4)show collection
--> To view all the collections in the Database.


5)db.createCollection("Collection Name") eg;db.createCollection("Name")
-->To create a new collection inside database.


6) db.<collectionName>.insert({<key> : <value>, <key> : <value>})  eg:db.Qualifications.insertOne({id:1 ,"Name":"Ayush","Age":21,"Degree":"B.Tech"})
--> To Insert Record In a Collection.


7)db.<Collection Name>.insertMany([{Data 1},{data 2},{Data n}])
Eg:db.Qualification.insertMany([{id:2 ,"Name":"Vyas","Age":21,"Degree":"B.Tech"},{id:3,"Name":"Pratyaksh","Age":22,"Degree":"BA"}])
--> use insertMany() to insert more then one data in single go.
 
