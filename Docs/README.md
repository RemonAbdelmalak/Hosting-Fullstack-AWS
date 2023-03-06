# Udagram

---

## Description

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### AWS Cloud Setup

- RDS - Database Host: database-1.co5afygpb7yx.us-east-1.rds.amazonaws.com
- RDS - Database Port: 5432
- RDS - Database Name: postgres

- S3 Endpoint - Frontend: http://projectbucket241769392460.s3-website-us-east-1.amazonaws.com/

- Elastic Beanstalk URL - Backend: http://udagram-api.eba-pmf3eyj7.us-east-1.elasticbeanstalk.com/

## Environment Variables

Setup the following variables in the .env file or in the cloud environments:
```
- POSTGRES_USERNAME = "postgres"
- POSTGRES_PASSWORD = "remonwagdy11"
- POSTGRES_HOST = "database-1.co5afygpb7yx.us-east-1.rds.amazonaws.com"
- POSTGRES_DB = "postgres"
- AWS_BUCKET = "arn:aws:s3:::projectbucket241769392460"
- AWS_DEFAULT_REGION = "us-east-1"
- AWS_PROFILE = "default"
- JWT_SECRET = "mysecretstring"
- URL = "http://localhost:8080"
- AWS_ACCESS_KEY_ID = "AKIATQSUUFFGBDZTWLOJ"
- AWS_SECRET_ACCESS_KEY = "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"

```

## Pipeline

From the root of the project:
- `npm run frontend:install`    - To install frontend dependencies.
- `npm run frontend:build`      - To build the Angular/Frontend.
- `npm run backend:install`     - To install backend dependencies.
- `npm run backend:build`       - To transpile the Typescript/Backend.
- `npm run backend:deploy`      - To deploy the project to EB 
## CircleCi

The order of the run jobs:

- Spin up enviroment.
- Preparing enviroment variables.
- Install NodeJS 14.15.
- Setting Up Elastic Beanstalk CLI.
- Install AWS CLI.
- Configure AWS AccessKeyID.
- Checkout Code.
- Frontend Install dependencies.
- Frontend Build the angular.
- Backend Install dependencies
- Backend Build.
- Deploy App.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd udagram-frontend`
2. `npm run test`
3. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework