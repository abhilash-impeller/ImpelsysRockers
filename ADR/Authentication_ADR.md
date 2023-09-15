# Amazon Cognito and Amazon Web Identity Federation as Registration and Authentication system and Social Integration

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to manage User Authentication and be able to scale at capacity.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to authenticate the users.
* A Light weight authentication system which can give basic authentication and must be able to scale to high usages.

## Decision drivers

* This is a Travel Management Application, The data should be highly available and reliable
* The Application and the data should be secured
* The Application should be fault tolerant

## Decision

Leverage Amazon Cognito as Registration and Authentication system
Levearge Amazon Web Identity Federation for Social Integration

__Reasons:__ 

* Deliver frictionless customer identity and access management (CIAM) with a cost-effective and customizable service and relatively simple and inexpensive and pay as you go.
* Add security features such as adaptive authentication, support compliance, and data residency requirements.
* Scale to millions of users with a fully managed, high-performant, and reliable identity store.
* Federate sign-in using OIDC or SAML 2.0 and connect to a broad group of AWS services and products.

### Consequences

* Complexity-AWS Cognito offers a wide range of features, including user management, authentication, authorization, and synchronization with social identity providers. This complexity can make it challenging to set up and configure correctly, especially for developers who are new to the service.

* Regional Availability:AWS Cognito is not available in all AWS regions, which may limit your deployment options depending on your geographical needs.