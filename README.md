# AWS-Cloudformation

Welcome to the AWS CloudFormation project for deploying a custom Virtual Private Cloud (VPC) and an EC2 instance. This infrastructure-as-code (IaC) template automates the setup process, streamlining the creation of a scalable and secure environment on Amazon Web Services (AWS).
Overview

## This CloudFormation template enables the creation of a robust infrastructure with the following components:

   1. Custom VPC with defined CIDR block
   2. Public and private subnets across multiple availability zones
   3. Internet Gateway for external connectivity
   4. Route tables for routing within the VPC
   5. Security groups to control inbound and outbound traffic
   6. EC2 instance running a basic web server in a public subnet
   
# Getting Started
## Prerequisites
Before you begin, make sure you have the following:

    AWS Account: Ensure you have an AWS account with the necessary permissions to create resources.
    AWS CLI: Install the AWS Command Line Interface to interact with AWS services.

# Deployment Steps
Use the command below 
1. aws cloudformation create-stack --stack-name YourStackName --template-body file://path/to/your/template.yaml --capabilities CAPABILITY_IAM '

    aws cloudformation: This is the AWS CLI command for interacting with AWS CloudFormation. 

    create-stack: This sub-command is used to create a new CloudFormation stack.

    --stack-name YourStackName: This flag specifies the name you want to give to your CloudFormation stack. Replace YourStackName with the desired name for your stack.

    --template-body file://path/to/your/template.yaml: This flag specifies the location of the CloudFormation template file. Replace path/to/your/template.yaml with the actual path to your CloudFormation template file. Make sure the file is in YAML format.

    --capabilities CAPABILITY_IAM: This flag acknowledges that the stack might create AWS Identity and Access Management (IAM) resources. It's required when your CloudFormation template includes IAM resources.


