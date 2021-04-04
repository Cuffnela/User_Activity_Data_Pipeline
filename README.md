# Data Pipeline: Tracking User Activity 

This is a theoretical project completed during the MIDS program at UC Berkeley. 
The project utlizes a multitude of tools to implement ETL with parallel processing 
through custom Spark lambda functions. Google Cloud platform and docker containers were 
used throughout the project.

## Original Project Brief

In this project, you work at an ed tech firm. You've created a service that
delivers assessments, and now lots of different customers (e.g., Pearson) want
to publish their assessments on it. You need to get ready for data scientists
who work for these customers to run queries on the data. 

### Tasks

Prepare the infrastructure to land the data in the form and structure it needs
to be to be queried.  You will need to:

- Publish and consume messages with Kafka
- Use Spark to transform the messages. 
- Use Spark to transform the messages so that you can land them in HDFS

In order to show the data scientists at these other companies the kinds of data
that they will have access to, decide on 1 to 3 basic business questions that
you believe they might need to answer about these data.

### Deliverables

- `docker-compose.yml` used for spinning the pipeline. 
- Jupyter Notebook report containing the following
    - Relevant code for pipeline initialization for reproducibility
    - Sample business questions and answers from SQL queries

## Data

To get the data, run 
```
curl -L -o assessment-attempts-20180128-121051-nested.json https://goo.gl/ME6hjp`
```
Note on the data: It is a nested JSON file, where you need to unwrap it
carefully to understand what's really being displayed. 