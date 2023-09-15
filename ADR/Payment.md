# Stripe as Payemnt Service

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to integrate with Payment Service without any hassle

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to configure the Payment Gateway and it should be one time and commission based transaction fee.

## Decision drivers

* This is a Travel Management Application, and it would require a quick way to configure the  Payment Gateway.

## Decision

Leverage Stripe as Payemnt Service

__Reasons:__ 

* Stripe is a popular payment processing platform that offers competitive pricing, especially for online businesses. It provides a straightforward fee structure and allows you to accept various payment methods, including credit and debit cards, ACH transfers, and more.

### Consequences

* Supported in some of the countries, we may have to switch the service based on region , during internationalization.
