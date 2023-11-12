**Lab 1**: Migrating Taxi data to Amazon DynamoDB and Amazon Aurora using AWS DMS

**Overview:**


In this lab, we will be performing a migration of sample taxi application data from RDS Oracle to Amazon DynamoDB and Amazon Aurora PostgreSQL databases using Amazon Database Migration Service (DMS)

**High Level Architecture (HLA):**

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ba36bad4-8c63-4a54-a0b8-e3045ec749dd)

**Lab Pre-requisites:
**

1. Create a stack based on the cloud formation stack 

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/81adb042-c992-4cc2-8f1a-d96b5c8ffdcc)

2. Clone the github repo https://github.com/aws-samples/amazon-rds-purpose-built-workshop.git

  cd ~/environment
  git clone https://github.com/aws-samples/amazon-rds-purpose-built-workshop.git

  Install PostgreSQL client
  
  sudo yum install -y postgresql96 postgresql96-contrib postgresql96-devel 

  Install JQ in the Cloud9 environment
  cd ~/environment
  sudo yum -y install jq gettext

  Connect to target Aurora PostgreSQL using psql command 

  Format: 
  psql -h <Host Name> -U <Username> -d <Database Name> -p <Port>
  e.g. psql -h xxxxx.us-east-1.rds.amazonaws.com -U auradmin -d taxidb -p 5432

  ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6e644e8e-e444-44a7-8a59-1b153d9910ee)
  ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/b4d05244-1360-4faf-8103-0876bde10d03)
  ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/796dcb91-aac4-4b32-81c5-172522155196)
  ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4a5ae789-a4e2-44ef-ac3a-191ee531baf1)


We have done with all the pre-requisites for this lab and good to proceed with the data migration part.

**Creation of Source and Target database endpoints:**

1. Create a Source endpoint for Oracle RDS

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cadb137e-fe4f-4279-91cb-fdc0a3d5e335)

2. Test endpoint connection
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d523285f-fd3e-4d83-b596-7d5b86d80239)

3. Create a Target endpoint for Aurora PostgreSQL
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a21dfa24-ff7d-471e-a466-cc0780688092)

4. Test endpoint connection
   ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bba1eb2c-b85d-4be2-a656-4dd8ccc4b1fb)

5. Create a Target endpoint for Amazon DynamoDB
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6f76ed0c-5c0f-4792-a472-590c3eef4c89)

6. Test endpoint connection
   ![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/878af809-b60f-4d80-a48a-e08faa0a031a)


**Migrate data from Oracle source to DynamoDB target**


Creating Replication Task for DynamoDB Migration
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1533768f-c180-48bf-877c-a9ada9113b3c)

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/da287424-0313-4371-916c-dbe6e029c544)
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fa3a683d-36f2-4992-baee-7e7dde809fd6)

Monitoring Replication Task for DynamoDB

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2df46ef3-e6be-4a72-9705-469d6d793d6c)

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/42847960-6b31-4797-8724-088ff554f89d)

Migrate data from Oracle source to Aurora PostgreSQL target
Creating Replication Task for Aurora Migration
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dd4ea13d-cc49-4619-a3ec-fbac8767e507)

Monitoring Replication Task for Aurora PostgreSQL
![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3872eb79-3a90-48c2-b970-673ac6d98184)

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/86059947-c959-4510-a61f-225573898cfe)

![image](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f4aa5033-613c-4b34-aecf-d8f8e9d335fa)

Lab1 has been successfully completed and we are moving to Lab 2.







