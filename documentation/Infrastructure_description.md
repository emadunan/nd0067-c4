# Udagram Application Infrastructure Description

## Services need to run in order to deploy the application
- AWS Relational Database Service (RDS)
- AWS Elastic Beanstalk (EB)
- AWS Simple Storage Service (S3)
- CircleCI

***

### AWS Relational Database Service (RDS):
Database environment that hosts a postgresql database engine version 13.4. The database endpoint is "database-1.c9pyylv2hx9y.us-east-1.rds.amazonaws.com" and running on port 5432.
![RDS screenshot](../documentation/screenshots/RDS_screenshot.png)

***

### AWS Elastic Beanstalk (EB):
An application server that hosts a backend API for Udagram application with NodeJS version 16 running on 64bit Linux 2/5.5.1 platform. The API Url is [udagram-api-dev222.us-east-1.elasticbeanstalk.com](http://udagram-api-dev222.us-east-1.elasticbeanstalk.com)
![RDS screenshot](../documentation/screenshots/EB_screenshot.png)

***

### AWS Simple Storage Service (S3):
Amazone Storage Service that contains buckets for the backend application which is served by elastic beanstalk and the frontend Angular application served by S3.
![RDS screenshot](../documentation/screenshots/S3_screenshot.png)

***

### CircleCI:
A service for continues Integeration and continues deployment. CircleCI is connected to my github account and linked to the master branch to the Udagram application repository (nd0067)
![RDS screenshot](../documentation/screenshots/CircleCI_screenshot3.png)