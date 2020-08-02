# MongoDB

## using a db
`use <DB_NAME>`

## Create 
`db.createCollection(<CollectionName>)`

##  Find
`db.<CollectionName>.find(<OBJECT>)`

### find all 
`db.<CollectionName>.find()`


### **sorting**
`db.<CollectionName>.find().sort(<SORTING_OBJECT>)`

#### desc sorting
	`db.<CollectionName>.find().sort({ <KEY> : -1 })`
	
#### $elemMatch

****
#### $gt / $gte / $lt / $lte

## Update
`db.<CollectionName>.update({ })`

## $set a spectific field

``` 
db.[CollectionName].update({ 
$set: {
	// target specific fields here
}
})
``` 

### rename a field

## Deleting
