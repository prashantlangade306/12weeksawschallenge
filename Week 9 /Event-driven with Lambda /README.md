1. Create a Lambda function - InventoryFunction with runtime as python 3.9
![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f7680c2c-fa17-4b10-8cda-925eea78886d)

2. Look at the details of this Lambda function 
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ad35fc2e-62bf-40d4-a086-f41edffb01c9)

3. Set the destination type to EventBridge and with Destination ARN
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f64d8f6d-2199-4e24-8761-a95db3ac7d63)

4. Save and it reflects the EventBridge
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/739fb5f3-3318-4187-be0d-5cfd06c39cee)

5. Create different rules - OrderProcessingRule and InventoryDevRule
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bd0773c5-7b29-4fee-8081-eda569a5c88e)

6. Create Event bus for Orders, Event Source as "com.aws.orders" and Detail Type as "Orders Processed" and Event Detail as shown below
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1ff2ef25-38c6-4ad2-9745-318fd11c289f)

7. Send the event
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bed27a27-92bb-42f2-af1f-2bcac1763c26)

8. Go to CloudWatch and access the Log groups as shown
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/436f38bd-e07c-4b5b-925b-5875ab85d069)

9. Add another destination for messages going to DLQ for Inventory
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f1e53542-1bbf-43a5-bd2d-3f3e7019651d)

10. Save the details and it reflects SQS
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/387573ac-9eec-4a38-a9d7-8bbce58cb71f)

11. Create Event bus for Orders, Event Source as "com.aws.orders" and Detail Type as "Orders Processed" and Event Detail as shown below
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e0cf3fab-0ef1-460e-897c-e35daf259db9)

12. Send the event
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cd185eb4-a42c-4e44-8f46-1b020c89ec38)

![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6cae7560-1b17-43a6-9038-43d78bcddb24)
