AWS Serverless Visitor Counter Application
Overview
This project deploys a serverless visitor counter application using AWS CloudFormation.

Architecture
API Gateway | Lambda Function | DynamoDB

Components
Amazon API Gateway
AWS Lambda
Amazon DynamoDB
IAM Role
AWS CloudFormation Nested Stacks
CloudFormation Templates
api-gateway.yaml
lambda-function-exe-role.yaml
visitors-table.yaml
main.yaml
Deployment
Validate:

aws cloudformation validate-template
--template-body file://main.yaml

Deploy:

aws cloudformation deploy
--stack-name visitor-counter
--template-file main.yaml
--capabilities CAPABILITY_NAMED_IAM

Learning Outcomes
Infrastructure as Code (IaC)
AWS Lambda
API Gateway Integration
DynamoDB
IAM Roles
CloudFormation Nested Stacks

