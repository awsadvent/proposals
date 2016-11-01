## Making AWS instances automagically register with Chef	
* Getting instances to automatically register & deregister themselves in Chef, specifically in autoscaling groups

## Cost Control in AWS	
* AWS is a fantastic resource right up until the point where your CFO reverts to his or her first language: loud screaming. In this entertaining post, X discusses different methods of controlling spend inside of AWS, how to forecast more accurately, and at what points it makes sense to consider AWS alternatives (spoiler: it's a lot larger scale than you think!). 

## Modular & Programmatic EC2 Bootstraping with cfn-init & SparkleFormation	

* Description of modular patterns for using AWS' cfn-init to bootstrap EC2 instances provisioned with Cloudformation and SparkleFormation. 

Key points: 
* Where provisioning ends & Configuration Management starts
* Planning, Coding, and Distributing Modular cfn-init config sets with SparkleFormation
* The benefits of using a programmatic approach to provisioning in AWS"

## Docker on AWS using ECS / ECR	
* Developing Web applications using Java and using CI/CD + ECR + ECS to deliver them in an automated manner using CFn and Codeship

## Are you getting the most out of IAM?	

* IAM basics
* Neat things to do with IAM including identity federation, cross-account access, per-oauth-user s3 bucket path permissions.

## Session Management on AWS	
* What is session management
* Options  in AWS for session management

## Just add Code: Repeatable Infrastructure with Terraform Modules	

* Advanced Terraform topics will be covered in an AWS context, with example Terraform modules provided for VPC, network, and auto-scaling configuration with ALB. An emphasis will be placed on the use of a small subset of repeatable code to configure an EC2 Auto-Scaling group by just supplying an AMI, service port, and network details.

## Cost Control: Beyond Reserved Instances	

* There are a variety of tools and SaaS offerings to tell you how to cut AWS costs-- but they attempt to bring a one size fits all solution to a complex problem. This entertaining post covers a few alternative solutions to maintaining control over what you're spending that go beyond buying a pile of reserved instances. Cake will also be served.

## IAM Policies, Roles and Profiles and how to keep secrets away from your instances.	

* IAM instance roles/profiles and how to use them in place of storing keys directly on your instances. 
* What policies/roles/profiles are (including the difference between roles/profiles when working with the api); 
* Work through an example of setting up access using IAM and terraform, accessing your credentials (most apps are magic, but you can curl the api to get them); 
* explain some situations where this is useful (grafana cloudfront access, storing secrets in s3 using citadel, managing EBS volumes from inside the instance).

## Serverless everything: One-click serverless deployment pipeline for a serverless app 	

* build a deploy pipeline for a sample serverless web app consisting of only AWS components (except for Github). 
* codified and automated and can be provisioned with a one-click CloudFormation template which bootstraps everything. 
* use Lambda for the build steps, and it will utilize the Serverless framework to deploy the actual app.

## Getting started with AWS CodeDeploy	

* monitoring, rollback, on-premise support and improved integration with CodePipeline. We use it deploy our Ansible code so it configures the whole instances (+ deploys our updated code).

## Building custom AMIs with packer	
* Why custom AMIs and how to build them. What are the options somebody can choose in regards of different builders and provisioner during the build process.

## Exploring Concurrency in AWS & Python	
* Discuss a simple problem of multi file S3 transfers 
* Present a pure python concurrency approach to solve it 
* Present a hybrid AWS & Python concurrency approach for solving it

## Getting rid of access keys with federated logon and STS	

* One of the largest attack surfaces of an AWS account is the long-lived access keys attached to IAM users. If a key pair is accidentally pushed to a public source control repo, your account will be compromised in a matter of minutes, putting your private data AND you credit card at risk. 
* Organizations using directory services like LDAP or Google Apps can use federated logon to the management console via SAML, Amazon Directories, or custom signin URLs. 
* An additional benefit to federated logon is the ability to use STS to generate short-lived access keys that users can use to perform automation, similar to instance profiles in EC2/etc."

## Securely managing multiple AWS accounts without going crazy	
* Multi-accounts is becoming more and more common and there is a lack of documentation on how to do it securely, using IAM. This article will provide a template for centralized management of multiple AWS accounts, without resorting to external SSO.

## server-free pubsub (and nearly code-free)
* apigateway + built in AWS services can get you going with little code and zero servers, total pay as you go. 
* does it scale horizontally? guess what it doesn't matter you don't have to scale it
* using bleeding edge technologies removes some operational burden because nobody else understands more about what you're doing than you do