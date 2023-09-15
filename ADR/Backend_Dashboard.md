# AWS Aurora, Amazon EC2 ,S3 , ECR , EKS and Amazon Elastic Load Balancer  for Back End hosting  Deployment.

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to manage Back end deployment.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to configure and deploy the Back end module.
* Use seperate module for front end and Back end.

## Decision drivers

* Use seperate module for front end and Back end.

## Decision

Leverage AWS Aurora, Amazon EC2 ,S3 , ECR , EKS and Amazon Elastic Load Balancer  for Back End hosting  Deployment.

__Reasons:__ 

* Deliver secure, reliable, high-performance, and cost-effective compute infrastructure to meet demanding business needs.
* Deliver the broadest choice of compute, networking (up to 400 Gbps), and storage services purpose-built to optimize price performance for ML projects.
* Scale at capacity within minutes with SLA commitment of 99.99% availability.
* Secure application with integrated certificate management, user-authentication, and SSL/TLS decryption.
* Applications can be delivered with high availability and automatic scaling.
* Health and performance of the applications can be monitored  in real time, bottlenecks can be uncovered, and SLA compliance can be maintianed.
* Container images can be pushed to Amazon ECR without installing or scaling infrastructure, and images can be pulled using any management tool.
* Images can be shared and downloaded securely over Hypertext Transfer Protocol Secure (HTTPS) with automatic encryption and access controls.
* Images can be Accessed and distributed faster, download times  reduced, and availability can be improved using a scalable, durable architecture.


### Consequences

* Complexity of configuring  and special attention towards security.
* Operational Overhead: We are responsible for managing the operating system, patching, security updates, and backups. This can be a significant burden, especially for small teams with limited resources.
* Network Latency: Accessing container images in ECR from regions different from where the images are stored can introduce network latency, which may affect application startup times and overall performance.
* ECR is tightly integrated with other AWS services like Amazon ECS (Elastic Container Service) and AWS Fargate. If you decide to migrate your containers to a different cloud provider or container orchestration platform, you may need to refactor your container deployment and image registry strategy* Complexity:Managing EC2 instances requires a certain level of expertise. Choosing the right EC2 instance type can be challenging
