# Viewing Database

- Using Connection String provided from MongoDB Atlas Dashboard will get you connected to your database
- After connecting to database using mongosh, you can view your database by the following command :

      db

# Show All Databases

- To see all available databases, type this command :

      show dbs

> ___Note*___ : Empty Database is non-existant. A Database is not actually created until it gets some content.

# Change or Create Database

- To change or create database, type this command :

      use <databaseName>

- If the specified database exists already, current database will be changed; otherwise it will be created
