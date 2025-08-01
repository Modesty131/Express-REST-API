# Express-REST-API APP

In this project, I developed a functional Express REST API App that is functional and renders the message "Hello World!". 

This project implements the following componenets:

Set up a basic Express app with middleware

Define a root route (/) returning “Hello, World!”

Implement full CRUD operations on an in-memory items store

Handle validation errors, missing routes, and server errors

Test the API via Postman or curl

Examples request and expected responses includes the following:

Root Route
Request GET http://localhost:3000/

Response Status: 200 Body: Hello, World!

Create an Item
Request POST http://localhost:3000/items Headers: Content-Type: application/json Body:
{
  "name": "Sample Item",
  "description": "This is a test item."
}

Response Status: 201 Body:
{
  "id": 1,
  "name": "Sample Item",
  "description": "This is a test item."
}

Retrieve All Items
Request GET http://localhost:3000/items
[
  {
    "id": 1,
    "name": "Sample Item",
    "description": "This is a test item."
  }
]

Retrieve One Item
Request GET http://localhost:3000/items/1

Response Status: 200 Body:
{
  "id": 1,
  "name": "Sample Item",
  "description": "This is a test item."
}

Update an Item
Request PUT http://localhost:3000/items/1 Headers: Content-Type: application/json Body:
{
  "id": 1,
  "name": "Updated Item",
  "description": "Updated description."
}

Delete an Item
Request DELETE http://localhost:3000/items/1

Response Status: 204 Body: (no content)

Suggestions for Further development
Use environment variables for configuration (e.g., PORT, database URLs).

Add a process manager (PM2) or containerize the app with Docker for automated restarts and load balancing.

Replace the in-memory store with a persistent database (MongoDB, PostgreSQL) for real data durability.

Implement request rate limiting, logging, and security middleware (Helmet, CORS).

Thank you



Response Status: 200 Body:
