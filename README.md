# banking-modern-datastack
This project is based on the pipeline build using dbt, docker, airflow, python, sql 

# Project Flow

1) Created Postgres Database
2) All the changes in the database are captured by CDC(kafka  + debezium) which is data streaming stage.
3) The streamed data is then pushed into s3 bucket, and then data is pulled out and pushed into snowflake bronze table
4) The whole data processing is done by DBT
5) Snowflake is a data warehouse
6) Whole process is orchestrated using Airflow
7) We then implemented Continous integration and Continous Deployment (CI/CD)
8) Then business ready data is then connected to POWERBI where we build beautifull dashboards 
