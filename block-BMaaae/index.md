writeCode

Write code to:-

- create a database named `sports`. // use sports
- list all databases present in local mongod server. //show dbs
- create 3 collections named `cricket`, `football`, `TT` in sports databse. //db.createCollection('TT')
db.createCollection('cricket')
db.createCollection('football')

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`. //db.football.insertMany([{"name": "neymar", "age": 28, "email": "neymar@gmail.com", "bid_price": "5000000000"},{"name": "messi", "age": 33, "email": "messi@gmail.com", "bid_price": "700000000"}, {"name": "ronaldo", "age": 36, "email": "ronaldo@gmail.com", "bid_price": "4000000000"}])

//db.cricket.insertMany([{"name": "rahul", "age": 24, "email": "rahul@gmail.com", "bid_price": "8000000"}, {"name": "kohli", "age": 30, "email": "kohli@gmail.com", "bid_price": "10000000"}, {"name": "dhoni", "age": 36, "email": "msd@gmail.com", "bid_price": "100000000"}])

//db.TT.insertMany([{"name": "ajay", "age": 20, "email": "ajay@gmail.com", "bid_price": "2000000"},{"name": "ram", "age": 24, "email": "ram@gmail.com", "bid_price": "3000000"},{"name": "chethan", "age": 28, "email": "chethan@gmail.com", "bid_price": "6000000"} ])

- list all collections in sports database. //show collections

- rename `TT` collection to `tennis`. //db.TT.renameCollection("tennis")

- create a capped collection called `khokho` which should have max 3 documents. //db.createCollection('khoko', {capped: true, size: 1024, max: 3})

  Try inserting more than 3 and see what happens? //db.khoko.insertMany([{"name": "neymar", "age": 28, "email": "neymar@gmail.com", "bid_price": "5000000000"}, {"name": "kante", "age": 30, "email": "kante@gmail.com", "bid_price": "9000000000"}, {"name": "ronaldo", "age": 36, "email": "ronaldo@gmail.com", "bid_price": "9000000000"}, {"name": "messi", "age": 35, "email": "messi@gmail.com", "bid_price": "8000000000"}])

- check whether a collection is capped or not? //db.khoko.isCapped()
- drop all documents from `football` collection. //db.football.remove({})
- delete cricket collection completely. //db.cricket.drop();
- delete sports database. //db.dropDatabase()
- check which database you are connected to ? //db
- connect to test database //use test
