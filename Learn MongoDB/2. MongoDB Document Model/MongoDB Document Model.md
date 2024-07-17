# MongoDB Document Model

  - Easier to plan how application will correspond to data in database
  - Model data in any shape or structure

# MongoDB Document

  - Basic Unit of Data in MongoDB
  - Records in MongoDB Database
  - Data Structure composed of _key : value_ pairs
  - Similar to JSON Objects
  - Field Values may be Numbers, Strings, Booleans, Arrays, Nested Documents, etc.

Example =>

    {
	    title: "Post Title 1",
	    body: "Body of post.",
	    category: "News",
	    likes: 1,
	    tags: ["news", "events"],
	    date: Date()
    }

# Collection

  - Grouping of MongoDB Documents

# MongoDB Database

  - Container for Collections

# Relation between MongoDB Database & Atlas

  - MongoDB Database is at core of Atlas
  - Atlas is Developer Database Platform
  - Additional functionality offered by Atlas like Full Text Search, Data Visualisation, etc. are built on top of data store & cloud-hosted MongoDB Database Deployment
