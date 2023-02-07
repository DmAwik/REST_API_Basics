# REST_API_Basics

Task: https://github.com/mjc-school/MJC-School/blob/027d2511f5ea880ed0507f1e5cb3b097bf253885/stage%20%233/java/module%20%232.%20REST%20API%20Basics/rest_api_basics_task.md

Business requirements:

Develop web service for Gift Certificates system with the following entities (many-to-many):
![image](https://user-images.githubusercontent.com/63674815/214316247-57054ec7-a3d5-4615-bd5a-68a8877bd77c.png)

The system should expose REST APIs to perform the following operations:


CRUD operations for GiftCertificate. If new tags are passed during creation/modification – they should be created in the DB. For update operation - update only fields, that pass in request, others should not be updated. Batch insert is out of scope.

CRD operations for Tag.

Get certificates with tags (all params are optional and can be used in conjunction):

by tag name (ONE tag)

search by part of name/description (can be implemented, using DB function call)

sort by date or by name ASC/DESC (extra task: implement ability to apply both sort type at the same time).


Application requirements:


JDK version: 8 – use Streams, java.time.*, etc. where it is possible. (the JDK version can be increased in agreement with the mentor/group coordinator/run coordinator)

Application packages root: com.epam.esm

Any widely-used connection pool could be used.

JDBC / Spring JDBC Template should be used for data access.

Use transactions where it’s necessary.

Java Code Convention is mandatory (exception: margin size – 120 chars).

Build tool: Maven/Gradle, latest version. Multi-module project.

Web server: Apache Tomcat/Jetty.


Application container: Spring IoC. Spring Framework, the latest version.

Database: PostgreSQL/MySQL, latest version.

Testing: JUnit 5.+, Mockito.


Service layer should be covered with unit tests not less than 80%.
