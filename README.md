# User Details Application
This is a Spring Boot Application which has basic Operations for a updating a User Database.
To Run this application proceed with the followig steps:
1. Goto Terminal --> To the Directory in which you downloaded this apllication.
2. Run cmd "mvn spring-boot:run"
3. For using Create API use POST methhod & URI: http://localhost:8080/user/create with 
Payload : {
	"id": "12345",
	"fName": "joe",
	"lName": "smith",
	"email": "abc@abc.com",
	"pinCode": 3200,
	"birthDate": "02-Mar-2020",
    "isActive": true
}
4. For using Update API use PUT method & URI: http://localhost:8080/user/update/12345 with 
Payload: {
	"id": "12345",
	"fName": "john",
	"lName": "smith",
	"email": "abc@abc.com",
	"pinCode": 3200,
	"birthDate": "02-Mar-2020",
    "isActive": true
}
5. For using Delete API use DELETE method & URI: http://localhost:8080/user/delete/123456 
6. TO Run Junit uncomment the Class and run it outside the application using mvn surefire:test -DuserControllerTest=UserControllerTest

This is how you can use the basic CUD operations for the User Database.

Features to be developed:
1. Implmenting Read API
2. Proper Logging Configuration for better Debugging purposes.
3. Using Actual DB like Hibernate/SQL.
