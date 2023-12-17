[tracks_list.json](https://github.com/prashantlangade306/12weeksawschallenge/files/13694281/tracks_list.json)1. Overview of the AWS analytics architecture

![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9cbf1eaf-bc8e-4896-bc10-512f6255a7a8)

2. Create S3 bucket as below 
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6d1f0efc-d218-4f72-9151-daabf73175eb)

3. Create a folder named "data" inside that S3 bucket
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/33d2d697-16c8-40c4-80bb-91bc54ef319d)

4. Create a folder named "reference_data" inside that folder
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/89780e29-8f54-4197-aec8-74313528f97a)

5. Upload the tracks_list.json file to the bucket
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/205f9772-9266-4266-8095-864662555a81)

6. Go to Amazon Kinesis Data Firehose console and create a delivery stream
![6E](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/80feff9e-fcf4-4884-bd99-90bb27ad66a6)

7. Then go to Cloudformation console and create a stack 
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/50f8b401-79a1-43a9-92af-d476289b843e)

8. Provide details as shown
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/da832aa1-ef34-4d4b-8353-7055b39f6478)

9. Monitor the cloud formation logs and verify the stack status is "CREATE_COMPLETE"
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/201a0ff0-77f1-4d68-b19b-feb8d58e443d)

10. Then go to Outputs tab and click on the link for KinesisDataGeneratorUrl
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/febfda23-9e63-4900-9b5f-9d1435002845)

11. This will open the Kinesis Data Generator in new window.
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/79ba4acd-d5ce-4efc-8dc0-4542c863bdde)

12. Select Region as "us-east-1" and provide other details as shown and click on send.
    Once the count reaches over 10,000, click on stop.
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c002748b-0e82-4a5b-aa49-e0b54af89b5e)

13. Go back to S3 console and access the S3 bucket created previously. There are various folders created inside data/ directory for the data streams as shown
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d473865a-66ea-4928-92d4-f396e3411429)

14. Now look at the architecture diagram below for storing, catalog and transform component
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ecf45f4d-3355-4ce5-a571-c54c362406d2)

15. Create IAM role that will be used by AWS Glue to call other AWS services
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0bd8c0b9-71f7-4cc5-96bb-78b313d81510)

16. Ensure to assign Admin access and AWSGlueServiceRole and create the role
![16](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2e33d58b-e057-4bda-ab11-508ea7d8aab8)

17. Create a new Crawler where the source data is S3 and provide the S3 path
![17](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/909daa8d-a86c-4414-969c-23c18a3637e4)

18. 
![18](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1558fe62-4398-4422-a242-150332ab0fd6)
![19](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dd1d8897-af2e-4181-858a-55ac3bfe59dd)
![20](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ace59e66-769c-45a8-b19d-6722c558a9f8)
![21](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a0ae256e-acbc-471e-9973-15b0106b8b90)
![22](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0216cf25-ae2c-4c39-9226-6afe79d07b5d)
![23](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/eddd52b3-686a-45ad-a9fb-9ec1e9e12b49)
![24](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/837a6fd0-e689-40a1-9468-06b68afd11db)
![25](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/005631e3-9905-4014-9c83-0114f869f4cd)
![26](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a7464d6c-ad5d-47ba-84d7-eade09981f64)
![27](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2671e530-d2d0-4c07-a454-196135848651)

![28E](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6a7f7996-ffd9-46a5-9beb-de63379cd33c)


![29](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7e5808ec-391d-418a-9674-561139210061)
![30](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ed57b44f-fbeb-4f9e-9773-6f595d124574)
![31](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cf8da5e8-f54d-457b-b623-0da7f58a7fa8)
![32](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e7477300-cb85-4fc5-bd75-94aeef7387e7)
