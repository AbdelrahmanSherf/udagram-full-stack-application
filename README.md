# Udagram [![CircleCI](https://circleci.com/gh/circleci/circleci-docs.svg?style=svg)](https://github.com/AbdelrahmanSherf/dagram-full-stack-application) 

The udagram application is an application that includes all the major components of a Full-Stack web application.

# [Chlick Here For More Information About Project's Infrastructure Provided by AWS, Screenshots included](./Documentation/project-infrastructure.md)
# [Chlick Here For More Information About Pipeline-Infrastructure Provided by CircleCi, Screenshots included](./Documentation/pipeline-infrastructure.md)

## Provision the necessary AWS services needed for running the application:
1. AWS RDS Link [database-1.c3figwjumoou.us-east-1.rds.amazonaws.com](database-1.c3figwjumoou.us-east-1.rds.amazonaws.com)

2. AWS S3 Bucket for Front-End Link [http://udagram-704326196974.s3-website-us-east-1.amazonaws.com](http://udagram-704326196974.s3-website-us-east-1.amazonaws.com)
3. AWS EB for Back-End [http://Udagramapidev2-env.eba-kvwe23rr.us-east-1.elasticbeanstalk.com/api/v0](http://Udagramapidev2-env.eba-kvwe23rr.us-east-1.elasticbeanstalk.com/api/v0)

## Getting Started Locally

- Install all Modules with `npm i`
- Connect to the default user on PSQL terminal and setup a dev database, run `CREATE DATABASE <DB NAME>`
- Create an environment variables file in the root dir of `udagram-api`, the schema for the .env file is:
```
POSTGRES_HOST =         <YOUR VALUE HERE>
DB_PORT =               <YOUR VALUE HERE>
PORT =                  <YOUR VALUE HERE>
POSTGRES_USERNAME =     <YOUR VALUE HERE>
POSTGRES_PASSWORD =     <YOUR VALUE HERE>
POSTGRES_DB =           <YOUR VALUE HERE>
RDS_DIALECT =           <YOUR VALUE HERE>
AWS_REGION =            <YOUR VALUE HERE>
AWS_PROFILE =           <YOUR VALUE HERE>
AWS_BUCKET =            <YOUR VALUE HERE>
URL =                   <YOUR VALUE HERE>
AWS_ACCESS_KEY_ID =     <YOUR VALUE HERE>
AWS_SECRET_ACCESS_KEY = <YOUR VALUE HERE>
JWT_SECRET =            <YOUR VALUE HERE>
```
- Start the api with `npm run dev`
- Start the frontend with `npm run start`

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version
- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project
- AWS CLI v2, v1 can work but was not tested for this project
- A RDS database running Postgres.
- A S3 bucket for hosting uploaded pictures.

```

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
