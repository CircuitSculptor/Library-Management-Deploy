You need Docker Desktop installed first!

then clone this deploy repo (Library-Management-Deploy) and make sure you're in the directory. 
once done you can run "docker compose up --build" which will pull everything you need to get started.

all services should now be running! you can check endpoints with swagger and use the provided funtionality 

http://localhost:8080/swagger-ui/index.html 

http://localhost:8081/swagger-ui/index.html 

http://localhost:8082/swagger-ui/index.html 

http://localhost:8083/swagger-ui/index.html

#NOTE any long id values must be removed from request bodies as id's are auto incremented
