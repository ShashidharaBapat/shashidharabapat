# Spring boot RESTful API message scheduler

A Spring boot RESTful API that schedules messages to be printed in the console.
I used https://start.spring.io/ to start the project.

## Prerequisites

- Install Eclipse with Spring Tools 4
- To test the API, you can install SoapUI (https://www.soapui.org/downloads/soapui.html)

I used awaitility (https://github.com/awaitility/awaitility) to write a test case.
All the rest are spring boot and its libraries.

## Install

### Import the project in Eclipse 

Import the Git project: https://github.com/ShashidharaBapat/shashidharabapat.git
 
## Run Spring Boot App

Right-click on the project -> Run As -> Spring Boot App 

## Test the API

Send HTTP Post request to /api/v1/messages/message with the following Json structure :

{"hour":H,"minute":M,"second":S, "message":"MSG"}

With 
- H = hour between 0 and 23 (one-digit number if < 10)
- M = Minute between 0 and 59 (one-digit number if < 10)
- S = Second between 0 and 59 (one-digit number if < 10)
- MSG = message to be scheduled (not empty)

## Run JUnit tests

- Run src/test/java/com.challenge.scheduler.UserMessageIntegrationTest with ** Junit test 4 **
- For more informations about the test cases, check the comments.

## Author

* **Shashidhara Bapat** - *Initial work* - (https://github.com/ShashidharaBapat/shashidharabapat.git)
"# shashidharabapat" 
