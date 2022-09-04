# devops-exercise

## Introduction

Hello, 

Your assignment is to create an environment that launches two instances in AWS, installs Kubernetes and deploys a simple application written in Python.

In order to test your environment you will be given a limited AWS account and user that will be able to load t3.small instances in eu-central-1 (Frankfurt) region.

In addition, you should create documentation that will allow any user to take the code and bring it up in any AWS account.

## Tasks

### Terraform
Create terraform scripts to launch two AWS t3.medium instances (assuming there is a default VPC and an existing key-pair), one for the Kubernetes master and one for the worker node.

The user running the terraform command should provide two variables: AWS region and key-pair name.

### Ansible
Create ansible roles to install the Kubernetes components on the AWS instances.

### Kubernetes deployment
Create Kubernetes deployment configuration with three replicas running the application below.

### Application
Create a Python HTTP application based on Flask (https://palletsprojects.com/p/flask/) which will provide a single API on the URL: `/hello`.
The API reponse will return `Hello world!` when called.
The application container should be stored on DockerHub.


## Deliverables
A GitHub link to your repositry, containing:

* The terraform code

* Ansible roles for Kubernetes master and work nodes

* Ansible playbook and inventory to run the roles

* Kuberenetes deployment yaml

* README file with instructions on how to use this code and bring up the environment

