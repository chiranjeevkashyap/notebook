# Spring Boot Cohort

## Table of Contents
- [Application Properties](#basic-application-properties)
- [Module 12](#module-12-introduction-to-microservice-architecture)
    - [Module 12.1](#121-introduction-to-the-microservice-architecture)
    - [Module 12.2](#122-setting-up-the-inventory-management-system)

## Basic Application Properties

| property | used for |
| --- | --- |
| `spring.application.name` | |
| `spring.main.banner-mode` | |
| `spring.datasource.url` | |
| `spring.datasource.username` | |
| `spring.datasource.password` | |

## Module 12: Introduction to Microservice Architecture


### 12.1 Introduction to the Microservice Architecture

Microservices are an architectural style where applications are developed as a collection of small, loosely coupled, independently deployable services.

Characteristics of Microservices
 - Small, focused on doing one thing well
 - Independently deployable
 - Organized around business capabilities
 - Decentralized data management
 - Communication via lightweight protocols (typically HTTP/REST)

Comparison with Monolith
 - Monolith: tightly coupled, single codebase
 - Microservices: loosely, coupled, multiple independent services

Challenges of Microservices
 - Increased complexity in managing microservices
 - Distributed System issues like Latency, Load Balancing, network reliability and consistency
 - Managing transactions and consistency across services
 - Handling communication protocols (REST, gRPC, messaging)
 - Monitoring and Logging needs centralized monitoring and logging solutions

Why use Microservices
 - Scale services independently based on demand (e.g., scale only payment service during high traffic)
 - Services can be written in different programming languages, suited to specific tasks
 - Small team can work on different services simultaneously, reducing time to market
 - Failure in one service doesn't bring down the entire system
 - Each service can be updated, deployed and scaled independently
 - Teams can work on different services without affecting each other

### 12.2 Setting up the Inventory Management System

Return to [Table of Content](#table-of-contents) or [Top](#spring-boot-cohort)