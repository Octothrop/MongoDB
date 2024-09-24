## Install MongoDB CLI 
1. Install MongoDB CLI from `https://www.mongodb.com/try/download/shell`
2. Extract the folder items > Navigate to bin folder > copy the path
3. Edit System Environment > Environment Variables > Path > Edit > New > paste the copied path > ok > ok > ok 
4. Chcek if the mogosh ia available on terminal using `mongosh --version`

## MongoDB as Service 
1. Download the .msi from `https://www.mongodb.com/try/download/community`
2. Run the .msi file
 
## Get started
1. Open PowerShell in administrative mode > run `net start MondoDB` 
2. Open terminal > run `mongosh` 

## commands 
1. `show dbs;` - shows all the databses present in the server
2. `use db_name;` - switches to database if exists or creates a new database
3. `db;` - displays current database name
4. `db.createCollection("collection_name");` - creates a collection in the current database
5. `db.insert.collection_name({document ...}, {document ...}, ...);` - used to insert documents into the collection
6. `db.collection_name.updateMany({ filter_criteria }, { $set: { field: value } }, { upsert: true });` - updates value if present else inserts the new document into the collection
7. `db.dropDatabase();` - drops the current database
8. `show collections;` - displays all collection in the current database
9. `db.collection_name.save({_id: ObjectId(), new_data})` -  creates documnet if not present else replaces existing document with new document
10. `db.collection_name.remove({deletion criteria} {justOne: boo;l});` - delete documents from a collection
11. `db.students.update({criteria}, {$unset: {key:field}});` -  remove field form the existing document
12. `db.collection_name.find({find_criteria}, {visibility});` - to find elements based on some predefined criteria
13. `$nin` : neither nor
14. `$in` : either or or
15. `/^letter_starts_with/ - /letter_end_with$/ - /letter_anywhere/` 
16. `$regex`
17. `"fruits.1":"grapes"` : gives all doc at which grapes ia at pos 1 in array or position 2
18. `db.food.find({fruits:{$size:2}});` : gives all fruits whose size 2
19. `[0, 2]` starting from  0 2 values
