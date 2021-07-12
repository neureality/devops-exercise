# devops-exercise

## Introduction

Hello, 
Your assignment is to create an environment that launches two instances in AWS, installs Kubernetes and deployes a cluster with a given image.

You should be able to test your environment with a free-tier AWS account and recreate this with any other AWS account.

In addition, you shuold create documentation that will allow any user to take the environment and be able to deploy the Kubernetes cluster.

## Tasks

### Terraform
Create terraform scripts to launch two AWS instances (assuming there is a default VPC so you don't need to specific anything except for the region), one for the Kubernetes master and one for the worker node.

### Ansible
Create an ansible playbooks to install Kubernetes on the AWS instances.

### Kubernetes
Create Kubernetes deployment with three replicas running [this image](https://hub.docker.com/r/gairadzi/webserver)

## Deliverables
A GitHub Pull-Request to **YOUR DUPLICATED REPO**, containing:


* The terraform code

* Ansible roles which takes care of provisioning both the Kubernetes master and work nodes

* Ansible playbook to install the Kubernetes cluster

* Kuberenetes deplyoment yaml

* README file with instructions on how use this code and deploy the Kubernetes cluster

