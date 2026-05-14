# Mostafa Alaa — .NET Backend Developer

I'm a software engineer based in Egypt, focused on backend architecture and distributed systems. My background is unconventional — I studied accounting, then spent several years building the engineering foundation myself, working through real projects until the skills were solid enough to ship production systems.

What I care about most is getting the architecture right: clean domain models, systems that handle failure gracefully, and code that the next developer can actually maintain.

---

## Technical Skills

| Area | Technologies |
|---|---|
| **Core** | C#, ASP.NET Core, Web API, Background Services |
| **Databases** | SQL Server, PostgreSQL |
| **Messaging & Caching** | RabbitMQ, Redis |
| **Frontend** | React, TypeScript, Tailwind CSS |
| **DevOps** | Docker, Docker Compose, GitHub Actions |
| **Testing** | xUnit, Moq |
| **Practices** | Clean Architecture, SOLID, REST API design, Serilog, Git |

---

## Selected Projects

### [Metriflow](https://github.com/MostafaAlaa) — Event-Driven Analytics Pipeline
*Jan 2026*

An end-to-end ETL pipeline built to ingest high-volume event data and expose aggregated insights through a secured REST API.

- Designed a seven-stage aggregation pipeline (Raw → Staged → Page → Daily → Time Interval → Monthly → Yearly), each stage powered by a dedicated background worker service communicating over RabbitMQ.
- Processed **26 million records in under 3 minutes** using Producer–Consumer channels, streaming JSON deserialisation, and `SqlBulkCopy` at 250K records per batch.
- Optimised database performance with columnstore indexes, stored procedures with ACID transactions, and workload-specific use of ADO.NET and EF Core.
- Handled late-arriving and duplicate events by recomputing affected aggregates to maintain pipeline consistency.
- Used Redis for arbitrary date-range queries outside pre-aggregated boundaries.
- Fully containerised with Docker Compose; CI/CD via GitHub Actions; unit tests covering core aggregation logic.

---

### [Kemet](https://github.com/MostafaAlaa) — E-Commerce Platform *(Freelance)*
*Apr 2025 – Aug 2025 · Feb 2026 – Apr 2026*

A production-ready e-commerce system built to replace a manual, spreadsheet-based order workflow.

- Architected the full system using Clean Architecture with clear separation across domain, application, infrastructure, and presentation layers.
- Built a multi-role authentication system with JWT, refresh tokens, and ASP.NET Identity, extended with a custom resource-authorisation layer that verifies both role and ownership on every request — preventing IDOR and privilege escalation by design, not convention.
- Modelled a 6-stage order fulfilment pipeline and a 7-state seller subscription lifecycle, with optimistic locking for concurrent writes and a deferred stock-deduction model to prevent inventory abuse.
- Delivered a fully type-safe React/TypeScript frontend using TanStack Query with a Context Endpoint Pattern aligned to backend auth boundaries.
- Codebase delivered production-ready; project paused at client direction.

---

### [GovConnect](https://github.com/MostafaAlaa) — Government Services Backend
*Feb 2025*

A backend system for managing driver, vehicle, and licence data, built with ASP.NET Core and EF Core.

- Applied layered architecture with Dependency Injection and the Repository Pattern.
- Implemented role-based access control across Admin, Employee, and User roles.
- Developed licence issuance triggered through publish–subscribe event logic; validated data with custom validators and SQL Server constraints.
- Wrote unit tests covering core services to support reliability and future refactoring.

---

## Background

I hold a B.Com. in Accounting from Helwan University (2017–2021). In 2023 I committed to software engineering full-time through self-directed study — working through data structures, algorithms, backend architecture, relational databases, and frontend development, applied through progressively complex projects.

Everything in this profile reflects work I've actually shipped, not coursework exercises. I find that building real systems with real constraints teaches things that nothing else does.

---

## Currently

Open to full-time roles and freelance/contract engagements — remote or Egypt-based.

If you're working on something that needs solid backend engineering, feel free to reach out.

📫 mostafaalaa11998@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/mostafaalaa) · [GitHub](https://github.com/MostafaAlaa)
