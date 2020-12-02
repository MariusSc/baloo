# Extract
Proof of concept using various technologies, tools, patterns and practices like Microsoft Orleans, EventStoreDb, Elastic Search, Kafka, Docker, Kubernetes, .Net 5, Source Generators, Project Tye, DDD, CQRS, Keda, Event Sourcing, Azure DevOps CI/CD, ....

# Objectives
As a developer I want to deliver new features fast. I don't want to care about all the cermony that is required to build, deploy and run modern distributed (microservice based) backends. To do so, I want simple concepts at hand that are convinient to implement and covers almost all aspects to build such applications. Among that, the software development lifecycle should support having many teams working on the same application concurrently.

# Architecture requirements

1. The application should be capable to schedule background jobs
1. The application should be capable to expose the entire functionality as HTTP APIs
    - Business domain APIs
    - Application configuration APIs
    - Application maintenance APIs
1. The application should be capable of integrating 3rd party APIs
1. The application should be capable of building an auditlog for events

# Non goals/out of scope

1. Implementing (micro)services in other languages than .Net
1. User Frontends like Browser, Mobile, etc.

# Aimed non-functional requirements

1. ~10 deployments a day
1. Zero downtime upgrade deployments
1. High availiability 99,99%
1. Self scaled
1. Multitenancy ~500k tenants
1. ~10k Users per tenant
1. ~1k domain entity types
1. ~10k domain event types and versions
1. ~1k domain events/s
1. Eventual consistency to clients/consumers












