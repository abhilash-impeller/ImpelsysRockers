# AWS EC2 as compute engine

## Status

ACCEPTED

## Context and Problem Statement

The backend services developed for the The Road warrior system should be deplopyed on a secure, resizable compute capacity in the cloud. It should be highly available, reliable and scale on Demand.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to deploy the appications with easy configurations to scale 

## Decision drivers

* This is a Travel Management Application, It should be highly available, performant and reliable
* Reccomendation/ Scrapping Service has some ML Ops involved
* The Application and the data should be secured

## Decision

Leverage Amazons EC2 as compute capacity to support any workload

__Reasons:__ 
* Deliver secure, reliable, high-performance, and cost-effective compute infrastructure to meet demanding business needs.
* Deliver the broadest choice of compute, networking (up to 400 Gbps), and storage services purpose-built to optimize price performance for ML projects.
* Scale at capacity within minutes with SLA commitment of 99.99% availability.

### Consequences

* Operational Overhead: We are responsible for managing the operating system, patching, security updates, and backups. This can be a significant burden, especially for small teams with limited resources.
* EC2, doesn't guarantee 100% uptime. We need to architect their applications for high availability if they require it.
* Complexity:Managing EC2 instances requires a certain level of expertise. Choosing the right EC2 instance type can be challenging
* Manual Scaling: EC2 instances need to be manually scaled up or down based on demand. 
