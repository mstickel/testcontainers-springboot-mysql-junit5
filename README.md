# Testcontainers / MySQL / Spring Boot Example Application

Here is an example of how to use the following technologies to test a database:
* Java 11+
* Maven
* Docker
** Failsafe plugin
* Spring Boot (we use Data JPA, Web, and Test)
* Testcontainers
** MySQL container
* JUnit 5 (Jupiter)

### Prerequisites:
* Java 11 or newer
* Maven
* Docker (Docker for Mac/Windows works if developing on those OSes)

### To run:

`mvn clean integration-test`

### Notes:

I was banging my head against the desk for awhile with this one, getting failures with even the most basic test cases.  I traced the issue to a problem running Spring Boot integration tests using Maven Failsafe Plugin version 3.0.0.M5.  This is why we use version 3.0.0.M4.  See here for more information: https://stackoverflow.com/questions/64272249/spring-boot-integration-test-cant-find-configuration

#### Happy Testing!
