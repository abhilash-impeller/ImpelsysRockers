# AWS Lambda as compute engine

## Status

ACCEPTED

## Context and Problem Statement

The Scraping services developed for the The Road warrior system should be deplopyed on a pay as you use compute capacity in the cloud. We should be able to Run code without thinking about servers or clusters

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to deploy the appications with easy configurations to scale 

## Decision drivers

* This is a Travel Management Application, It should be highly available, performant and reliable
* Scrapping Service has some ML Ops involved
* The Application and the data should be secured

## Decision

Leverage Amazons Lambda as compute capacity to support any workload

__Reasons:__ 
* Automatically respond to code execution requests at any scale, from a dozen events per day to hundreds of thousands per second.
* Save costs by paying only for the compute time you use—by the millisecond—instead of provisioning infrastructure upfront for peak capacity.
* Optimize code execution time and performance with the right function memory size. Respond to high demand in double-digit milliseconds with Provisioned Concurrency.

### Consequences

* Cold Starts: Lambda functions can experience cold starts, which result in increased latency for the first invocation of a function after it has been idle
* Execution Time Limits: Lambda functions have execution time limits (e.g., 15 minutes per execution for the default limit)
* Statelessness: Lambda functions are designed to be stateless, which means they do not retain state between invocations.
* No Persistent Storage: Lambda itself does not provide persistent storage. You may need to use other AWS services like Amazon S3 or Amazon RDS to store data between function invocations.