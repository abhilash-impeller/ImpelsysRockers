# Amazon Simple Queue Service (SQS), CloudWatch Events and AWS Step Function to  consume and poll events into the system from Thirdparty

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to consume and poll events into the system from Thirdparty

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to consume and poll events into the system from Thirdparty

## Decision drivers

* This is a Travel Management Application, and it would require a quick way to consume and poll events into the system from Thirdparty

## Decision

Leverage Amazon Simple Queue Service (SQS), CloudWatch Events and AWS Step Function to  consume and poll events into the system from Thirdparty

__Reasons:__ 

* Amazon SQS is a fully managed message queuing service that allows you to decouple the components of a cloud application. While SQS is more commonly associated with message-driven, event-driven processing, you can use it to implement timer polling-based queues by having your worker processes poll the queue at regular intervals.
* CloudWatch Events is a service that allows you to set up scheduled rules to trigger actions at specified times or intervals. You can create a scheduled rule to invoke an AWS Lambda function or an AWS Step Functions state machine to poll a queue periodically.
* AWS Step Functions is a serverless orchestration service that allows you to coordinate multiple AWS services into serverless workflows. You can use Step Functions to create complex workflows that involve polling a queue (e.g., SQS) at specific intervals.

### Consequences

* Operational Overhead and learning curve involved in using these services
