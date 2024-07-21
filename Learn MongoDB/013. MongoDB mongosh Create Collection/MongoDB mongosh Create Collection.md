# MongoDB mongosh Create Collection

2 Ways to create Collection :

1. `Using createCollection() Database Method` :

       db.createCollection("<collectionName>")

2. `Create Collection during insert() process` :

       db.<collectionName>.insertOne(<object>)

> ___Note*___ : Here, <object> is a valid JavaScript object containing post data 
