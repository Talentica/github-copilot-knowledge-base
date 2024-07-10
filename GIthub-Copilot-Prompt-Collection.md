Prompt for generating controllers.
----------------------------------

Generate a controller class as specified below.

*   Create a nestjs controller to update repayment entity createdBy and frequency columns.
    
*   Generate controller script by taking reference from file mandate-creation.controller.ts.
    
*   Also consider a swagger documentation implementation as specified in mandate-creation.controller.ts.
    

![image-20240529-032138.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-032138.png?version=1&modificationDate=1716952900740&cacheVersion=1&api=v2&width=758 "Digital Lending > Github Copilot Prompt collection > image-20240529-032138.png")

Prompt for service file code generation.
----------------------------------------

Generate a service class as specified below

*   Should update createdBy and frequency in the repayment table.
    
*   Update createdBy with light\_system where repayment type is automatic and partner where repayment type is manual.
    
*   Update frequency as recurring where repayment type is automatic and adhoc where repayment type is manual.
    

![image-20240529-033309.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-033309.png?version=1&modificationDate=1716953590914&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240529-033309.png")![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_7_for_29884483.png?version=1&modificationDate=1716288211111&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > att_7_for_29884483.png")

Prompt for generating db repository functions:
----------------------------------------------

Ex 1: Create a function which take status and date as input and return the repayments with the given status and scheduledAt as the given date b/w 00 hours to 23 hours.

![image-20240529-033531.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-033531.png?version=1&modificationDate=1716953733167&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240529-033531.png")

Ex 2:   Create a function to get all the repayments with status as DRAFTED and update them with status cancelled

![image-20240529-033700.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-033700.png?version=1&modificationDate=1716953822656&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240529-033700.png")

Ex 3: create a function to modify the createdBy of repayments in which created at it between 5 am to 8 am to LIGHT\_SYSTEM .

![image-20240529-034014.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-034014.png?version=1&modificationDate=1716954015731&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240529-034014.png")

Prompt for calling third party service
--------------------------------------

Ex: call third party service to send a notification that we updated status of repayments using axios handle proper error handling

![image-20240529-034333.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240529-034333.png?version=1&modificationDate=1716954215329&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240529-034333.png")

Prompt for generate smaller utils:
----------------------------------

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_6_for_29884483.png?version=1&modificationDate=1716288211018&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_6_for_29884483.png")

Ex 2: Update all empty createdBy in repayments where repayment.type === RepaymentType.AUTOMATIC add createdBy = RepaymentInitiator.LIGHT\_SYSTEM else RepaymentInitiator.PARTNER, do it most optimised way.

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_3_for_29884483.png?version=1&modificationDate=1716288210967&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_3_for_29884483.png")

Ex: 3

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_4_for_29884483.png?version=1&modificationDate=1716288211024&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_4_for_29884483.png")

Results:

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_5_for_29884483.png?version=1&modificationDate=1716288211084&cacheVersion=1&api=v2&width=682 "Digital Lending > Github Copilot Prompt collection > att_5_for_29884483.png")

Prompt for generating scripts.
------------------------------

Ex: Create a nestjs command to update repayment entity createdBy and frequency columns. Generate command script by taking reference from file generate-loan-expirydate-command.ts

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_11_for_29884483.png?version=1&modificationDate=1716288211352&cacheVersion=1&api=v2&width=756 "Digital Lending > Github Copilot Prompt collection > att_11_for_29884483.png")

Use copilot as a search engine
------------------------------

Input Prompt:

// Give me commands to push the changes to the remote repository  

Response:

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_1_for_29884483.png?version=1&modificationDate=1716288210897&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_1_for_29884483.png")

Use of Github copilot chat feature
----------------------------------

Chat Prompt:

Modify below loop like that , if frequency is empty then add frequency= 'RECURRING' in automatic repayment case , and frequency = 'ADHOC' in manual repayment case.

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_10_for_29884483.png?version=1&modificationDate=1716288211380&cacheVersion=1&api=v2&width=476 "Digital Lending > Github Copilot Prompt collection > att_10_for_29884483.png")![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_9_for_29884483.png?version=1&modificationDate=1716288211242&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_9_for_29884483.png")

Generate Unit test:
-------------------

Ex: Generate unit tests covering all positive and negative scenarios , including edge cases. use reference of create-first-repayment-request-event-handler-service.spec.ts as correct example and generate accordingly, make sure you generate providers as same format as in create-first-repayment-request-event-handler-service.spec.ts. Cover all code execution flows for maximum coverage.

![](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/att_8_for_29884483.png?version=1&modificationDate=1716288211029&cacheVersion=1&api=v2&width=612 "Digital Lending > Github Copilot Prompt collection > att_8_for_29884483.png")

Writing regular expressions
---------------------------

Working with regular expressions can be challenging and confusing at times. However, GitHub Copilot can help in simplifying the process of writing regular expressions. it is crucial to adjust and test the generated regular expressions according to your specific requirements and the programming language you are utilizing.

![1_7aCn5lr50GGZ66RwvNfdDg.gif](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/1_7aCn5lr50GGZ66RwvNfdDg.gif?version=1&modificationDate=1716952580187&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > 1_7aCn5lr50GGZ66RwvNfdDg.gif")

Writing sql queries
-------------------

GitHub Copilot understands the syntax and context of SQL code. You should keep related entity files open and write a prompt with context about what you want to achieve with the SQL query.

![1_qwbxARk7vjylKOmWSkMIpQ.gif](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/1_qwbxARk7vjylKOmWSkMIpQ.gif?version=1&modificationDate=1716952580209&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > 1_qwbxARk7vjylKOmWSkMIpQ.gif")

Writing Commands
----------------

You can use GitHub Copilot for finding the command you’re looking for. You can use code comments to find the command. Also as you begin typing the initial part of the command, GitHub Copilot analyses the context and generates relevant suggestions, and completes the command for you. For instance, This feature proves particularly helpful when you’re learning or writing Git commands.

![1_mZ0SA5scA7TOw1bTuYbn2A.gif](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/1_mZ0SA5scA7TOw1bTuYbn2A.gif?version=1&modificationDate=1716952580218&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > 1_mZ0SA5scA7TOw1bTuYbn2A.gif")

Prompt for writing entity
-------------------------

Prompt : Generate payment type entity with columns of id (auto increment int), finfluxTypeId (string) , name (string) with reference of repayment.entity.ts . Also create a builder class.

![image-20240701-094037.png](https://light-microfinance-pvt-ltd.atlassian.net/wiki/download/thumbnails/29884483/image-20240701-094037.png?version=1&modificationDate=1719826839989&cacheVersion=1&api=v2&width=760 "Digital Lending > Github Copilot Prompt collection > image-20240701-094037.png")
