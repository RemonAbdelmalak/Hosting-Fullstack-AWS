# Udagram

## Description

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```
### Installation

1. Go to AWS and make sure that the RDS is setup and take the endpoint.
1. After that, go and create a S3 Bucket for your FrontEnd.
1. Now go and navigate to `cd starter/udagram-api` and type `npm install`.
1. Then, navigate to the `cd starter/udagram-frontend` and aslo type `npm install`.

<!-- ## Environment Variables

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

``` -->
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