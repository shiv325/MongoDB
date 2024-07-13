# Introduction to MongoDB

  - MongoDB is Document Database
  - Stores data in BSON (JSON type)
  - Can be installed locally or hosted in Cloud

# MongoDB Document

  - Records in MongoDB Database
  - Data Structure composed of _key : value_ pairs
  - Similar to JSON Objects
  - Field Values may be Numbers, Strings, Booleans, Arrays, Nested Documents, etc.

# SQL vs Document Databases

  1. `SQL` :
      - Relational Database
      - Stores related data in separate tables
      - Queried from multiple tables to join data back together

  2. `MongoDB` :
      - Non-Relational Database
      - Stores all related data together in flexible documents
      - Fast data reading
      - Multiple data groups can be created
      - Here, Tables are called `Collections`

# Using MongoDB

1. `Install MongoDB` :-

   Ways to install MongoDB :

   - `Local Database` :
      - Download & Install MongoDB Community Server
      - Allows hosting your own MongoDB server on your hardware
      - Manage, upgrade server and maintain server yourself

   - `Cloud Database` :
      - Use MongoDB Atlas (Cloud Database Platform)
      - Sign up for MongoDB Atlas Account

2. `Create Cluster` :-

    - Set up Free Shared Cluster
    - Choose preferred cloud provider & region
    - Set up user
    - Add your IP Address to list of Allowed IP Addresses
    - Under 'Database Access', create a new user
    - Keep track of username & password
    - Under 'Network Access', add your current IP Address to allow access from your computer

> ___Note*___ : By default, MongoDB Atlas is completely locked down. It has no external access.

3. `Install MongoDB Shell (mongosh)` :-

    - Download & Install mongosh in your computer from Official Website

4. `Connect to Database` :-

    - In MongoDB Atlas Dashboard, under 'Databases', click 'Connect' button for your Cluster
    - Choose 'Connect With the MongoDB Shell'
    - Copy your Connection String
    - Example of Connection String =>

          mongosh "mongodb+srv://cluster0.ex4ht.mongodb.net/myFirstDatabase" --apiVersion 1 --username YOUR_USER_NAME
    
    - Paste this in your terminal.
    - Hit Enter
    - You will be prompted to enter your Database User Password which you created earlier