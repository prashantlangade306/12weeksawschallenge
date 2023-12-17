A. Create a SQS Queue

![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/38fb55eb-4e05-4e49-9b6c-e3b466ee6038)

B. Create a Lambda Function
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d24374a5-4ccc-492b-a083-8c4b0c38645b)

C. Ensure under Triggers, SQS state is "Enabled"
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/70c47791-3253-49e0-b687-64f65450661a)

D. If the state is not "Enabled", check the checkbox against "Activate Trigger" and click on save
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7479a009-74cc-4a84-ae97-4e3e6956bcda)

E. Go to SQS console and send a sample message as shown below. Click on "send message" 10 times.
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fe52752d-3e6c-4858-84bd-54c53e3d815d)

F. Go to Cloudwatch console and then to Log groups from the left hand panel
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/150d3633-195d-4101-999e-676f7455a7be)

G. click on the log group for the SQS queue and you can see the log events for the messages sent previously
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/721036df-9bc2-40ca-8cbe-8fee464b4e05)

H. In the same console, go to Logs Insights
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cc015af4-1384-45da-a451-29e966f924a3)

I. Analyze Logs using various queries
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/814c7ca5-911a-48d6-a0d8-93ac6b7b8ca7)

J. Change the limit from 20 to 5 and then run the query
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d9576303-3986-4bc0-9266-a1523d9d5428)

K. Change the query to count by timestamp under Logs Insights and see the output
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d7d2f0ca-db93-4ce8-977d-7d4e3e15637b)

L. Change the query to count it by bin(30s) and see the output
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5afc3f93-5da3-4fd2-aab7-5ec1959c9de2)

M. Under the "Visualisation" tab, you can see the liniear graph.
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1f72d7a6-0f7b-4524-b137-f72b190dfc93)

N. Change it to Bar from the dropdwon
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fb22ab20-0ad7-4a36-82b2-a91cbd625be4)

O. Finally validate the result of the labs as shown. Note: This is applicable only to those who are using Whizlabs account for running the labs.
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/86def9ba-c3ef-4ae8-b0fa-1252d9aaf22f)
