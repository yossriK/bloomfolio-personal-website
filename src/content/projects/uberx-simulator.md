---
title: "UberX — Ride Simulation Platform"
description: "Simulating real-time ride dispatch and fleet management using Rust, NATS, Redis, and PostgreSQL."
image: "../../assets/projects/uberx-thumbnail.png"
link: "https://github.com/yossriK/UberSimX"
startDate: "2025-08"
skills:
  - Rust
  - NATS
  - Redis
  - PostgreSQL
  - WebSockets
  - Linux (WSL)
---

## Overview
UberX is a personal project simulating a ride-hailing backend system. It models drivers, riders, and ride requests in real-time to test dispatch algorithms and system behaviors, providing a realistic simulation of fleet management operations.

---

## Backend Architecture
- **Language:** Rust  
- **Architecture style:** Event-driven microservices  
- **Real-time communication:** WebSockets for driver and rider updates  
- **Message bus:** NATS for decoupled event handling between services  
- **Caching / state:** Redis for fast in-memory state management  
- **Persistence:** PostgreSQL for structured ride, driver, and rider data  
- **OS/Environment:** Linux-based development (WSL)

The backend is designed to **handle multiple concurrent ride requests** while maintaining **low-latency updates**. Services are modular, allowing independent development, testing, and future scaling.

---

## Simulation
- Simulates riders requesting rides and drivers accepting them  
- Tracks driver locations, ride states, and fleet distribution  
- Event-driven system ensures consistent simulation updates across all services  
- Designed to **stress-test dispatch logic** and system behavior under load

---

## Current Status
- Backend implemented in **Rust**, including microservices and event-driven logic  
- NATS message bus handles ride events asynchronously  
- Redis caching implemented for real-time location and ride state management  
- PostgreSQL database used for persistent storage of rides and driver info  
- WebSocket layer implemented for live updates  
- Simulation and automated tests in progress  
- Deployment on cloud is in progress  

---

## Goals & Highlights
- Build a **scalable real-time backend** capable of handling simultaneous ride requests  
- Maintain **data consistency** and low-latency updates using Redis + PostgreSQL  
- Develop **testable modules** for future authentication, deployment, and monitoring  
- Implement realistic ride-matching and fleet simulation logic  
- Demonstrate system-level thinking in **distributed event-driven systems**

---

## Technologies & Skills
- **Languages & Frameworks:** Rust  
- **Messaging / Event Handling:** NATS  
- **Databases:** Redis, PostgreSQL  
- **Real-time Protocol:** WebSockets  
- **Environment / OS:** Linux (WSL)  
- **System Design:** Event-driven microservices, modular backend architecture

---

## GitHub
[UberSimX Repository](https://github.com/yossriK/UberSimX)
