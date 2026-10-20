<!--
  Maintenance: update the Featured Projects section when a project changes,
  and keep the stack table limited to what a repository demonstrates.
-->

<div align="center">

<img src="./assets/banner.svg" alt="Khader Mohamed, Junior .NET Backend Developer" width="100%">

</div>

**Turning business rules into tested, well-structured APIs with C# & ASP.NET Core.**

I'm a junior .NET backend developer based in Gharbia, Egypt, and a B.Sc. Information Technology student (expected 2027). I build REST APIs and server-side web apps with C#, ASP.NET Core, EF Core and SQL Server, and I care about what sits behind the endpoints: business rules, data integrity, error handling, architecture and tests. I'm looking for a junior .NET backend role where I can keep growing as a backend engineer.

## Featured Projects

### [LibrarySystem](https://github.com/khadermohamed/LibrarySystem) — REST API, Clean Architecture

A REST API for a library's catalogue, members, and borrowing and returns.

- Four-project Clean Architecture (API, Services, Data, Contracts), with the dependency rule checked by architecture tests (NetArchTest)
- Eight documented business rules (availability, fines, loan limits and more), enforced through typed domain exceptions
- A global exception middleware maps errors to 404, 409 and 422 responses in RFC 7807 problem-details format
- Concurrency handling with `UPDLOCK` and EF Core `RowVersion`
- Unit tests (xUnit, Moq), integration tests (WebApplicationFactory, Testcontainers) and load tests (NBomber, JMeter)

**Stack:** .NET 10 · ASP.NET Core · EF Core · SQL Server · FluentValidation

### [Gym Management System](https://github.com/khadermohamed/gym-management-system-dotnet) — ASP.NET Core MVC

A web app for gym operations: members, trainers, session booking, memberships and admin dashboards.

- Three-layer architecture with repositories, a Result pattern and Autofac modules
- EF Core: Fluent API configurations, soft delete via global query filters, an audit-column interceptor and TPH inheritance
- Role-based access for Admin, Trainer and Member using ASP.NET Identity
- Structured logging with Serilog and Seq, a hosted background cleanup job, and configuration via user secrets

**Stack:** .NET 10 · ASP.NET Core MVC · EF Core · SQL Server · Autofac · Serilog

### [School Portal](https://github.com/khadermohamed/school-portal) — microservices with Docker

Two independent ASP.NET Core services (Students and Grades), each with its own database.

- Database-per-service isolation on SQL Server
- Grades validates students over HTTP against the Students API and degrades gracefully if it is unavailable
- Docker Compose orchestration, multi-stage Dockerfiles and automatic EF Core migrations

**Stack:** ASP.NET Core 10 · EF Core · SQL Server · Docker Compose

**Also on my profile:**
[Bank-Management-System](https://github.com/khadermohamed/Bank-Management-System) (EF Core Code-First model with many-to-many relationships via Fluent API) ·
[e-commerce-checkout-system](https://github.com/khadermohamed/e-commerce-checkout-system) (clean-architecture checkout engine with custom typed exceptions)

## Tech Stack

| Area | What I use | See it in |
|---|---|---|
| Language | C#, SQL | All projects |
| Web | ASP.NET Core (Web API, MVC), FluentValidation, ASP.NET Identity | LibrarySystem, Gym Management |
| Data | EF Core (Code-First, Fluent API, migrations, interceptors), SQL Server | All projects |
| Architecture | Layered and Clean Architecture, repository and unit of work, Result pattern, microservices basics | LibrarySystem, Gym Management, School Portal |
| Testing | xUnit, Moq, Shouldly, Testcontainers, NetArchTest, NBomber, JMeter | LibrarySystem |
| Tooling | Docker and Docker Compose, Serilog and Seq, Git | School Portal, Gym Management |

## Current Focus

- Authentication and authorization for APIs: JWT and refresh-token flows
- API design, validation and consistent error handling
- CQRS with MediatR, and vertical slice architecture
- Database design and query performance
- Extending automated testing across more of my projects

## Education

**B.Sc. Information Technology**, Delta Technological University, Menoufia, Egypt. Expected graduation: 2027.

## Contact

[LinkedIn](https://www.linkedin.com/in/khader-mohamed-b1b395352) · [Email](mailto:khaderelhabal923@gmail.com)
