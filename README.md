## Library Management System

As a group, we have created a multi-service application that uses Java Programming, Spring Boot, JPA, PostgreSQL and Docker Compose.

This is the Deploy Repository for our group project. There are 4 microservices in our project. 

The GitHub repositories can be viewed below:

* User Service: https://github.com/meeeiiike/user-service 
* Book Service: https://github.com/meeeiiike/book-service
* Loans Service: https://github.com/meeeiiike/loan-service
* Notification Service: https://github.com/meeeiiike/notification-service

## Project Setup

First you need to install Docker Desktop on your computer by following this link to their download page: (Docker Desktop is free) https://www.docker.com/products/docker-desktop/

Docker Desktop does not have to be open for the following steps to work although it will show more details about the microservices.

With that done, you need to open a new Terminal window. You can navigate to it manually or press Win+X then I in Windows, Ctrl+Alt+T in Linux and Command+Space and type Terminal on MacOS.

Run the following command.
```bash
git clone https://github.com/CircuitSculptor/Library-Management-Deploy.git
```
You have now cloned the Deploy Repository.

Next you have to go into the directory where the cloned files are. Run the following command.
```bash
cd Library-Management-Deploy
```
Optionally you can enter `ls` to see all the files within this directory and `cat README.md` to view this in the Terminal.

Now you are one command away from running our project. Run the following command.
```bash
docker compose up --build
```
This command will begin to pull down our project onto your computer and start automatically. It will show the 4 microservices starting up.

## How to use our project

Below are 4 links to each microservice that you have just launched.

* User Service: http://localhost:8080/swagger-ui/index.html 
* Book Service: http://localhost:8081/swagger-ui/index.html 
* Loans Service: http://localhost:8082/swagger-ui/index.html 
* Notification Service: http://localhost:8083/swagger-ui/index.html

You can fill in some details in the User Service or the Book Service.

NOTE: Any long ID values must be removed from the request bodies as ID's are auto incremented by the database

All services are running and you can check all the endpoints with Swagger and use the provided functionality.

It is good practice to always close down any unused projects in Docker. It will free up space and valuable RAM. Run this final command.
```bash
docker compose down -v
```
NOTE: Running `docker compose down -v` will remove all database data.

You may need to open a new Terminal window (with cd) or press Ctrl+C to be able to enter this command.

Alternatively you can stop and delete the project manually from the Docker Desktop app.
___

### Architecture Overview

This project follows a microservices architecture where each microservice has its own database schema and communicates via REST APIs. 

Docker Compose is used to facilitate each microservice startup and networking between all the microservices.

### Project Contributors
* https://github.com/CircuitSculptor
* https://github.com/meeeiiike
* https://github.com/FirstGit178
* https://github.com/KucukBalik
