# MongoDB mongosh Insert

- 2 Methods to insert Documents via MongoDB mongosh :

  1. insertOne()
  2. insertMany()

# insertOne() Method

Command =>

    db.<collectionName>.insertOne(<object>)

- Inserts single document
- Example =>

      db.posts.insertOne({
        title: "Post Title 1",
        body: "Body of post.",
        category: "News",
        likes: 1,
        tags: ["news", "events"],
        date: Date()
      })

- If the insertion of document into the collection is successful, we get the an output similar to this :

      {
        acknowledged: true,
        insertedId: ObjectId("<objectID>")
      }

# insertMany() Method

Command =>

    db.<collectionName>.insertMany([
      <document1>,
      <document2>,
      <document3>,
      ...
    ])

- Inserts multiple documents at once
- This method expects an array of documents to be passed
- Each document in the array must be separated by comma
- Example =>

      db.posts.insertMany([  
        {
          title: "Post Title 2",
          body: "Body of post.",
          category: "Event",
          likes: 2,
          tags: ["news", "events"],
          date: Date()
        },
        {
          title: "Post Title 3",
          body: "Body of post.",
          category: "Technology",
          likes: 3,
          tags: ["news", "events"],
          date: Date()
        },
        {
          title: "Post Title 4",
          body: "Body of post.",
          category: "Event",
          likes: 4,
          tags: ["news", "events"],
          date: Date()
          }
        ])

- If the insertion of document into the collection is successful, we get the an output similar to this :

      {
        acknowledged: true,
        insertedIds: {
          '0': ObjectId("<objectID>"),
          '1': ObjectId("<objectID>"),
          '2': ObjectId("<objectID>"),
          .....
        }
      }

> [!Note]
> - If you try to insert documents into a collection that does not exist, MongoDB will create the collection automatically
> - This helps avoiding creation of unnecessary collections

> [!Important]
> - Every document in collection must have _id field with a unique value
> - If we don't provide _id, MongoDB will automatically generate it

