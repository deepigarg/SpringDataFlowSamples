# SpringDataFlowSamples
This repository contains two sample tasks using Spring Cloud Data Flow server.
1. Bill-setup-task:\
It reates a table in the SQL Database.
2. Bill-run-task:\
It calculates the bill amounts for the users mentioned in the given Json file, and stores the bill details in the table created in the previous task.

## Requirements
- docker
- java jdk version 17
- JAVA_HOME should point to the the jdk version 17

## Setting up mysql for the tasks
If you do not have an instance of MySQL available to you, you can follow these instructions to run a MySQL docker image for this example:

- Pull a MySQL docker image by running the following command:\
docker pull mysql:5.7.25

- Start MySQL by running the following command:\
docker run -p 3306:3306 --name mysql -e MYSQL_ROOT_PASSWORD=password -e MYSQL_DATABASE=task -d mysql:5.7.25


## Runing the tasks

1. Bill-setup-task
  - Clone the project
  - cd into the billsetuptask
  - Deploy the project locally by following the steps mentioned from: \
  https://dataflow.spring.io/docs/batch-developer-guides/batch/spring-task/#deployment
  - To deploy and run the project using Spring Cloud Data Flow, follow \
  https://dataflow.spring.io/docs/batch-developer-guides/batch/data-flow-simple-task/#create-task-definition

2. Bill-run-task
  - Clone the project
  - cd into the billrun
  - Deploy the project locally by following the steps mentioned from \
  https://dataflow.spring.io/docs/batch-developer-guides/batch/spring-batch/#deployment
  - To deploy and run the project using Spring Cloud Data Flow, follow \
  https://dataflow.spring.io/docs/batch-developer-guides/batch/data-flow-spring-batch/#create-task-definition


