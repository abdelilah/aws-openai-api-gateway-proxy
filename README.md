# AWS OpenAI API Gateway proxy

This is a simple AWS API Gateway proxy for the OpenAI API. It allows you to use the OpenAI API without having to expose your API key to the public. This is particularly useful if you want to grant multiple users access to the API and apply usage limits.

## Pre-requisites

- AWS account
- OpenAI API key

## Setup

Setup should be straightforward, you can either use the cloudformation template in this repo or use click the following button to open the template in the AWS console:

[![Launch Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://github.com/abdelilah/aws-openai-api-gateway-proxy/blob/master/cloudformation.yaml)

### Deploying using the command line with AWS CLI

```bash
aws cloudformation create-stack --stack-name OpenAI --template-body file://cloudformation.yaml --parameters ParameterKey=OpenAIKey,ParameterValue=YOUR_OPENAI_API_KEY
```