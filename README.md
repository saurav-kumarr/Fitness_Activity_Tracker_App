# Fitness_Activity_Tracker_App



1️⃣ Fitness Activity Tracker built using Spring Boot Microservices, featuring AI-driven recommendations, OAuth2 authentication with Keycloak, and a React + Redux frontend.



2️⃣ 🏃‍♂️ Fitness Activity Tracker – Microservices Architecture

A scalable Fitness Activity Tracker application developed using Spring Boot Microservices that enables users to log fitness activities, manage profiles, and receive AI-powered fitness recommendations.

The system is composed of independent services including User Service, Activity Service, and AI Recommendation Service, all registered with Eureka Service Discovery and centrally managed via a Spring Cloud Config Server.
An API Gateway handles routing and security, while Keycloak (OAuth 2.0 PKCE flow) ensures secure authentication and authorization.

The application uses RabbitMQ for asynchronous event-driven communication between services.
AI-based insights and personalized recommendations are generated using the Gemini API.
A modern React + Redux frontend provides login, activity tracking, dashboards, and detailed views with complete end-to-end integration.

Key Features:

Microservices-based architecture

Secure OAuth 2.0 authentication with Keycloak

AI-driven workout recommendations

Event-driven communication using RabbitMQ

Centralized configuration & service discovery

Fully integrated React frontend

Tech Stack:
Spring Boot, Spring Cloud, Eureka, Config Server, API Gateway, Keycloak, OAuth 2.0, RabbitMQ, Gemini API, React, Redux, MySQL/PostgreSQL





3️⃣ Architecture Overview:

Frontend (React + Redux)
Handles user authentication, activity submission, and dashboards using secured APIs.

API Gateway
Acts as a single entry point, enforces security via Keycloak, and routes requests to microservices.

Keycloak
Provides OAuth 2.0 PKCE-based authentication and user identity management.

Eureka Server
Enables service discovery for all microservices.

Config Server
Centralized configuration management for all services.

User Service
Manages user profiles and Keycloak user mapping.

Activity Service
Stores and processes fitness activities and publishes events to RabbitMQ.

AI Service
Consumes activity events asynchronously and generates fitness recommendations using Gemini API.

RabbitMQ
Facilitates asynchronous, event-driven communication between services.

This architecture ensures scalability, loose coupling, fault tolerance, and easy extensibility.
