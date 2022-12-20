# Automation / Devops Exercise

## Introduction

Hello, 

Your assignment is to create a container that exposes a REST API and a test code that will test the API functionality.

In addition, you should create documentation that will allow any user to take the code, create the container and run the tests.

## Tasks

### Application
Create a Docker container with Python HTTP application which will provide 2 APIs 

API 1: `/reverse`  
The API should receive as string via "in" query parameter using GET HTTP request, and return a response JSON with a field named "result" and its value should be the string provided with the words in reverse order.

For example:
Where in value of:
```
The quick brown fox jumps over the lazy dog"
```
Result value should be:
```
dog lazy the over jumps fox brown quick The
```

API 2: `/restore`  
The API will return the last result from API 1.

### Tests
Create a code in Python using pytest which:
* Starts the application container created above
* Run tests to ensure the API conforms to the Application requirements listed above.
* Shuts down the application container when test is completed or on error.
* Publishes the result as JUnit file.

## Deliverables
A GitHub link to your repositry, containing:

* Application code

* Dockerfile

* Tests written using pytest

* A README file with instructions about this assignment, how to build the container, how to run tests and what should be a successful test result.

