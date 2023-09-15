# Amazon Machine Learning Offerings to provide a pre trained Email Filter

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to filter Travel related Email(Spam/Ham).

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to configure the pre trained custom ML Model.

## Decision drivers

* This is a Travel Management Application, and it would require a quick way to configure the pre trained custom ML Model.

## Decision

Leverage Amazon ML Offerings to provide a pre trained Email Filter

__Reasons:__ 

* AWS ML Offerings provide comprehensive machine learning platform that allows you to build, train, and deploy custom machine learning models. While it provides tools and infrastructure for custom model development, it also offers built-in algorithms and pre-trained models to accelerate the development process. SageMaker includes built-in algorithms for common tasks like classification, regression, clustering, and more.

### Consequences

* While these services provide pre-trained models and tools to simplify machine learning tasks, you may still need to fine-tune models or customize them further to suit your specific requirements
