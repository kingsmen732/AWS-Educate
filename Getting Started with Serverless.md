## Session Questions and Answers

### 1. Which of the following are serverless benefits? (Select THREE.)
- **High availability**
- **No server management**
- **Continuous scaling**

### 2. Which is a feature of Amazon CloudFront that lets you run code closer to users of your application, which improves performance and reduces latency?
- **Lambda@Edge**

### 3. Which AWS Service allows you to create, publish, maintain, monitor, and secure APIs? These APIs act as "front doors" for your applications.
- **Amazon API Gateway**

### 4. Which of the following statements about invocation models are correct? (Select THREE.)
- **When Alexa is the event source, Lambda makes three attempts to invoke the function before putting the failed invocation into the dead letter queue (DLQ).**
- **Amazon SQS triggers Lambda using the polling invocation model.**
- **Amazon API Gateway triggers Lambda synchronously.**

### 5. Which of the following IAM entities must be included in an execution role for a Lambda function to interact with other services, such as DynamoDB? (Select TWO.)
- **IAM policy that defines the actions that can be taken within DynamoDB**
- **Trust policy that grants "AssumeRole" permission to Lambda to act on DynamoDB**

### 6. Which would you use to analyze details about an invocation to look for a bottleneck?
- **AWS X-Ray**

### 7. What does an AWS Identity and Access Management (IAM) resource-based policy control?
- **What the other AWS services can do when processing the events**

### 8. What is the importance of the IAM execution role?
- **Gives your function permissions to interact with other services**

### 9. Which of the following patterns are Lambda invocation models? (Select THREE.)
- **Asynchronous**
- **Synchronous**
- **Polling**

### 10. Which of the following are reasons a developer would set a concurrency limit (or reserve) on a function? (Select THREE.)
- **To manage costs**
- **To regulate how long it takes to process a batch of events**
- **To match the limit with a downstream resource**

