Prompt for generating controllers.
----------------------------------

Generate a controller class as specified below.

- Create a nestjs controller to update repayment entity createdBy and frequency columns.
- Generate controller script by taking reference from file mandate-creation.controller.ts.
- Also consider a swagger documentation implementation as specified in mandate-creation.controller.ts.
    ![image-20240529-032138](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/ecd86543-6b37-45ec-9d8a-ffa72eb95c40)


Prompt for service file code generation.
----------------------------------------

Generate a service class as specified below

- Should update createdBy and frequency in the repayment table.  
- Update createdBy with light\_system where repayment type is automatic and partner where repayment type is manual.  
- Update frequency as recurring where repayment type is automatic and adhoc where repayment type is manual.

![image-20240529-033309](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/827e751e-b842-4d2f-967c-60856657f0dc)

![att_7_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/6b277ddd-d5eb-4f9c-abd6-e2361dc5a386)


Prompt for generating db repository functions:
----------------------------------------------

Ex 1: Create a function which take status and date as input and return the repayments with the given status and scheduledAt as the given date b/w 00 hours to 23 hours.

![image-20240529-033531](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/274d3e28-7fe2-4ddb-87de-c7f0cfa6e029)


Ex 2:   Create a function to get all the repayments with status as DRAFTED and update them with status cancelled
![image-20240529-033700](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/861e2c31-75ab-4785-a71e-9878e5588815)


Ex 3: create a function to modify the createdBy of repayments in which created at it between 5 am to 8 am to LIGHT\_SYSTEM .

![image-20240529-034014](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/b7667322-e374-4e67-b256-daae79d22f9e)


Prompt for calling third party service
--------------------------------------

Ex: call third party service to send a notification that we updated status of repayments using axios handle proper error handling

![image-20240529-034333](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/08ce1294-8595-487b-b81c-c04e1cb80bfe)


Prompt for generate smaller utils:
----------------------------------

![att_6_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/5f5efae3-dad6-40d7-bdc2-7ab43c0a394e)


Ex 2: Update all empty createdBy in repayments where repayment.type === RepaymentType.AUTOMATIC add createdBy = RepaymentInitiator.LIGHT\_SYSTEM else RepaymentInitiator.PARTNER, do it most optimised way.

![att_3_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/beb59093-b346-4256-baa4-e6b1718d88be)


Ex: 3

![att_4_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/0adbdd45-a464-4d4c-983d-a6d676d1ad71)


Results:

![att_5_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/699e662c-8bd3-4c68-8205-97731e3d57f8)


Prompt for generating scripts.
------------------------------

Ex: Create a nestjs command to update repayment entity createdBy and frequency columns. Generate command script by taking reference from file generate-loan-expirydate-command.ts

![att_11_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/965e248b-f411-4db0-9d47-224b29b836ab)


Use copilot as a search engine
------------------------------

Input Prompt:

```
// Give me commands to push the changes to the remote repository  
```

Response:

![att_1_for_29884483 (1)](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/be244705-bd06-4da4-895b-d322066372ac)


Use of Github copilot chat feature
----------------------------------

Chat Prompt:

Modify below loop like that , if frequency is empty then add frequency= 'RECURRING' in automatic repayment case , and frequency = 'ADHOC' in manual repayment case.

![att_10_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/9bafbc2a-65f6-41d3-9315-5e5f516b208f)

![att_9_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/f127cfaa-8d9e-4289-9f15-e27ef2aed734)

Generate Unit test:
-------------------

Ex: Generate unit tests covering all positive and negative scenarios , including edge cases. use reference of create-first-repayment-request-event-handler-service.spec.ts as correct example and generate accordingly, make sure you generate providers as same format as in create-first-repayment-request-event-handler-service.spec.ts. Cover all code execution flows for maximum coverage.

![att_8_for_29884483](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/981a7c82-a402-40cd-80c9-45ef4e5b46a5)


Writing regular expressions
---------------------------

Working with regular expressions can be challenging and confusing at times. However, GitHub Copilot can help in simplifying the process of writing regular expressions. it is crucial to adjust and test the generated regular expressions according to your specific requirements and the programming language you are utilizing.

![1_7aCn5lr50GGZ66RwvNfdDg](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/7d4d56db-c031-4e4b-bc1c-d3854eb8701a)


Writing sql queries
-------------------

GitHub Copilot understands the syntax and context of SQL code. You should keep related entity files open and write a prompt with context about what you want to achieve with the SQL query.

![1_qwbxARk7vjylKOmWSkMIpQ](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/9016d4fa-15b1-43a3-b051-429b96af199f)


Writing Commands
----------------

You can use GitHub Copilot for finding the command you’re looking for. You can use code comments to find the command. Also as you begin typing the initial part of the command, GitHub Copilot analyses the context and generates relevant suggestions, and completes the command for you. For instance, This feature proves particularly helpful when you’re learning or writing Git commands.


![1_mZ0SA5scA7TOw1bTuYbn2A](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/89f4136c-f2fd-4281-90c0-b546c9f986b6)

Prompt for writing entity
-------------------------

Prompt : Generate payment type entity with columns of id (auto increment int), finfluxTypeId (string) , name (string) with reference of repayment.entity.ts . Also create a builder class.

![image-20240701-094037](https://github.com/Talentica/github-copilot-knowledge-base/assets/109061225/46b4792a-1133-4cf9-89ce-f543172ab374)
