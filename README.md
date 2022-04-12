# Udagram

A Full-Stack web application where visitors can freely register without charges and post their feeds in the web application. The application consists of an Express API runs on Nodejs runtime and an Angular frontend application.

Here is the link for the frontend [Udagram Application](http://udagram222.s3-website-us-east-1.amazonaws.com).

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

***

### **AWS** *services needed for running the application*:

#### ***AWS RDS*** for the database: Endpoint "database-1.c9pyylv2hx9y.us-east-1.rds.amazonaws.com" on Port "5432"
![RDS screenshot](./documentation/screenshots/RDS_screenshot.png)

#### ***AWS ElasticBeanstalk*** for the API [http://udagram-api-dev222.us-east-1.elasticbeanstalk.com](http://udagram-api-dev222.us-east-1.elasticbeanstalk.com)
![RDS screenshot](./documentation/screenshots/EB_screenshot.png)


#### ***AWS S3*** for web hosting [http://udagram222.s3-website-us-east-1.amazonaws.com](http://udagram222.s3-website-us-east-1.amazonaws.com)
![RDS screenshot](./documentation/screenshots/S3_screenshot.png)

***

### CircleCI Pipeline with Github

#### 


## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

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
