# devops-exercise

## Introduction

Hello, 

Your assignment is to create an environment that launches an instances in AWS and deploys a simple application written in Python using docker compose.

In order to test your environment you will be given a limited AWS account and user that will be able to load t3.small instances in eu-central-1 (Frankfurt) region.

In addition, you should create documentation that will allow any user to take the code and bring it up in any AWS account.

## Tasks

### Terraform
Create terraform scripts to launch an AWS t3.medium instance (assuming there is a default VPC and an existing key-pair).

The user running the terraform command should provide two variables: AWS region and key-pair name.

### Ansible
Create ansible roles to install the docker compose components on the AWS instance.

### Docker-compose deployment
Create Docker-compose deployment configuration running the application below.

### Application
Create a Python HTTP application which will provide 2 APIs 

API 1: `/reverse`  
The API should receive as string via "in" query parameter using GET HTTP request, and return a response JSON with a field named "result" and its value should be the string provided with the words in reverse order.

For example:
For in value of:
```
The quick brown fox jumps over the lazy dog"
```
Result value should be:
```
dog lazy the over jumps fox brown quick The
```

API 2: `/restore`  
The API will return the last result from API 1.



The application container should be stored on DockerHub.


## Deliverables
A GitHub link to your repositry, containing:

* Application code

* Terraform code

* Ansible roles

* Ansible playbook and inventory to run the roles

* Docker-compose deployment yaml

* README file with instructions on how to use this code and bring up the environment

