# Homework: Full Stack Games Hub App

### Learning Objectives

- Understand the relationship between client, server and database
- Be able to navigate a codebase that you haven't written

## Brief

Your boss has asked to you look over the codebase of a full-stack JavaScript application. The front-end is written in JavaScript using Vue, the back-end uses an Express server and a MongoDB database. Your task is to make yourself familiar with the codebase.

The application includes a README.md with instructions on running the application.

![Overview of the tech stack and tooling with commands](images/tech_stack_with_commands.png)

*Overview of the tech stack and tooling with commands*

## MVP

### Task

Draw a diagram showing the dataflow through the application starting with a form submission, ending with the re-rendering of the page. This will involve a multi-direction data-flow with the client posting data to the server and the server sending data back to the client with the response. Detail the client, server and database in the diagram and include the names of the files involved in the process.

### Questions

1. What is responsible for defining the routes of the `games` resource?

The Express server.

2. What do you notice about the folder structure?  Whats the client responsible for? Whats the server responsible for?

The front-end (client) is written in JavaScript using Vue. The client posts data to the server and the server sends data back to the client with the response.

3. What are the the responsibilities of server.js?

It stores data that it is going to send back to the client if a request is made.

4. What are the responsibilities of the `gamesRouter`?

The router handles more than one source and the Restful routes related to the sources.

5. What process does the the client (front-end) use to communicate with the server?

It makes request to the server in order to get data back.

6. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs

An init object. It is used to get games hub data back.

7. Which of the games API routes does the front-end application consume (i.e. make requests to)?

The Index/Get request.

8. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?

MongoDB database running allow us to connect and interact with the MongoDB database.

## Extension

Why do we need to use [`ObjectId`](https://mongodb.github.io/node-mongodb-native/api-bson-generated/objectid.html) from the MongoDB driver?

Because it helps to identify the unique id of the object we are targeting.

Add to your diagram the dataflow for removing a game.
