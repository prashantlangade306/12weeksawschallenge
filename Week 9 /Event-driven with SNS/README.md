1. Create Orders SQS queue.
![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/34adfac6-6a1b-4c68-8590-973c9e71debe)

2. Specify the SNS queue for this queue
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a4297241-599d-4d5c-9333-7c97ebfd609f)

3. Update the access policy to grant access to the subscribed SNS topic
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d43e64b1-9966-4b1c-af22-da9a6136d3cd)

4. Publish the message to the topic
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/18204b82-2226-4747-8839-10674689021e)

5. Successful publishing of the message
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c4f76473-b254-41a8-93c8-4d8bdf81c7f6)
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/24577430-30e3-4d16-9ba2-fd412e735c34)

6. View the SQS queue for Orders with messages available as 1
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dac8fa2b-d732-4e1c-bf1c-017659308310)

7. Poll messages and you can see the details of the message 
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/26799d7d-2783-496b-b27c-52bd2010423d)

8. Select the message and delete it
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d48f8119-8830-4cbc-aa3a-f804a6d3ad2b)

9. Successful deletion of the message.
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cb783be1-2747-4123-ac77-bf2ef7f3b556)

10. Create a new SQS queue - Orders-EU
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/aad88db7-af69-4f2c-b309-8a2d99a29932)

11. Check the details of the created order
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d3dd3258-27ea-4d32-ac4e-ffef0cd0a199)

12. Check the SNS subscription
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e2d9d623-a9a5-47d9-bc1e-11220fc7b290)

13. Edit the filter policy based on the location - eu-west
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bb4596cd-f8cf-413b-a373-6e562acf04f1)

14. Save the updated details
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a00c24c2-487d-446c-9d19-e44445190b95)

15. Create BookOrders queue
![16](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/226afa72-4ea1-4627-8f28-7fcf18f0b508)

16. Check the BookOrders details
![17](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/12bd8ca1-3546-441d-860a-05d6472c7415)

17. Check the Orders subscription
![18](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/71632db1-1c50-4f1a-ae0a-d3639b54107d)

![19](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7118df5a-9990-4a32-9f2f-d653d9b00712)

18. Update the filter policy with category - books
![20](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a6ef3acc-e700-4787-b099-4cff46dbfe60)

19. Save the subscription
![21](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7f5386d4-6ada-4551-a0d2-868e5fcda76b)

20. Publish Test message to this topic
![22](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/44813f57-e4ff-4e43-97ab-1a4e9ef02aee)

21. Message successfully published
![23](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5b31f7eb-811c-4e7e-98b8-a81bef49d860)

22. Again publish Test message to this topic
![24](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/89a9e813-51d5-42ff-af28-567f388a2aa6)

23. Message successfully published
![25](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e45f5280-89ab-4198-af6b-c0ae404a32b9)

24. Again publish the message with different content as shown
![26](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7207b4b3-cde5-4895-805a-f432fcd53d81)

25. Succesful publishing of message
![27](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/43de767e-0215-47bd-8c3c-3da12964a636)

![28](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e04021a9-4883-46af-a0f4-12bb65cfd296)


![29](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ed6b15e6-bdc9-4379-858c-06fe13d43666)

26. View all the queues with different number of messages published to each queue.
![30](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0b04b9f2-02c7-42f8-9175-6c773fbbace2)

27. Create a new SQS - Orders-XL
![31](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7129ff69-c8b0-4202-ac46-7a76974e7637)

28. Create the subscription to the SNS topic
![32](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7c0a4753-35cb-44aa-92f3-b996ea8a4f31)

29. View the subscription topic 
![33](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/584822fe-d5e0-4c79-8289-cf76121fbf77)

![34](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5e937088-3679-42b3-93dc-7d264270c001)

![35](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4941ec6a-7122-4b19-b24e-8dd35793da22)

![36](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9c898d84-d872-444b-99f4-56cee94d810d)

![37](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/75c085ff-d82b-4b7c-b73c-5c2f8bd0809b)

![38](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1a412d93-7524-4cb0-95f7-053a93ff13ea)

![39](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/df7988e8-b10c-4609-825a-c94d5b25215a)

![40](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8f37e57c-31ae-4f1f-b283-597703dc4402)

![41](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fd465c7a-fd13-45b4-bc6f-32ec1a95c852)

![42](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/87eabf8f-25c0-458c-9785-78d3ea6738fd)

![43](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2865f051-dc25-47bf-aaeb-e863da9a3e32)

![44](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3a832d46-cbd4-4bd2-84ca-7e8f5762ca9e)

![45](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0e7ff72e-efe3-47e6-bb2a-da2923d7b371)

![46](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/53452975-09f9-44cc-be4d-5bea085adcaa)

![47](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/28f77cd7-67a5-4442-96b9-8f7bbfa4539d)

![48](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1586d826-aafa-42d8-92e3-9085fa8cd93e)

![49](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9793910b-fe04-41eb-bd67-09aa3068d50b)

![50](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/be28a88b-c5ac-4f5e-9d0a-54ab788d9bca)

![51](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f01ccc2b-56cf-424c-baba-2f61cd04eb4c)

![52](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4fe00288-19c4-4f1d-b2fd-47f0a6069b32)

![53](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/18a5cefb-48b7-491d-8e92-973855331e46)

![54](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/741278b4-a616-4232-9087-149f78cf1bf7)





















