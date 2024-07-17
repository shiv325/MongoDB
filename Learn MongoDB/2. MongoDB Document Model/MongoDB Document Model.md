# MongoDB Document Model

  - Easier to plan how application will correspond to data in database
  - Model data in any shape or structure

# MongoDB Document

  - Basic Unit of Data in MongoDB
  - Records in MongoDB Database
  - Data Structure composed of _key : value_ pairs
  - Similar to JSON Objects
  - Field Values may be Numbers, Strings, Booleans, Arrays, Nested Documents, etc.
  - Displayed in JSON
  - Stored in BSON (Binary JSON)

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

# BSON (Binary JSON)

  - Adds support for datatypes unavailable in JSON

# DataTypes in MongoDB

  - Strings
  - Objects
  - Array
  - Boolean
  - Null
  - Dates
  - Numbers
  - ObjectID

and many more!

# ObjectID

  - Special datatype used to create unique identifiers
  - Every document needs an __id_ field
  - Acts as Primary Key
  - MongoDB automatically generates an ObjectId for _id field if inserted document doesn't include it

# Schema Model & Polymorphism

  - By default, MongoDB supports flexible Schema Model & Polymorphic Data
  - Allows to store documents with different structures in same collection together
  - Documents may contain different fields
  - Fields may contain different datatypes
  - Flexible Schema helps to iterate quickly & evolve
  - Allows updation of classes to include new fields
  - Allows insertion of documents with new schema
  - To have more control over structure & content of database, we can add optional schema validation rules to set constraints on structure of documents

# Document Structure

Syntax =>

    {
	"key": value,
	"key": value,
 	"key" : value
    }

Example =>

    {
	"_id": 1,
	"name": "AC3 Phone",
	"colors" : ["black", "silver"],
	"price" : 200,
	"available" : true
    }
