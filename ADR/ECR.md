
# Amazon Elastic Container Registry for deploying container software

## Status

ACCEPTED

## Context and Problem Statement

The containerized app developed for the The Road warrior system should be stored and deplopyed on a secure container registry.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to store containerized appications with easy configurations 

## Decision drivers

* This is a Travel Management Application, It should be highly available, and secure
* The Application and the data should be secured

## Decision

Leverage Amazons ECR as Container registry

__Reasons:__ 
* Container images can be pushed to Amazon ECR without installing or scaling infrastructure, and images can be pulled using any management tool.
* Images can be shared and downloaded securely over Hypertext Transfer Protocol Secure (HTTPS) with automatic encryption and access controls.
* Images can be Accessed and distributed faster, download times  reduced, and availability can be improved using a scalable, durable architecture.

### Consequences

* Network Latency: Accessing container images in ECR from regions different from where the images are stored can introduce network latency, which may affect application startup times and overall performance.
* ECR is tightly integrated with other AWS services like Amazon ECS (Elastic Container Service) and AWS Fargate. If you decide to migrate your containers to a different cloud provider or container orchestration platform, you may need to refactor your container deployment and image registry strategy* Complexity:Managing EC2 instances requires a certain level of expertise. Choosing the right EC2 instance type can be challenging
