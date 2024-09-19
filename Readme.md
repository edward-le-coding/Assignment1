# Assignment 1 - A Simple Containerized Web App

This web app supports the following commands:

1. curl localhost:8080/foo
* The response will be "bar"

2. curl -H "Accept: application/json" -H "Content-Type: application/json" -X POST --data "{\"name\": \"Prabh\"}" localhost:8080/hello  
* The response will be "Hello {name}" {name} comes from the JSON object submitted to the server

3. curl localhost:8080/kill
* This will kill the server.

The docker image can be created by running the following command:
* docker build -t assignment1-edward-le .

The docker image can be run by using the following command:
* docker run -it -p 8080:8080 assignment1-edward-le
