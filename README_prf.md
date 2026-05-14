# Hey, I'm Mostafa 👋

I'm a .NET backend developer based in Egypt who got into software the slow way — accounting degree, then a few years of self-teaching, then building real things until the skills stuck. No bootcamp shortcut. Just a lot of time with docs, broken builds, and projects that gradually stopped breaking.

These days I spend most of my time on backend architecture: designing systems that are actually maintainable, thinking through data models before touching a keyboard, and caring probably too much about how things fit together under the hood.

---

## What I actually work with

**Day-to-day:** C#, ASP.NET Core, SQL Server, Docker  
**When the job calls for it:** React + TypeScript, PostgreSQL, RabbitMQ, Redis  
**How I work:** Clean Architecture, SOLID, proper testing (xUnit + Moq), CI/CD with GitHub Actions, structured logging via Serilog

I'm comfortable across the stack — I've shipped full React/TypeScript frontends — but backend architecture and performance is where I go deep.

---

## Things I've built that I'm proud of

### [Metriflow](https://github.com/MostafaAlaa) — Event-Driven Analytics Pipeline
This one was a proper engineering challenge. Built an end-to-end ETL pipeline that takes high-volume event data and aggregates it across seven stages (Raw → Staged → Page → Daily → Time Interval → Monthly → Yearly), each powered by background worker services communicating through RabbitMQ.

The part I enjoyed most: getting 26 million records through the pipeline in under 3 minutes. That meant combining Producer–Consumer channels, streaming JSON deserialisation, and `SqlBulkCopy` at 250K records per batch. Also handled late-arriving and duplicate events by recomputing affected aggregates — because real-world data is never clean.

Stack: .NET, RabbitMQ, Redis, SQL Server, Docker Compose, GitHub Actions

---

### [Kemet](https://github.com/MostafaAlaa) — E-Commerce Platform (Freelance)
Replaced a manual spreadsheet-based order workflow with an actual system. Built it end-to-end: multi-role auth with JWT and refresh tokens, a custom resource-authorisation layer that verifies both role *and* ownership on every request (no IDOR by accident), a 6-stage order fulfilment pipeline with optimistic locking for concurrent writes, and a fully type-safe React/TypeScript frontend.

The client paused the project, but the codebase was production-ready and fully delivered.

---

### [GovConnect](https://github.com/MostafaAlaa) — Government Services Backend
Earlier project, but still one I reference. Built to manage driver, vehicle, and licence data with layered architecture and role-based access control. Implemented licence issuance through pub/sub event logic and wrote unit tests to support future refactoring — because systems like this get maintained, not rewritten.

---

## How I think about software

A few things I care about that don't always make it onto a CV:

- I'd rather model the domain correctly upfront than refactor six months later. Time spent on a good data model almost always pays back.
- Auth and ownership checks should be structural, not an afterthought. The Kemet authorisation layer wasn't a requirement I was handed — it was just the right thing to build.
- Performance matters, but not everywhere equally. I optimised Metriflow's ingestion because the numbers demanded it. Most of my other code is optimised for being read by the next developer.

---

## A bit of background

I studied accounting, not computer science. In 2023 I decided to take software seriously and started building — data structures, algorithms, C#, backend architecture, databases, and eventually frontend too. Everything in my CV came from building real projects, not coursework.

I'm not going to pretend that's the conventional path. But I think it's made me more deliberate about understanding *why* things work, not just *that* they work.

---

## Currently

Open to full-time roles and freelance/contract work — remote or Egypt-based, whatever makes sense. If you're working on something interesting and need someone who genuinely cares about the backend holding everything together, let's talk.

📫 mostafaalaa11998@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/mostafaalaa) · [GitHub](https://github.com/MostafaAlaa)
