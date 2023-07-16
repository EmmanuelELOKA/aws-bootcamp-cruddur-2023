# Week 0 — Billing and Architecture

## REQUIRED ASSIGNMENTS

## Recreate Conceptual Diagram in Lucid Charts or on a Napkin

Below is both a lucid chart concept including a napkin conceptual diagram

![cruddur-app-concept(modified)](https://user-images.githubusercontent.com/85324899/218800885-2f19ae23-23f3-4e17-b236-98e47e85c9ef.jpeg)

![Cruddur App - Napkin (Modified)](https://user-images.githubusercontent.com/85324899/218800602-d6e23de3-1c2d-4e30-9b51-07e240c07eee.jpg)


[Lucid Chart Link](https://lucid.app/lucidchart/66afba8e-48af-48d3-a5d9-5e7a0d01060b/edit?viewport_loc=-1465%2C-1030%2C5029%2C2760%2CTkZwZafFC.xz&invitationId=inv_c69171d5-6ce4-4aaf-a868-cba75b27c4e7) 

## Recreate Logical Architectual Diagram in Lucid Charts 

![Cruddur App Revised](https://user-images.githubusercontent.com/85324899/219288667-fe23317f-13d8-43fe-854b-caa07d284c13.jpeg)


[Lucid Chart Link](https://lucid.app/lucidchart/66afba8e-48af-48d3-a5d9-5e7a0d01060b/edit?viewport_loc=-623%2C-390%2C3025%2C1660%2Cr1Xw4p3k9qia&invitationId=inv_c69171d5-6ce4-4aaf-a868-cba75b27c4e7)


## Create an Admin User

User "NGOMBE" was created in IAM with Administrator Access

<img width="1685" alt="iam-user" src="https://user-images.githubusercontent.com/85324899/218663987-ce2a8185-89ad-4d85-8ba8-97c7d6292789.png">


## Use CloudShell 

Cloud Shell was used to verify caller identity and list s3 buckets

<img width="1685" alt="cloudshell" src="https://user-images.githubusercontent.com/85324899/218664183-ea05d673-91bc-4ac5-9598-ed9bdafa205c.png">


## Generate AWS Credentials

AWS Credentials was generated for User "NGOMBE"

<img width="1685" alt="credentials " src="https://user-images.githubusercontent.com/85324899/218664570-f1e7c05f-c9cc-4e58-b2f3-4405ddcdc99e.png">


## Installed AWS CLI

Installed AWS CLI and Modified `.gitpod.yml` file

<img width="1685" alt="aws-cli" src="https://user-images.githubusercontent.com/85324899/218664789-2bcccf2e-8bc9-4221-91cb-2b11b9fb296c.png">


## Create a Billing Alarm

Created a billing alarm using AWS CLI and modifying the `alarm-config.json` file

<img width="1685" alt="billing-alarm" src="https://user-images.githubusercontent.com/85324899/218664988-160fbcea-5ac7-4f53-bc17-7b9e6737ab53.png">


## Create a Budget

Created three budgets. Two from the concole and 1 with the AWS CLI after modyfying the `budget.json` file

<img width="1685" alt="budget1" src="https://user-images.githubusercontent.com/85324899/218662738-a0407928-9ebc-42e1-b14b-a5917ba9656d.png">


<img width="1685" alt="budget2" src="https://user-images.githubusercontent.com/85324899/218663088-e4bc0a85-ae3c-4eee-9936-090d9aab660a.png">


<img width="1685" alt="budget3" src="https://user-images.githubusercontent.com/85324899/218663230-810f7579-c6bd-4a85-897a-1798bb33a703.png">


## STRETCHED ASSIGNMENTS

## Set MFA on my Root Account

<img width="1684" alt="MFA" src="https://user-images.githubusercontent.com/85324899/219277165-dc726c39-4a18-4a45-afd8-4702f70b5d31.png">


## Created an architectural diagram of the CI/CD logical pipeline in Lucid Charts

I added a simple CI/CD pipeline so that any changes to the application code will be automated. It starts with the developers commiting their code on Github which will be the SCM, and then that will trigger the Code Pipeline to start the automation. Code Build will then build the application including the new changes and Code Deploy will deploy to the environment. Amazon ECR will be used to store the artifact in this use case. Services and tools used will include:

Docker is one of the services that will be used. It is a platform that lets you build, test, and deliver applications in packages called containers.

Git which is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among developers, but it can be used to track changes in any set of files. 

AWS CodeBuild which is a fully managed build service that helps you compile source code, run unit tests, and produce artifacts that are ready to deploy. AWS CodeBuild scales continuously and processes multiple builds concurrently, so your builds are not left in the queue.

AWS CodePipeline which helps you quickly model and configure the different stages of a software release and automate the steps required to release software changes continuously. In this case, AWS CodePipeline with GitHub.

Amazon Elastic Container Registry (Amazon ECR) is a fully managed registry that makes it easy for developers to store, manage, and deploy Docker container images. Amazon ECR is integrated with Amazon ECS to simplify your development-to-production workflow. 

Amazon Elastic Container Service (Amazon ECS) is a highly scalable, high-performance container orchestration service that supports Docker containers and allows you to easily run and scale containerized applications on AWS. 

![CI_CD Pipeline Cruddur New](https://user-images.githubusercontent.com/85324899/219515285-70d1d7e7-8414-459c-b99e-8ce7cb1bb2cc.jpeg)

[Lucid Chart Link](https://lucid.app/lucidchart/66afba8e-48af-48d3-a5d9-5e7a0d01060b/edit?viewport_loc=-1307%2C-560%2C4154%2C2280%2CakExEEdSWn.z&invitationId=inv_c69171d5-6ce4-4aaf-a868-cba75b27c4e7) 


## Used EventBridge to hookup Health Dashboard to SNS for a notification when there is a service health issue

<img width="1684" alt="Event Bridge" src="https://user-images.githubusercontent.com/85324899/219277373-7a3b7dbd-9946-44a1-9125-085a0a51daa3.png">


## Opened a support ticket and requested a service limit for Elastic IP’s

<img width="1684" alt="Support Ticket" src="https://user-images.githubusercontent.com/85324899/219277447-0d4ebafe-fd45-4b38-a8ab-7cce62675304.png">


## Reviewed  the questions of each pillar in the Well Architected Tool

<img width="1684" alt="WAR" src="https://user-images.githubusercontent.com/85324899/219277505-d0b0d34f-01cb-424a-a9d8-44fe011cb56c.png">


## Researched on the technical and service limits of specific services

<img width="1684" alt="Technical   Service Limits1" src="https://user-images.githubusercontent.com/85324899/219277747-c04e6b51-a0ef-4a90-8114-84b5e688499c.png">

<img width="1684" alt="Technical   Service Limits2" src="https://user-images.githubusercontent.com/85324899/219277758-2a1f6da3-55fe-478b-9020-8cf2808f0e2b.png">

[Reference](https://docs.aws.amazon.com/general/latest/gr/ec2-service.html)



