# Connecting to MongoDB Database

- MongoDB Connection String allows us to connect to Cluster & work with data
- It describes host to be used & options to connect to MongoDB Database
- Connection String can be used to connect from Mongo Shell, MongoDB Compass, or any other application
- MongoDB provides 2 formats for Connection String :-
    - `Standard Format` :
        - Used to connect standalone clusters, replica sets or shared clusters

    - `DNS Seed List Format` :
        - Allows us to provide DNS Server List to our Connection Stream
        - Gives more flexibility of deployment
        - Provides ability to change servers in rotation without reconfiguring clients

> ___Note*___ : Connection String from MongoDB Atlas Dashboard uses DNS Seed List Entry, which has list of hosts behind it that we can connect to.

# Locate Connection String

- Go to 'Database Deployments' Page
- Click 'Connect' button for desired cluster
- A Modal Box appears giving options to connect to the required database via :
    - MongoDB Shell
    - Application
    - MongoDB Compass
- All these options will provide similar Connection Strings
- Choose 'Connect to Your Application' option
- Another Modal Box appears having the Connection String
- The Connection String will look similar to the below one :

      mongodb+srv://<username>:<password>@<clusterName>.usqsf.mongodb.net/?retryWrites=true&w=majority

# Breakdown of Connection String

    mongodb+srv://<username>:<password>@<host>[:port]/?<options>

- `mongodb` : Required Prefix identifying as MongoDB Connection String
- `+srv` : SRV Edition automatically sets TLS Security option to True & tells MongoDB to use DNS Seed List
- `<username>` : Username created for database in Atlas Dashboard
- `<password>` : Password created for database in Atlas Dashboard
- `<host>` : Host where Database instance is running
- `[:port]` : Optional Port Number to database
- `<options>` : Conditions to be included like Connection Timeout, TLS & SSL, Connection Pooling, Read & Write Concerns, etc.
> ___Note*___ : If Port Number is not specified, MongoDB will default to port 27017
