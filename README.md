# AWS Project Setup Guide
Learn how to set up your AWS project with ease. This guide walks you through the essential steps, including IAM role creation, Lambda function setup, DynamoDB table creation, and API Gateway configuration.

 # IAM Role Creation
Create IAM Roles: Begin by creating IAM roles in the AWS Management Console.

Assign Permissions: Assign the necessary permissions to the roles, ensuring access to AWS services required for your project.
   
1.AWSLambdaBasicExecutionRole: Provides basic execution permissions for Lambda functions.

2.AWSDynamoDBFullAccess: Grants full access permissions to DynamoDB tables.

# Lambda Function Setup
Create Lambda Function: Use the AWS Lambda service to create a new Lambda function.

Configuration: Configure the function according to your project's needs, including triggers, environment variables, and function code.

Choose the latest version of Python as the runtime.

Assign an appropriate execution role.

# DynamoDB Table Creation
Create DynamoDB Table: Head to the AWS DynamoDB service to create a new table.

Configuration: Name the table as specified in your Python code and choose "email" as the partition key.

Select default settings for other configurations.

# API Gateway Configuration
Set Up API Gateway: Configure an API Gateway in the AWS API Gateway service.

Define Endpoints: Define API endpoints, methods, and integrations with Lambda functions or other AWS services.

Create a REST API with both GET and POST methods.

Deploy the API to the "dev" stage and copy the provided invoke URL.

Example Usage

Access the provided API Gateway link to access the login page. After logging in, users can submit data via the UI, which will be stored in DynamoDB for storage and retrieval.

