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
   
