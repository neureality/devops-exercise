# devops-exercise

## Introduction

Hello, 
Your assignment is to create an environment that launches two instances in AWS, installs required packages on them and deployes a Kubernetes cluster with the dockers given.

You should be able to test your environment with a free-tier AWS account and recreate this with any other AWS account.

In addition, you shuold create documentation that will allow any user to take the environment and be able to deploy the Kubernetes cluster.

## Tasks

### Terraform
Create terraform scripts to launch two AWS instances, one for the Kubernetes master and one for the worker node.

### Kubernetes
Create Kubernetes configuration with a single namespace and two pods with the docker in 'images' folder on the worker node

### Ansible
Create an ansible playbook to install relevant packages on the AWS instances.

Create an ansible playbook to launch Kubernetes master on the relevnat AWS instance which the configuration to load the pods on the worker node

## Deliverables
A GitHub Pull-Request to **YOUR DUPLICATED REPO**, containing:


The terraform scripts

Kuberenetes configuration for the cluster

Ansible roles which takes care of provisioning both the Kubernetes master and work nodes

Ansible playbook to launch the Kubernetes cluster

README file with description of the code you added and how to use it

