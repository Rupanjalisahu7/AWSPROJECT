AWS Project Setup Guide
Explore the essential steps required to set up an AWS project, covering IAM role creation, Lambda function configuration, DynamoDB table establishment, and API Gateway setup.

Step 1: IAM Role Creation
Begin by creating an IAM role in the AWS Management Console. Assign the necessary permissions to the role, ensuring access to the required AWS services for your project.

Role Permissions
To enable Lambda functions and DynamoDB access in this project, create an IAM role with the following permissions:

AWSLambdaBasicExecutionRole: Provides basic execution permissions for Lambda functions.
AWSDynamoDBFullAccess: Grants full access permissions to DynamoDB tables.
Ensure these roles are assigned to Lambda functions and any other resources needing DynamoDB access.

Step 2: Lambda Function Setup
Create a Lambda function using the AWS Lambda service. Configure the function according to project requirements, including triggers, environment variables, and function code. Select the latest version of Python as the runtime and assign an appropriate execution role. After creating the function, upload the zip file containing your code.

Step 3: DynamoDB Table Creation
Create a DynamoDB table in the AWS DynamoDB service. Name the table as specified in your Python code and choose "email" as the partition key. Select default settings for other configurations and create the table to complete the setup.

Step 4: API Gateway Configuration
Set up an API Gateway in the AWS API Gateway service. Define API endpoints, methods, and integrations with Lambda functions or other AWS services.

Create a REST API with both GET and POST methods.
Deploy the API to the "dev" stage and copy the invoke URL provided. Users can submit data via the API, which will be stored in the DynamoDB table.
Example Usage
Users can access the provided API Gateway link to access the login page. After login, users can submit data via the UI, which will be stored in DynamoDB for storage and retrieval.
