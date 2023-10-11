# Dalmatian

AWS SAM + Node.JS app/test harness, being used to demonstrate automated deployments for AWS for a client.

This project includes:

1. A basic set of lambda functions, written in Node.JS (Typescript)
1. AWS Serverless Application Model (SAM) configs that describe our AWS Infrastructure as Code (IaC), including:
   1. AWS API Gateway
   1. AWS Lambda functions
   1. AWS IAM Roles
   1. AWS S3 Buckets
   1. AWS CloudFormation (automated via SAM)
1. [pending] Automated deployment via GitHub Actions

## Deployed resources

- Hello world (GET) API
  - [Prod](https://0tl3p69tl9.execute-api.us-east-2.amazonaws.com/Prod/hello/)
  - [Staging](https://0tl3p69tl9.execute-api.us-east-2.amazonaws.com/Stage/hello/)

## Clients: contributing to, or using, this repo

Developers are encouraged to contribute to this repo, below are some staring points. You should also check out the [AWS SAM Hello World Tutorial](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-getting-started-hello-world.html).

### Prerequisites

The following software is needed for you to be able to build a run this software:

- [NodeJS](https://nodejs.org/en)
  - v18.16.0
  - v9.5.0 of npm (comes with node)

#### Optional software

The following software is optional, but is highly recommended.

##### Manual deployment tools

If you are involved in _manually_ deploying this API on [Amazon Web Services (AWS)](https://aws.amazon.com/), you will need the following software:

- [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/)
  - v2.x.x
- [AWS Serverless Application Model (SAM) CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
  - v1.x.x

Note that developers do **not** need to install the AWS CLI or the AWS SAM CLI, it is only required for _manual_ deployment; the deployment process is automated via GitHub Actions.

##### Local testing tools

To test this  API's lambda functions locally, you should install the AWS CLI & AWS SAM CLI tools as listed above, plus the following:

- [Docker](https://www.docker.com/)
  - v2x.x.x
  - Docker Desktop can also be used (recommended)

Reference guide: <https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-docker.html>.

**Note testing your code locally may result in the team being grumpy with you. Don't be _that_ guy - test your code.**
