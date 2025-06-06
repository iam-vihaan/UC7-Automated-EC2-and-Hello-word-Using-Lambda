# UC7-Automated-EC2-and-Hello-word-Using-Lambda

Overview

DevOps Challenge! In this usecase, you will demonstrate your skills in containerization, Infrastructure as Code (IaC), CI/CD, and cloud deployment using AWS services. You will be working with a simple hello word webpage.

Challenge Structure

1. AWS Lambda Container Deployment

Common Requirements

You will be working with the following common elements:

1. Containerization: You need to containerize these microservices using Docker.

2. Infrastructure as Code (Terraform):

o Set up a Terraform project structure supporting multiple environments (dev, staging, prod).

o Provision the following AWS resources:

§ VPC with public and private subnets across two availability zones

§ IAM roles and security groups

§ S3 bucket for Terraform state storage

§ DynamoDB table for state locking

§ (Other resources specific to your chosen track)

3. Terraform State Management:

o Implement remote state storage using S3

o Set up state locking with DynamoDB

o Configure workspace separation for different environments

4. GitHub Actions for IaC:

o Create workflows for:

§ Terraform fmt and validate on all PRs

§ Terraform plan on pull requests

§ Terraform apply on merges to main branch

5. CI/CD: Implement a CI/CD pipeline using GitHub Actions for your application code.

6. Monitoring and Logging: Set up basic monitoring and logging using AWS CloudWatch.


Evaluation Criteria

While specific criteria vary by track, you will generally be evaluated on:

1. Correct implementation of the chosen deployment platform

2. Quality and security of the IaC implementation

3. Effectiveness of the CI/CD pipeline

4. Containerization best practices

5. Monitoring and logging setup

6. Documentation quality

7. Overall architecture and security considerations

8. Proper implementation of Terraform state management and collaboration features

Getting Started

1. Review the common requirements and evaluation criteria.

2. Follow the specific instructions for your chosen track.

3. Use the provided microservices code as a starting point for your application.







AWS Lambda Container Deployment

Objective

Deploy the containerized microservices using AWS Lambda with container images, demonstrating your skills in serverless architecture, containerization, and AWS services.

Technical Requirements

1. Infrastructure as Code (Terraform)

o Provision a VPC with public and private subnets (if needed)

o Set up Lambda functions configured for container image deployment

o Configure necessary IAM roles and security groups

o Set up an ECR repository for your container images

1. Create an API Gateway to trigger your Lambda functions

2. Containerization

o Create a Dockerfile for the microservices, optimized for Lambda

o Build and push the Docker image to ECR

3. Lambda Configuration

o Configure Lambda functions to use container images

o Set up appropriate memory and timeout settings

4. CI/CD (GitHub Actions)

o Implement a workflow for Terraform (lint, plan, apply)

o Create a workflow for building and pushing Docker images

o Implement a workflow for updating Lambda functions

5. Monitoring and Logging

o Set up CloudWatch for Lambda logging and metrics

o Implement X-Ray for distributed tracing

Deliverables

1. GitHub repository containing:

o Terraform code

o Dockerfiles optimized for Lambda

o GitHub Actions workflows

o Application code (provided microservices)

2. Documentation:

o Architecture diagram

o Setup and deployment instructions

o Monitoring and logging overview

Evaluation Criteria

1. Lambda configuration and security

2. API Gateway setup and integration

3. CI/CD pipeline efficiency and reliability

4. IaC quality and modularity

5. Containerization best practices for Lambda

6. Monitoring and logging effectiveness

7. Documentation clarity and completeness


Sample Code/Output:

Print “Hello World”
