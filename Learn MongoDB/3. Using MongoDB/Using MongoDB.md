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

3. `Load Sample DataSet` :-

    - In 'Database Deployments', go to your Cluster
    - Click (...) for more options
    - Click on 'Load Sample Dataset' option from the dropdown
    - A dialog box appears having information about sample dataset created
    - Click on 'Load Sample Dataset' button
    - Wait until the sample dataset is successfully loaded

4. `Install MongoDB Shell (mongosh)` :-

    - Download & Install mongosh in your computer from Official Website

5. `Connect to Database` :-

    - In MongoDB Atlas Dashboard, under 'Databases', click 'Connect' button for your Cluster
    - Choose 'Connect With the MongoDB Shell'
    - Copy your Connection String
    - Example of Connection String =>

          mongosh "mongodb+srv://cluster0.ex4ht.mongodb.net/myFirstDatabase" --apiVersion 1 --username YOUR_USER_NAME
    
    - Paste this in your terminal
    - Hit Enter
    - You will be prompted to enter your Database User Password which you created earlier
    - Enter your Credentials correctly
    - Now, you are connected to Database
