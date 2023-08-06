# WildRydes Serverless Web Application
This repository contains the code and configuration files for the WildRydes serverless web application, which enables users to request unicorn rides from the Wild Rydes fleet. The application is built using various AWS services including AWS Lambda, Amazon API Gateway, AWS Amplify, Amazon DynamoDB, and Amazon Cognito.

## Table of Contents
- Overview
- Module 1: Static Web Hosting with Continuous Deployment
- Module 2: User Management
- Module 3: Serverless Service Backend
- Module 4: Deploy a RESTful API

## Overview
The WildRydes web application allows users to request unicorn rides from a fleet of mythical creatures. The application consists of a static web interface hosted using AWS Amplify, user authentication and management using Amazon Cognito, a serverless backend using AWS Lambda and Amazon DynamoDB, and a RESTful API exposed through Amazon API Gateway.

## Application architecture & Features
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/1400aa17-726b-4eb4-9392-53b30e2e9c7b)

- Static web resources (HTML, CSS, JavaScript) are hosted using AWS Amplify.
- User authentication and management are handled by Amazon Cognito.
- The backend service uses AWS Lambda and Amazon DynamoDB to process ride requests.
- The API Gateway exposes a RESTful API for handling ride requests from the web application.

## Module 1: Static Web Hosting with Continuous Deployment
In this module, we configure AWS Amplify to host the static resources for the web application and set up continuous deployment for updates.
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/e753dd92-a173-4bb2-8da9-578bf167b229)
Implementation Steps
1. Create a Git repository (using AWS CodeCommit or GitHub).
2. Clone the repository and copy the static files from S3.
3. Commit and push the static files to the repository.
4. Enable web hosting with AWS Amplify Console.
![Amplify Hosting](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/44c5a2cf-7d48-4161-9541-fba02882e51c)
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/889eac63-7a13-45fd-881c-19ba021eea33)
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/7da86c4a-be22-40c4-b770-b519900e9133)
5. Modify your site

![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/2a080e00-a570-4c9c-9fb3-2e45d0838cb7)

## Module 2: User Management
This module focuses on setting up user management and authentication using Amazon Cognito.
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/69f6ca7a-40c7-44d8-95ed-7b22627562b1)
Implementation Steps
1. Create an Amazon Cognito User Pool.
2. Update the website configuration with Cognito user pool details.
3. Register and confirm user accounts.
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/de6be34b-f6ed-4844-915f-3cc7ca0f710d)

## Module 3: Serverless Service Backend
Build a backend process for handling ride requests using AWS Lambda and Amazon DynamoDB.
![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/455aabe6-6278-45d7-8222-3bf0d9b02faf)
Implementation Steps
1. Create an Amazon DynamoDB table for ride data.
2. Create an IAM role for the Lambda function.
3. Create a Lambda function to handle ride requests.


## Module 4: Deploy a RESTful API
Expose the Lambda function as a RESTful API using Amazon API Gateway.

![image](https://github.com/shivamdeshmukh/WildRydes_Website/assets/72214326/dc22cc6e-758c-434d-b037-01f06f0cfeb2)

Implementation Steps
1. Create a new REST API using Amazon API Gateway.
2. Create a new resource and method for ride requests.
3. Deploy the API.
4. Update the website configuration with the API invoke URL.

## Usage
Follow the implementation steps outlined in each module to set up the different components of the WildRydes web application. The provided steps cover setting up static web hosting, user management, serverless backend, and deploying a RESTful API. The application will allow users to register, log in, and request unicorn rides.

For detailed information and step-by-step instructions, refer to each module's file in the Modules folder.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
This project is based on the AWS WildRydes example and makes use of various AWS services. Special thanks to Amazon Web Services for providing the resources and inspiration for this application.
