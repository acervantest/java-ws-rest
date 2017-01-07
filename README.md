#Spring-REST#

##RESTful web service using Spring##

This project shows a RESTful web service using Spring. It demonstrates the GET, POST, PUT, and DELETE operations.

#### Prerequisites

- Java 7
- Maven 3

###tools and technologies###

* JDK 1.7
* Spring 3.2.0.RELEASE
* jackson-mapper-asl 1.9.13
* jaxb-api 3.0.3
* Tomcat 7.0
* Maven
* Eclipse 

### Build and run
#### Configurations

Open the `properties` of the project and set your own Targeted Runtime (server).

#### From terminal

Go on the project's root folder, then type:

    $ mvn tomcat:run

#### From Eclipse (Spring Tool Suite)

Import as *Existing Maven Project* and run it on *Server*.

### Run

- Run the application and go on http://localhost:8080/restservice/services/
- Use the following urls to invoke interface methods using a testing tool:
  
    * GET operation, so that you are allowed to see all objects in a list, try to go:                  `http://localhost:8080/restservice/services/studentService/student`, you will see all students, by default there is only one.
    
    * GET operation, so that you are allowed to see an object from the list, try to go:                  `http://localhost:8080/restservice/services/studentService/student/111`, where 111 es el id for the default student.
    
    * POST operation, so that you are allowed to add an object to the list, try to go:                  `http://localhost:8080/restservice/services/studentService/student`, adding a Json with the following properties:
{
	"enrollmentId" : 0 ,
	"name" : " [ name ] ” ,
	"lastname" : “ [ lastname ] ”
}
* PUT operation, so that you are allowed to edit an object from the list, try to go:                  `http://localhost:8080/restservice/services/studentService/student`, adding a Json with the following properties:
{
	"enrollmentId" : [ id ] ,
	"name" : " [ name ] ” ,
	"lastname" : “ [ lastname ] ”
}

 * DELETE operation, so that you are allowed to delete an object from the list, try to go:                  `http://localhost:8080/restservice/services/studentService/student/{id}`, where {id} es el id for the student to delete.
    
     
    
    
   
    
