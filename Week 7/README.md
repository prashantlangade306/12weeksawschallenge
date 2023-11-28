1. Create cloud 9 env. Name it as Labenv

![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4372c3b8-a7b5-470d-bddd-7f59b3338c5e)

2. Create Amazon ECR repo. Name it as myrepo
   
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c17c6cf5-7e8a-4414-93d1-414783a54edf)

3. Click on view push commands to view the commands
   
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ce209d78-ac61-4565-bf4a-6815158741f2)

4. Check the docker version in cloud9 env.
   
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/efab9603-bdfc-45a5-8e5d-5c9424b05679)

5. Create basic python app. app.py with the code that returns welcome page
   
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f1368ac2-9d18-4084-9c78-3e64a687dbbd)

6. Create Docker file with add this app.py file to the root directory and then installs Flask framework. This then also sets the entry point command to run this app.py when the ECS container starts
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7cd02446-b73b-4f2e-b26e-76ee26b9482a)

7. Then return to push commands and run it in sequence as below.
   Below command will show Login succeeded 
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a0cca26e-4c96-4504-8417-aa17f8a17ae9)

8. Belwo will build the repository (myrepo) that we created
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/33e7e26e-af87-4aa5-ad40-9be2fbd74c2b)

9. Next couple of commands will tag myrepo and then push the image to ECR
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a36c5ca5-162e-4143-95d5-2a6aa8d70692)

10. You can see this creates a new repository with the name myrepo in ECR console
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/da7aad32-dc32-4f94-a98c-a667d09fe26a)

11. Create ECS cluster mycluster
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/b55c4766-9a08-4626-8898-e7c15012ba00)

12. Then create a task defination with the name as mydefination. This can be used to deploy a service or run a task
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5626e03c-2247-4bbf-9379-2c79bf5c8dc8)

13. Click on the mycluster to see service named myfargateservice is deployed.
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/08c56446-66fe-486c-aab0-341fe80c5d9b)

14. Under "Tasks" tab, you can see the task as below
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/05af545c-6c75-474d-9378-2f475e000265)

15. Click on the task id to see the details of the task
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ff8a5bb1-1e00-4b37-a65f-b2628e78153a)

16. When you click on Public IP, it displays the contents from app.py - welcome message!


    Congratulations, you have successfully deployed a sample application on ECS Fargate!!!
