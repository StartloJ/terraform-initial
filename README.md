# terraform-initial template

Repo to provide fast tracked template for initial Terrraform projects with practical structure.

## Prerequisites

1. pre-commit; you can install [here](https://pre-commit.com/#installation).
2. terraform-cli; you can install [here](https://developer.hashicorp.com/terraform/downloads).

## Folder structure

You can follow up this article to create practics the Terraform development.

1. `components`;  

    This folder is provide reusable module or component of cloud resources  
    that you plan to create group of resources. In example, you can create  
    folder named **network** and develop the terraform file provide as VPC, Subnet, Routing rules, Firewall rules, and others.

2. `deployments`;

    This folder is provide separate environment value files. Therefore, you  
    can create file called `*.tfvars` to create a resource from module in `components` with specific information in each workspace or environment.  
    In example, you can create var file in `dev/network.tfvars` to create  
    the Network resources in **Dev** environment with some specific configurations.

3. Other folder;

    If you need to custom workflow that can't provide in the previous folders,  
    you would to create a custom folder to served your goals.

## Extend development process

You can improvement your development process with helper tools or platform.  
I was provide some practics that I used.

1. `Pre-commit`; I use to ensure source code before push them to Git server.
2. `Task`; I use to automate some workflows like `Make`.

## Contributes

You can help me to improve practical in Infra as Code development with  
create `Issue` or `PR` to this repo. I hope to learn a new practics together.
