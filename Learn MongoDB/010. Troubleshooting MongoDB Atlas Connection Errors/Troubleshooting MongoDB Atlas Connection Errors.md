# Troubleshooting MongoDB Atlas Connection Errors

- 2 Most Common Connection Errors :
    - `Network Access Error`
    - `User Authentication Error`
- Most Connection Issues stem from barriers put up by MongoDB to secure data

# Resolving Network Access Error

- Use Connection String in terminal to connect to Atlas Cluster
- If Error named 'MongoServerSelectionError' occurs, it means that MongoDB refuses the connection
- Reason for this error is that the IP Address has not been allowed to connect
- In Atlas Dashboard, go to 'Network Access' Section under 'Security' on left-hand menu
- Click 'Add IP Address' button
- A Modal Box appears to add IP Address allowed to access MongoDB
- Click on 'Add Current IP Address' button
- Your current IP Address will be added to Access List Entry
- Enable Toggle Switch below if this is a temporary IP Address
- Click 'Confirm' button to add your IP Address
- It may take some time to update the allowed IP Addresses List
- Then, use the updated Connection String to connect to Atlas Cluster

# Resolving User Authentication Error

- Use Connection String in terminal to connect to Atlas Cluster
- If Error named 'MongoServerError: bad auth : Authentication failed' occurs, it means that password has not been provided in the Connection String yet
- Update Connection String by replacing the <password> with your appropriate password
- Now use the updated Connection String to connect to Atlas Cluster
