1. Create a stack for event-driven architecture for the required resources for this lab

![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/facb90f8-afeb-43e4-8683-9029486e870c)

2. This is the architecture of the lab
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/eda38fd8-eb1a-4e89-a646-046bf1b89c79)

3. Create Event bus orders - Inventory and Orders
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f401a1d1-f528-4176-9fbd-9e1302f01026)

4. Create an EventBridge event rule - OrdersDevRule
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c51d11d6-2d29-46da-8745-7a99cd8a760c)

5. Add the event pattern
![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ec657dde-4458-4adf-a5e0-fecf1ddbdf2b)

6. Select Target with AWS service - Cloudwatch log group with orders log group
![6](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/13bc8634-ac50-4184-a673-4f837117f239)

7. Successfully created the OrdersDevRule
![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f5aa1fb9-0794-4632-a515-fc64f7bbb947)

8. Send the event
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d0c85603-5cc5-48cb-bf0e-64882ccd1e12)

9. Go to Cloudwatch log 
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6209e0d1-ca00-4bd4-9e5e-83a339cd49a5)

10. And check the log events for orders
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/bd0a65fb-e158-486d-be3e-c09bae9328ba)

11. Note down the API gateway endpoint URL from the CloudFormation stack console
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/492a4663-67cf-4b56-bc1b-075610aabbc3)

12. Create API destination 
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/52107cc2-48e5-4231-ad8a-cc69433ff47a)

13. Create another EventBridge Rule - OrdersEventsRule
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9ae69311-2267-4ba2-9da6-fa9c0e27f867)

14. Select EventBridge API destination in Target
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/006ba88e-613f-4f3e-9086-05873247a1e6)

15. Save and confirm that the OrdersEventsRule is created successfully
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/35649b35-7276-41e8-847d-91c2f04e8645)

16. Create Event source with event detail for Orders
![16](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ca01ca3f-0a38-44c3-b2f6-55e06ee39ef4)

17. Sent the Event
![17](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d9ab7b2b-ca03-4ba4-9a86-c6d08ec1e857)

18. Check the API gateway execution log and notice the log streams
![18](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9e9b704c-726b-4c03-8374-c2cad884adba)

19. Access the Cloudwatch log groups
![19](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d70f28e2-3ce8-4dd3-958c-814a78e4933b)

20. Create another EventBridge Rule - EUOrdersRule
![20](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8ce924d3-fd13-4981-8553-e11fdf4e1d4a)

21. Create Event source with event detail for Orders
![21](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f5eb3470-ec4c-40a4-8bf7-cbba21fcbcec)

22. Send the event
![22](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ce05387b-1851-4721-b302-ee15aba9e26b)

23. Create another Event source for USOrderEvent
![23](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4829b1c7-db4f-4c95-b1ca-393889bb0fca)

24. Send the event
![24](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/fad22bd5-9eca-419d-a00f-62684f04e137)

25. Check the Orders SQS 
![25](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2b8f8124-ddc9-4fd9-83b3-c43695ff63d7)

26. Create EventBridge Scheduler for OrdersProcessing
![26](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/35cccdcc-09c3-43e9-a71e-7391fb2b2d0d)

27. Create a scheduled event - PutEvents
![27](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e19f7e01-ca8a-4b55-8354-5cf3d9d46eb2)

28. The OrdersProcessing schedule is getting created
![28](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a9255bdd-0ce3-4fd7-9e57-5c898870af4e)

29. Check the log stream in the cloud watch and you can see the logs are getting updated based on the schedule run
![29](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/408b4f6f-b86c-4338-8897-e2ff93f71cfb)

30. Check the other details of this schedule - such as times when this schedule will run
![30](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e86f7541-f0c8-4919-a7c6-d75da1efcfda)

![31](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/65ca04d2-e78d-49b2-a058-88042b3ccf27)

![32](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/663052f7-b10c-431a-992e-8a8a401734b8)

![33](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/280c747e-721d-430f-b136-74958347ac29)

![34](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/126f5e4e-8679-4b32-9097-bce35846cadd)

![35](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c4e88e7d-4404-43b5-b06f-ecb98abe079f)

![36](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/be804e6f-dba4-4099-adc5-b7289195dc60)

![37](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5217635e-0661-43f4-a1c7-92a4ac84aa38)

![38](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cb4166d6-db2c-4a26-82f6-623b1fdee08d)

![39](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8932db42-24d5-4a85-aca4-8813f31e2463)

![40](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d0b2ca94-844a-415d-859c-f936583054eb)

![41](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7b35f54a-6ff0-4053-8e30-b3e7bf7281f5)

![42](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/91f226af-2487-4781-98f1-6ae0de43e72f)

![43](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/5cca4388-6ab3-4475-857c-a1054e9231c6)

![44](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8d5bfdf6-6a46-41ed-aa6e-820a1db1f839)

![45](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/24e38ac2-54f6-4a8c-9258-fc6b467cee33)

![46](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/398bcf5a-debd-4518-a8f7-ca7c275939d4)

![47](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dc5f94bc-48c1-42b2-b6b2-fc7ecc5fc815)

![48](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/68bfea1a-375b-457f-89e7-afa576788021)

![49](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e8d76a34-1668-42ae-9d25-c329c5056463)

![50](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f2067c8d-608f-4c47-9420-f6e2e1c958ba)

![51](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/afb4d71c-1560-45d6-9305-d14fb53b80fd)

![52](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d87e1d8e-1f96-4c58-93af-f2d24876805f)

![53](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/b5e192e5-81f6-4604-87ad-a63828e71d8b)

![54](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2329713b-acb0-4a99-8d6a-f58afa4c92e8)

![55](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0fbe0243-1a13-4156-a29f-1feea6868d87)

![56](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/db264d94-71a9-45d5-a587-ce3a76da8016)

![57](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/3e138277-8b39-457a-bdc9-a05ff3617d70)

![58](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d134a8db-c9c1-464c-9798-8d7429c20c48)

![59](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6c1883b0-9e6e-441f-9b94-75dac03ff65a)

![60](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/4ab4c515-afa2-411e-ac6f-fee823415b62)

![61](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6f52d947-9aac-44c6-a015-57dbd2cffc46)

![62](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e1ef4444-9fd6-450f-91e8-1599cacf25e5)

![63](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ed699b84-fd25-4a96-bd09-b8711be3d10c)

![64](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/eba9a8a4-3769-4d36-a7ed-f96b8f562094)

![65](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9572b99a-00b8-4a3a-8533-e05b5a9cbf98)

![66](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1b0a9474-c1c8-40de-bb8a-e4ee576ae2a7)

![67](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f7c41eca-6423-4839-9241-df43b48641bd)

![68](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d7e5cd98-7dd7-4c0b-8b56-6c723ed3d817)

![69](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a690e32a-cb1a-4770-a1c4-3169536a175e)

![70](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/f955373d-f638-4b99-b913-83bc07c33cbe)

![71](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a7669c9c-2655-451a-b68b-726fd0196f10)

![72](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dd5f00d5-7a30-4e28-87ed-2b12565c5feb)

![73](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/8bf25025-f02d-4fe6-88a2-f418a0059086)

![74](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c9093529-b418-4d1d-82aa-302ca2f6198c)

![75](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/aac3fb04-3e75-4954-8f37-aa3e2bdace6a)

![76](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/38a395f0-38fa-4141-bb79-39ced05fa6bd)

![77](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/68cb6cce-e574-43b4-bade-238c6265b76d)

![78](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ceb0ad54-a323-4f5d-be76-0eef9bfe2ddd)

![79](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a33385e7-dca3-4ceb-944d-c6f1dabb76f8)

![80](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cd0b6ef6-8b13-4a31-9ea3-290a5c45acba)

![81](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a5b30214-c8b8-4576-ab50-b0876e275736)
