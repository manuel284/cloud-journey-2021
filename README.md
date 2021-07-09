# cloud-journey-2021
This repo is about all the cloud-related topics I've been working on since July 1.

# Goals
- Certifications and trainings
  - Complete [Exam AZ-204: Developing Solutions for Microsoft Azure](https://docs.microsoft.com/en-us/learn/certifications/exams/az-204)
  - Participate in my employer's __Cloud Architect Program__
  - Complete Udacity's [SUSE Cloud Native Foundations Scholarship Program](https://www.udacity.com/scholarships/suse-cloud-native-foundations-scholarship)
  - Complete Udacity's [AWS Machine Learning Scholarship Program](https://www.udacity.com/scholarships/aws-machine-learning-scholarship-program)
- Books
  - [Learn Azure in a Month of Lunches](https://azure.microsoft.com/en-us/resources/learn-azure-in-a-month-of-lunches/)
  - [Azure for Architects](https://azure.microsoft.com/en-us/resources/azure-for-architects/)
  - [
The Developer’s Guide to Azure
](https://azure.microsoft.com/en-us/campaigns/developer-guide/)

# Diary
## Day 1 - July 1
- Set up this repository
- Defined above goals

## Day 2 - July 2
- AZ-204: Started learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Choose the best Azure service to automate your business processes</summary>

  - Learned about different Azure technology options (Logic Apps, Microsoft Power Automate, WebJobs, Azure Functions)
  - All four technologies can
    - accept inputs
    - can run actions
    - can include conditions
    - can produce outputs
    - can be triggered based on a schedule or by an external event
  - [How to choose a service](https://docs.microsoft.com/en-us/learn/modules/choose-azure-service-to-integrate-and-automate-business-processes/3-analyze-the-decision-criteria)
  ![How to choose a service](https://docs.microsoft.com/en-us/learn/modules/choose-azure-service-to-integrate-and-automate-business-processes/media/3-service-choice-flow-diagram.png)
    </details>

## Day 3 - July 3
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Create serverless logic with Azure Functions</summary>

  - Learned about the benefits and drawbacks of serverless compute solutions
    - \+ no need to provision VM servers
    - \+ stateless logic
    - \+ event driven
    - \- execution time
    - \- execution frequency
  - Created a function app in Azure Portal
  ![function app](screenshots/day3_function.png)
    </details>

## Day 4 - July 4
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Execute an Azure Function with triggers</summary>

  - Learned about triggers for Azure Functions
    - Types of triggers
      - Timer
      - HTTP
      - Blob
      - Queue
      - Azure Cosmos DB
      - Event Hub
    - [CRON expression](https://github.com/atifaziz/NCrontab) for a timer trigger
  - Created a function app with a timer trigger in Azure Portal
  ![function app](screenshots/day4_timertrigger.png)
  - Created a function app with a blob trigger in Azure Portal
  ![function app](screenshots/day4_blobtrigger.png)
    </details>

## Day 5 - July 5
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Chain Azure Functions together using input and output bindings</summary>

  - Learned about input and output bindings
  - Created a function app with an http trigger and a cosmos db input binding in Azure Portal
  ![function app](screenshots/day5_httptrigger_cosmosdbbinding.png)
  </details>

## Day 6 - July 6
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Create a long-running serverless workflow with Durable Functions</summary>

  - Learned about the different types of durable functions
    - Client functions
    - Orchestrator functions
    - Activity functions
  - Learned about the different applications patterns
    - Function chaining
    - Fan out/fan in
    - Async HTTP APIs
    - Monitor
    - Human interaction
  - Created a durable function
  ![durable function](screenshots/day6_durablefunction.png)
</details>

## Day 7 - July 7
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Develop, test, and publish Azure Functions by using Azure Functions Core Tools</summary>

  - Learned how to create Azure Functions locally and publish it to Azure
    - func init
    - func new
    - func start
    - func azure functionapp publish <app_name>
  ![func](screenshots/day7_func.png)
</details>

## Day 8 - July 8
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Develop, test, and deploy an Azure Function with Visual Studio</summary>

  - Learned how to create Azure Functions in Visual Studio 2019
    - Installed _ASP.NET and web development_ and _Azure development_ workloads
    - Created Function App in VS 2019
    - Tested it locally
    - Deployed it to Azure
    - Ran local unit tests
  ![func](screenshots/day8_vs.png)
  ![func](screenshots/day8_vs_publish.png)
  ![func](screenshots/day8_vs_unittests.png)
</details>

## Day 9 - July 9
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Monitor GitHub events by using a webhook with Azure Functions</summary>

  - Learned how to create a webhook to receive data from GitHub
    - Webhooks settings in GitHub
    - Securing the webhook with a secret
    - Extracting values from the webhook request
  ![func](screenshots/day9_webhook.png)
</details>
