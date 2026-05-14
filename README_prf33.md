# Hi, I'm Mostafa Alaa 👋

I'm a software engineer based in Egypt, focused on backend architecture and distributed systems. My background is unconventional — accounting degree, then several years of building the engineering foundation myself through real projects. No bootcamp shortcut, just a lot of time with docs, broken builds, and systems that gradually stopped breaking.

What I care about most is getting the architecture right: clean domain models, systems that handle failure gracefully, and code the next developer can actually maintain.

---

## Tech Stack

### Languages
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=csharp&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=for-the-badge&logo=JavaScript&logoColor=black)

### Backend
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-5C2D91?style=for-the-badge&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-000000?style=for-the-badge&logo=dotnet&logoColor=white)

### Databases & Messaging
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-D82C20?style=for-the-badge&logo=redis&logoColor=white)

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![TanStack](https://img.shields.io/badge/TanStack-000000.svg?style=for-the-badge&logo=TanStack&logoColor=white)

### DevOps & Tools
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## Projects

### [Metriflow](https://github.com/mustaphaAlaa/Metriflow) — Event-Driven Analytics Pipeline
*Jan 2026*

An end-to-end ETL pipeline that ingests high-volume event data, processes it through asynchronous worker stages, and exposes aggregated insights via a secured REST API.

- Designed a seven-stage aggregation pipeline (Raw → Staged → Page → Daily → Time Interval → Monthly → Yearly), each stage powered by a dedicated background worker service communicating over RabbitMQ.
- Processed **26 million records in under 3 minutes** using Producer–Consumer channels, streaming JSON deserialisation, and `SqlBulkCopy` at 250K records per batch.
- Optimised database performance with columnstore indexes, stored procedures with ACID transactions, and workload-specific use of ADO.NET and EF Core.
- Handled late-arriving and duplicate events by recomputing affected aggregates to maintain pipeline consistency.
- Used Redis for arbitrary date-range queries outside pre-aggregated boundaries.
- Fully containerised with Docker Compose; CI/CD via GitHub Actions; unit tests covering core aggregation logic.

---

### [Kemet](https://github.com/MustaphaAlaa) — E-Commerce Platform *(Freelance)*
*Apr 2025 – Aug 2025 · Feb 2026 – Apr 2026*

A production-ready e-commerce system built to replace a manual, spreadsheet-based order workflow with a proper integrated platform.

- Architected the full system using Clean Architecture with clear separation across domain, application, infrastructure, and presentation layers.
- Built a multi-role auth system with JWT, refresh tokens, and ASP.NET Identity — extended with a custom resource-authorisation layer that verifies both role *and* ownership on every request, preventing IDOR and privilege escalation by design, not convention.
- Modelled a 6-stage order fulfilment pipeline and a 7-state seller subscription lifecycle, with optimistic locking for concurrent writes and a deferred stock-deduction model to prevent inventory abuse.
- Delivered a fully type-safe React/TypeScript frontend using TanStack Query with a Context Endpoint Pattern aligned to backend auth boundaries.
- Added rate limiting, structured logging via Serilog, Docker/Docker Compose setup, and CI/CD with GitHub Actions.
- Codebase delivered production-ready; project paused at client direction.

---

### [Hyper JSON Generator](https://github.com/MustaphaAlaa/HyperJSONGenerator) — High-Performance Data Generator
*Dec 2025*

A .NET console application for generating millions of structured records used to load-test the Metriflow pipeline.

- Implemented streaming JSON generation with `Utf8JsonWriter` to write records incrementally without loading datasets into memory.
- Reduced allocations by switching from class-based objects to CPU-cache-efficient structs, replacing string identifiers with compact enum values and tick-based timestamps.
- Eliminated `OutOfMemoryException` errors during large dataset generation and improved stability under sustained high-volume output.

---

### [GovConnect](https://github.com/MustaphaAlaa) — Government Services Backend
*Feb 2025*

A backend system for managing driver, vehicle, and licence data, built with ASP.NET Core and EF Core.

- Applied layered architecture with Dependency Injection and the Repository Pattern.
- Implemented role-based access control across Admin, Employee, and User roles.
- Developed licence issuance triggered through publish–subscribe event logic; validated data with custom validators and SQL Server constraints.
- Wrote unit tests covering core services to support reliability and future refactoring.

---

## What I'm Interested In

Backend architecture and distributed systems are where I go deepest, but I'm genuinely interested in the full picture — from domain modelling and API design to database performance, event-driven processing, and auth systems that are secure by construction rather than by policy. I also build complete frontends when the project needs it.

---

## Background

B.Com. in Accounting, Helwan University (2017–2021). In 2023 I committed to software engineering full-time through self-directed study — data structures, algorithms, C#, backend architecture, relational databases, React, and TypeScript — applied through progressively complex, production-grade projects.

Everything here reflects work I've actually shipped. Building real systems with real constraints teaches things that nothing else does.

---

## Open To

I'm open to any software engineering role where the work is meaningful and the team cares about doing things properly — full-time, freelance, or contract, remote or Egypt-based.

- Backend / .NET Engineering Roles
- Full-Stack Development
- Data Engineering & High-Throughput Systems
- API & Platform Engineering
- Open Source Collaboration

---

## Connect

📫 mostafaalaa11998@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/mostafa-a-75b323120) · [GitHub](https://github.com/MustaphaAlaa)
