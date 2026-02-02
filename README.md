# DTC_HW2
### Overview

This repository contains my solution for Homework 2 of the DataTalksClub Data Engineering Zoomcamp.
### Pipeline Setup

I used the provided YAML configuration:

gcp_taxi_scheduled.yaml

The pipeline was executed with backfilling enabled in order to generate data for the required historical dates.

The backfill produced the necessary files/tables used to answer the homework questions.

No custom modifications were made to the pipeline logic itself — the focus was on correct scheduling and backfill execution.

Answering Questions (Q3–Q5)

For questions 3–5, I used simple SQL aggregation queries:

Basic COUNT(*)

Filtering by the required date ranges

No additional transformations or joins were needed
sql```
SELECT COUNT(*)
FROM <table_name>
WHERE <date_column> BETWEEN '<start_date>' AND '<end_date>';```
