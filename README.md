<!--
title: 'AWS NodeJS Example'
description: 'This template demonstrates how to deploy a NodeJS function running on AWS Lambda using the traditional Serverless Framework.'
layout: Doc
framework: v3
platform: AWS
language: nodeJS
priority: 1
authorLink: 'https://github.com/serverless'
authorName: 'Serverless, inc.'
authorAvatar: 'https://avatars1.githubusercontent.com/u/13742415?s=200&v=4'
-->

# Event Driven project with serverless integration

## This is the Diagram of the model implmented

![Image text](https://github.com/kiskee/node-ses-service-aws/blob/main/images/EventDia.png)

## Overview

This project utilizes serverless architecture to create an API Gateway that connects to a Lambda function, which in turn leverages Amazon SES (Simple Email Service) to send emails.

## Table of Contents
* Overview
* Getting Started
* Prerequisites
* Installation
* Usage
* Configuration
* Sending Emails
* Contributing
* License


## Getting Started
### Prerequisites
Before you begin, make sure you have the following prerequisites installed:

* Node.js (v12 or higher)
* Serverless Framework
* An AWS account with access to Lambda and SES
* AWS CLI


### Installation

1. Clone the repository:

```
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

2. Install dependencies:
```
npm install
```

3. Configure your AWS credentials using the AWS CLI:
```
aws configure
```

4. Start a serverless project

![Image text](https://github.com/kiskee/node-ses-service-aws/blob/main/images/initServerless.png)

## Usage

### Configuration

1. Update the serverless.yml file with your AWS configuration settings, such as the region and IAM roles.

![Image text](https://github.com/kiskee/node-ses-service-aws/blob/main/images/serverlessYml.png)

This configuration sets up an AWS Lambda function named "create" that is triggered by HTTP POST requests to the "/contact-us" endpoint, allowing you to handle contact form submissions and interact with Amazon SES for sending emails.

![Image text](https://github.com/kiskee/node-ses-service-aws/blob/main/images/lambdaFunction.png)

2. Configure your email settings in the Lambda function code. Update the code to specify the sender's email address, recipient's email address, subject, and message content.

```
We can see this conde in the index.js file inside this same repository
```























