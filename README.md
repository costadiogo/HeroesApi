## Project developed during the Inter java developer bootcamp in partnership with Digital Innovation One

### Used Stacks

* Java 11 
* Spring webflux 
* Spring data
* Dynamodb aws
* Junit
* Sl4j 
* Reactor

### Installing

A step by step that will guide you on how to run the project on your computer.


Clone the project repository:
```
> https://github.com/costadiogo/HeroesApi.git
```
After cloning the project open in an IDE of your choice.

After cloning the project it's time to install DynamoDB you can follow the documentation on this link.
```
> https://docs.aws.amazon.com/pt_br/amazondynamodb/latest/developerguide/DynamoDBLocal.html
``` 
After installing and configuring DynamoDB, type this command below to run the start the local server.
```
> java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
```
Boot the application using Spring Boot.

To check if the table was created in DynamoDB, type the command below:
```
> aws dynamodb list-tables --endpoint-url http://localhost:8000  
```

After all ready Heroes created populated tables you can check the documentation with Swagger in this link below:
``` 
> http://localhost:8080/swagger-ui-heroes-reactive-api.html
```
