# Pipeline Process
-After pushing commited code to github repository, CircleCI detect the changes since it was previosly linked to the github repository, then execute pipelines as it was defined in the config.yml file as follows:
- Preparing the environment
- Install the Frontend and backend dependencies
- Build the application components
- Deploy the application
![RDS screenshot](../documentation/diagrams/Pipeline_diagram.jpg)