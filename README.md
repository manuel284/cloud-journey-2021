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
  ![function in visual studio](screenshots/day8_vs.png)
  ![publish from visual studio](screenshots/day8_vs_publish.png)
  ![unit tests](screenshots/day8_vs_unittests.png)
</details>

## Day 9 - July 9
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Monitor GitHub events by using a webhook with Azure Functions</summary>

  - Learned how to create a webhook to receive data from GitHub
    - Webhooks settings in GitHub
    - Securing the webhook with a secret
    - Extracting values from the webhook request
  ![webhook](screenshots/day9_webhook.png)
</details>

## Day 10 - July 10
- AZ-204: Continued learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Enable automatic updates in a web application using Azure Functions and SignalR Service</summary>

  - Learned how to use an efficient web application architecture
    - communication between server and client only happens when data has changed
    - Use Cosmos DB trigger to detect data change
    - improve response time
</details>

## Day 11 - July 11
- AZ-204: Finished learning path [Create serverless applications](https://docs.microsoft.com/en-us/learn/paths/create-serverless-applications/)
    <details>
    <summary>Module: Expose multiple Azure Function apps as a consistent API by using Azure API Management</summary>

  - Learned how to expose an Azure Function as an API to Azure API Management
    - from the Function
    - from API Management
  - Learned about the benefits of using Azure API Management
    - Client apps are coupled to the exposed API, not the backend. This allows us to update the backend without impacting the client app.
    - We can make our APIs consistent, e.g. by transforming XML to JSON.
    - Enforce security requirements with policies
  ![apim](screenshots/day11_apim.png)
</details>

## Day 12 - July 12
- AZ-204: Started learning path [Connect your services together
](https://docs.microsoft.com/en-us/learn/paths/connect-your-services-together/)
    <details>
    <summary>Module: Choose a messaging model in Azure to loosely connect your services</summary>

  - Learned about communication strategies
    - Messages
      - contains raw data
      - contains the data itself, not a reference
      - the sender expects the receiver to process the message in a certain way
    - Events
      - publisher and receiver
      - broadcast communications
      - lightweight notification
      - can have 0,n receivers
      - "fan out"
  - Learned about different messaging models
    - Storage queue
    - Event Grid
    - Event Hubs
    - Service Bus
</details>

## Day 13 - July 13
- AZ-204: Continued learning path [Connect your services together
](https://docs.microsoft.com/en-us/learn/paths/connect-your-services-together/)
    <details>
    <summary>Module: Implement message-based communication workflows with Azure Service Bus</summary>

  - Learned when to choose Service Bus queues, topics, or relays
    - Queue
      - one sender, one receiver
      - FIFO
      - max. message size: 64 KB
    - Topic
      - similar to a queue but with multiple receivers  
    - Relay
      - direct communication between two partners
  - Configured and Azure Service Bus namespace
  - Created a Service Bus topic
  - Created a Service Bus queue
  ![azure service bus](screenshots/day13_azureservicebus.png)
</details>

## Day 14 - July 14
- AZ-204: Continued learning path [Connect your services together
](https://docs.microsoft.com/en-us/learn/paths/connect-your-services-together/)
    <details>
    <summary>Module: Communicate between applications with Azure Queue storage 1/x</summary>

  - Learned about Azure Queue storage
    - 1,n senders/receivers
    - requires Azure general-purpose storage accounts (v1 or v2)
  - Created an Azure Queue storage and send/received messages    
</details>

## Day 15 - July 15
- AZ-204: Continued learning path [Connect your services together
](https://docs.microsoft.com/en-us/learn/paths/connect-your-services-together/)
    <details>
    <summary>Module: Enable reliable messaging for Big Data applications using Azure Event Hubs</summary>

  - Created an EventHub using Azure CLI
  - Send/received messages through an Event Hub
  - Evaluated the performance in Azure Portal
</details>
