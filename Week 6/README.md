Infrastructure as a code

1. Create Cloud 9 env
   
![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/01478188-e68d-4c98-ad65-d63c60f30851)

2. Clone the repository
   
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a7de095a-bf4c-4fd3-9fda-d2d05a802473)

3. Update CLI version
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/13ee6fe7-766f-42c7-b968-a0865cb1ae00)
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f0e694c6-9977-4b7f-bc6e-0d96afa961fd)

5. Add the S3Bucket creation code in template-and-stack.yaml
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7ddf6419-19d7-47cd-a068-054bdb72c157)

5. Run the stack creation command and this will create a StackId if the command is successful
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8b7a782c-2c7e-4fae-bd10-6bd0298dcd83)

6. Check CloudFormation console to see if the stack (cfn-workshop-template-and-stack) is created successfully.
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/22e5f839-dc6e-4d9f-b221-93f4b07b2a22)

7. Update template-and-stack.yaml file to include versioning configuration to be enabled. 
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/35242f38-b268-4105-959e-e34f472e7fde)

8.Run the stack update command and this will create a StackId if the command is successful
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bae9a586-3ccd-419d-80ed-84da5ca4a94c)

9.Check CloudFormation console to see if the stack (cfn-workshop-template-and-stack) is updated successfully.
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9d65d761-4932-4e82-9bbf-d792f63861a7)

10. Open resources.yaml and add the code to create EC2 configuration
    
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/90a31807-007b-46ac-b19d-26cb517f0f28)

11. Run the stack creation command and this will create a StackId if the command is successful
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fc62f42a-960c-4492-bd10-29a11de1cca0)

Check the CloudFormation console to see the stack is successfully created.
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9ba57207-bec6-4988-b9f8-f8060d7b9d6b)

12. Run the command to get the AMI Id
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2ef148d5-8b11-4463-8d1f-1280e0d5802e)

13. Open instrinsic-functions.yaml and add the code for creation of EC2 instance referencing AMI Id
![16](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ec50c3f0-e9b2-47f7-bc08-190810898c51)


14. Run the stack creation command and this will create a StackId if the command is successful. Notice the AMI Id used in the command from previous step.
![17](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f18dd0b9-2c97-4112-b5e4-1035100baaf0)

15. Check CloudFormation console to see if the stack (cfn-workshop-instrinsic-functions) is created successfully.

![18](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1b336bc5-1975-48b4-83c6-c83153bae043)

16. Open EC2 console and see the webserver instance is up and running.

![19](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6c1da435-628f-46ea-a2b2-2405b1b7a8af)

17. Open instrinsic-functions.yaml and update the code and run the update stack command
![20](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/32f3fdae-30a4-4b2e-b59b-c97c26a1c6d4)

18. Check CloudFormation console to see if the stack (cfn-workshop-instrinsic-functions) is updated successfully.
![21](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c216dc95-a806-4eb6-8f80-9389f37c812b)

19. Open EC2 instance console and check that the "Tags" tab has all the correct values as updated in the previous step.
![22](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6f9d7d6a-e301-4688-a9b0-6155a7d4a08b)

20. Open mappings.yaml and add the code
![23](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/04c8fd76-794b-49fb-8d4d-e7b262b87a63)

21. Run the stack creation command and this will create a StackId if the command is successful
![24](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/88237238-8def-4a80-98be-84cae040e4ce)

22. Check CloudFormation console to see if the stack (cfn-workshop-mappings) is created successfully.
![25](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ecd15294-5eaf-44c3-a814-335cb053b168)

23. Open outputs.yaml file and run the create stack command.  Notice the AMI Id used in the command from earlier step.
![26](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3e0cfe21-dc38-4087-9a6a-c802c190a549)

24. Check CloudFormation console to see if the stack (cfn-workshop-outputs) is created successfully.
![27](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8f2be8d3-428e-47ec-8655-1186ea15841c)





