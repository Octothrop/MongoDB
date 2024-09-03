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