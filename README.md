# devops-exercise

## Introduction

Hello, 
Your assignment is to create an environment that launches two instances in AWS, installs Kubernetes and deployes an application.

You should be able to test your environment with a free-tier AWS account and recreate this with any other AWS account.

In addition, you shuold create documentation that will allow any user to take the code and bring it up in any AWS account.

## Tasks

### Terraform
Create terraform scripts to launch two AWS instances (assuming there is a default VPC and an existing key-pair), one for the Kubernetes master and one for the worker node.

The user running the terraform command should provide two variables, AWS region and key-pair name.

### Ansible
Create ansible roles to install the Kubernetes components on the AWS instances.

### Application
Create Kubernetes deployment configuration with three replicas running [this image](https://hub.docker.com/r/gairadzi/webserver).

## Deliverables
Please make sure you duplicate the repo and **do not fork it** ([duplicating-a-repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/duplicating-a-repository)).

A GitHub Pull-Request to **YOUR DUPLICATED REPO**, containing:


* The terraform code

* Ansible roles for Kubernetes master and work nodes

* Ansible playbook and inventory to run the roles

* Kuberenetes deplyoment yaml

* README file with instructions on how use this code and bring up the environment

