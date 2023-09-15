# Amazon SES as Email Authentication system and Email Recieveing System

## Status

ACCEPTED

## Context and Problem Statement

The Application developed for the The Road warrior system should be able to manage Email Authentication.

### Business Assumptions

* As the development team is a new startup, there would be budget constraints and it would require a quick way to authenticate the email.
* A Light weight authentication system which can give basic email authentication.

## Decision drivers

* This is a Travel Management Application, The email data should be authentic


## Decision

Leverage Amazon SES as Email Authentication system

__Reasons:__ 

* Amazon SES supports various methods of email authentication to help verify the authenticity of your emails, which is essential for ensuring that your emails are not treated as spam or phishing attempts.

* It  has a feature called the Simple Email Service Email Receiving (Amazon SES Email Receiving) that allows you to receive emails. You can use this feature to receive incoming emails, such as user-generated content, and verify the authenticity of those incoming messages.

### Consequences

* The initial setup can involve a verification process that may take some time.
