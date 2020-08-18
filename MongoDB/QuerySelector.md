**Query Selector**

## Comparision ##

1.  $eq - Find all value equal to given value.
`db.<Collection Name>.find(value : Equal To)`
Eg: `db.Qualifications.find({Age: {$eq:20}}) or db.Qualifications.find({Age : 20}) Both Are Same.`

2.  $ne - Find all value not equal to given value.
`db.<Collection Name>.find(value : not Equal To)`
Eg: `db.Qualifications.find({Age: {$ne:20}})`


3.  $gt - Return all Enteries with values Greater then the entered Value.
`db.<Collection Name>.find(value : {$gt : Greater Than To)`  
Eg: `db.Qualifications.find({Age: {$gt:20}})`

4.  $gte - Return all Enteries with values Equal and Greater to the entered Value.
`db.<Collection Name>.find(value : {$gte : Equal and Greater To)`  
Eg: `db.Qualifications.find({Age: {$gte : 21}})`

5.  $lt - Return all Enteries with values Less then the entered Value.
`db.<Collection Name>.find(value : {$lt : Less Than To)`  
Eg: `db.Qualifications.find({Age: {$lt:24}})`

6.  $lt - Return all Enteries with values Equal and Less to the entered Value.
`db.<Collection Name>.find(value : {$lt : Less and equal To)`  
Eg: `db.Qualifications.find({Age: {$lt:25}})`

7. $nin - return all value not equal to specified values


## Logical Operators ##

8)$and - AND Operation , returns Entry Where both the specified values are true**
Eg: `db.Qualification.find({$and : [{Age : 20},{Degree : "BA"}]})`

9)$or - OR Operation , Return Entry where any one of the Value Matches.**
Eg: `db.Qualification.find({$or : [{Age : 24},{Degree: "B.Tech"}]})`
