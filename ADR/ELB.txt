# Amazon Elastic Load Balancer for Distributing network traffic to improve application scalability

## Status

ACCEPTED

## Context and Problem Statement

The Road Warrior Application should support 2 million active users/week and additional spikes during peak season.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to scale  appications with easy configurations 

## Decision drivers

* This is a Travel Management Application, It should be highly available, and secure
* The Application health should be monoitored continuously 

## Decision

Leverage Amazons ELB as Load Balancer

__Reasons:__ 
* Secure application with integrated certificate management, user-authentication, and SSL/TLS decryption.
* Applications can be delivered with high availability and automatic scaling.
* Health and performance of the applications can be monitored  in real time, bottlenecks can be uncovered, and SLA compliance can be maintianed.

### Consequences

* Choice of  Load Balancer: AWS offers different types of ELB's and the best one should be selected based on use case
* Health Check Latency: The time it takes to detect an unhealthy target can sometimes result in a brief period of service disruption, as traffic is not immediately diverted away from the unhealthy target.