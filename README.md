# Project 2: Tracking User Activity

## Abstract 

In this project, a service that delivers assessments from an education tech firm was created. The data outcome is ready for further queries work according to customer's requirements. 

Main tasks of this project

- Publish and consume messages with Kafka
- Use Spark to transform the messages. 
- Use Spark to transform the messages so that can be landed in HDFS


---

## Problem Statement

The original data was acquired by 
```
curl -L -o assessment-attempts-20180128-121051-nested.json https://goo.gl/ME6hjp`
```
The data is contained in the file `assessment-attempts-20180128-121051-nested.json` in the Data folder, which is inclued in this repository. 


Questions are answered in this project:

- How many assesstments are in the dataset?
- What's the name of your Kafka topic? How did you come up with that name?
- How many people took Learning Git?
- What is the least common course taken? And the most common?
- Add any query(ies) you think will help the data science team
  
## Tool Used

- Docker Images: 
  - cloudera 
  - kafka                        
  - mids
  - spark
  - zookeeper_1  
  (docker configuration file __docker-compose.yml__ is included in the Code foler)
  
  
- Google cloud virtual machine 

- Jupyter Notebook

---


## Project Outcome

- Publish and consume messages with Kafka in topic assessment
  
- Use Spark to transform the messages(Spark TempTable: __select_assessment__, forced schema: __final_schema__) and can be landed in HDFS

- Question solved
  - 3242 distinct assesstments in the dataset
  - 390 people took Learning Git
  - The least common courses: Learning to Visualize Data with D3.js, Native Web Apps for Android, Nulls, Three-valued Logic and Missing Information and The Closed World Assumption
  - The most common course: Learning Git
   


 
---       

## Link to the report

[Project Report](Report\Project_2.ipynb)\
[Console history](Code\Haoyu_Zhang-history.txt)