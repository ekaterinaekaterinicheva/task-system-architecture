# Project: Scalable Task Management System (TMS) Architecture

## Project Overview

**Problem:** Data overload in rapid software development.

**Consequences:** Without structured management, teams face:
- Fragmentation: Loss of project status visibility and misunderstood task dependencies.
- Productivity Collapse: Misaligned priorities leading to procrastination and missed deadlines.
- Collaboration Barriers: Inefficient communication, particularly across distributed teams and different time zones.

**Project Goal**
To architect a robust Digital Task Management System (TMS) specifically engineered for software development workflows. The system aims to restore team alignment, clarify task hierarchies, and streamline global collaboration through system design.

## Project Scope

### 1. Requirements Engineering & Interaction Modeling

- Actor-Centric Design: Identifies main roles (Project Manager and Project Employee) and defines system boundaries using UML Use Case Diagrams.
- Behavioral Dynamics: Maps the lifecycle of system events via UML Sequence Diagrams, tracking a task from creation and assignment to completion.
- State Management: Implements a UML State Machine diagram to govern task transitions, preventing invalid workflow logic.

### 2. System Architecture & Decomposition

- Modular Subsystem Design: Decomposes the system into the following subsystems using UML Component Diagrams:
    - User Management
    - Project & Task Management
    - Collaboration
    - Notification
    - Data Management.
- Hardware/Software Mapping: Bridges software and infrastructure (physical nodes) using a UML Deployment Diagram.

### 3. Object-Oriented Design (OOD)
Domain Modeling: Defines the structural organization of the system through UML Class Diagrams, identifying attributes and methods for each primary object.

Subsystem Package Design: Organizes classes into logical packages (Collaboration, Notifications, etc.) to ensure low coupling and a maintainable code base.

### 4. Security, Identity & Observability
Identity Layer: Architects a secure authentication framework using OpenID Connect (OIDC) and OAuth 2.0. Modeled the interaction between Users and the Authorization Server to ensure industry-standard security.

Global Software Control: Integrated a log-management strategy using Better Stack. Designed sequence flows for log collection, parsing into structured JSON, and real-time dashboard alerting to ensure system observability.


