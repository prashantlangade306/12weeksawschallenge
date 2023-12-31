
1. Create EC2 instance named "MyEC2Server"
![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0a31d2d3-d9c9-4caa-8de8-d47bc8333f0a)

2. Enable auto assign public IP and create a new security group
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/b0d5e9f1-dd74-47b6-856e-87f2173f7511)

3. Ensure to edit Network Settings and update the inbound Security Group rules as shown
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3991f288-09b4-4eb6-ae30-b0ea11f9744c)

4. Add the user data script as shown that will run during EC2 instance start up
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3afc971f-ee52-4288-9ee9-56aa040e61c6)

5. Once the instance is created, ensure it is in running state
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2d523433-edfe-4aea-86ad-0c1bf31d502b)

6. Go to Simple Notification Service in AWS console and create a topic named "CPU_util" as shown
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0fec2fd3-1946-4c10-8a95-5327cb22580c)

7. The topic is created successfully
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1f427a5a-74f3-4c2c-9dde-6e5e77061ced)

8. Now create a new email subscription 
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d99cedb7-0bac-4e99-8e38-bbb1cb186a63)

9. Confirmation of successful creation of subscription
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e1fe875f-c74a-4c5c-b44e-052bcdf4410f)

10. Once you accept the subscription link sent to your email, you can see it is in confirmed state.
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f198d313-8009-4872-81ed-4189de25ea78)

11. Check the average CPU utilisation graph for the last 1 hour
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ace01784-4013-4d10-ae8d-c8ae9c359c6e)

12. Now navigate to Cloudwatch console -> All Mertrics -> EC2 and find the instance name with "MyEC2Server" for CPUUtilisation as shown
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/88b4bf13-cdc8-4e85-8acf-5a6d9b1f34b4)

13. Select the checkbox and then navigate to "Graphed Metrics" tab 
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/847d3109-0592-484f-b8fc-059c5f65e1ef)

