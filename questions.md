1. What is responsible for defining the routes of the games resource?

    I think create_router.js(helper) defines the routes of the resource.  Although line 17 of server.js tells createRouter which collections to use and line 18 specifies the first part of the route to use.

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?
    The app is divided into 2 parts: client and server.  I think the client is responsible for the front-end appearance and functionality.  It also sends requests over the the back end via the GamesService functions.  The server is responsible for the database and the routes to manipulate the database.

3. What are the the responsibilities of server.js?
    Server js listens for api calls coming from the client.  It links these to the databse with the routes


4. What are the responsibilities of the gamesRouter?
    gamesRouter appears to link the generic routes with the games collection so that the routes can be used with this collection.


5.  What process does the the client (front-end) use to communicate with the server?
    Not sure what this question is asking for, but I think the client communicates with the server via api requests.

6.  What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs
    The 2nd argument on a fethc metho is an init object used to control the settings.  In the case of the fetch used on GamesService line 10, it specifies the method is post, that the body of the post request should be turned into JSON and the header states that we are using json.

7. Which of the games API routes does the front-end application consume (i.e. make requests to)?
    The front end consumes localhost:5000/api/games

8. What are we using the MongoDB Driver for?
    I'm not sure which part of the code is the driver, but it will be used to connect to the mongoDB database and to access/modify our data
