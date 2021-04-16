# Checkpoint 0

Link to the RCOS blog with my post:
https://rcos.io/projects/mackqian/ossminecraftmod/blog

# Checkpoint 1

## Terminal output
![text](https://i.gyazo.com/40a3b909681fb135890fd764bd0bffbf.png)

# Checkpoint 2

## createCollection message
![text](https://i.gyazo.com/b0adced48890b26ec788b4bf4664b5b6.png)

# Checkpoint 3

## Insert and update
```
db.definitions.insert({word: "DogeCoin", definition: "priceisaquarter"})
db.definitions.update({"word":"All-nighter"},{$set:{"definition":"What I am doing tonight"}})
```

## Finding the two words
![text](https://i.gyazo.com/3218aa3a07191e552823be42040a708f.png)

## Git Diff
Since changing the data resulted in a lot of changes happening to the definitions file, I have used `grep` to show only the changes from my insert/update.
![text](https://i.gyazo.com/98447186d944e30692bd093883b7fd44.png)

# Checkpoint 4

## Python code
```python
import pymongo
from pymongo import MongoClient
import pprint
from bson.objectid import ObjectId

# Fetching all records
print('Fetching all records')

client = MongoClient()
database = client.mongo_db_lab
definitions = database.definitions
for definition in definitions.find():
	pprint.pprint(definition)

# Fetching one record
print('\nFetching one record')
pprint.pprint(definitions.find_one())

# Fetching a specific record
print('\nFetching All-nighter')
pprint.pprint(definitions.find_one({"word":"All-nighter"}))

# Fetch by ID
print('\nFetching an object by ID')
pprint.pprint(definitions.find_one({'_id': ObjectId('56fe9e22bad6b23cde07b8ca')}))

# Inserting a new word
print('\nInserting Doge')
definitions.insert({"word": "Doge", "definition": "A very kind animal. Man's best friend."})
pprint.pprint(definitions.find_one({"word":"Doge"}))

```

## Output
![text](https://i.gyazo.com/5ff4268eeed76182bd3268b184d3f2f3.png)


# Checkpoint 5
