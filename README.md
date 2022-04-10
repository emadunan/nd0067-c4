# Udagram

A Full-Stack web application where visitors can freely register without charges and post their feeds in the web application. The application consists of an Express API runs on Nodejs runtime and an Angular frontend application.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

## Run Locally

### Environment Variables

To run this project, you will need to add the following environment variables to your .env file

POSTGRES_USERNAME=retailer 
POSTGRES_PASSWORD=emadunan 
POSTGRES_DB=retailer_db 
DB_PORT=5432 
POSTGRES_HOST=database-1.c9pyylv2hx9y.us-east-1.rds.amazonaws.com 
PORT=8080 
AWS_REGION=us-east-1 
AWS_PROFILE=eb-cli 
AWS_BUCKET=udagram222 
URL=udagram-api-dev222.us-east-1.elasticbeanstalk.com 
JWT_SECRET=udacity 

### Install Postgresql database engine

#### PostgreSQL database engine configured to run on port 5432.

#### Connect to the database as ***postgres***, and run the following commands to create and configure the required databases for development.

##### Create database for the API project development

```sql
  CREATE DATABASE retailer_db;
```

##### Create database User and grants it the required privileges

```sql
  CREATE USER retailer WITH PASSWORD 'emadunan';
  GRANT ALL PRIVILEGES ON DATABASE retailer_db TO retailer;
```

Clone the project

```bash
  git clone https://github.com/emadunan/nd0067-c4.git
```

Go to the project directory

```bash
  cd nd0067-c4/udagram-api
```

Install the API dependencies

```bash
  npm install
```

Start the application server

```bash
  npm run start
```
Return to the project directory

```bash
  cd nd0067-c4/udagram-frontend
```

Install frontend dependencies

```bash
  npm install
```

Start the web server

```bash
  npm run start
```


### AWS

Provision the necessary AWS services needed for running the application:

#### AWS RDS for the database: Endpoint "database-1.c9pyylv2hx9y.us-east-1.rds.amazonaws.com" on Port "5432"
![RDS screenshot](./documentation/screenshots/RDS_screenshot.png)

#### AWS ElasticBeanstalk for the API [http://udagram-api-dev222.us-east-1.elasticbeanstalk.com](http://udagram-api-dev222.us-east-1.elasticbeanstalk.com)
![RDS screenshot](./documentation/screenshots/EB_screenshot.png)


#### AWS s3 for web hosting [http://udagram222.s3-website-us-east-1.amazonaws.com](http://udagram222.s3-website-us-east-1.amazonaws.com)
![RDS screenshot](./documentation/screenshots/S3_screenshot.png)

### CircleCI




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
