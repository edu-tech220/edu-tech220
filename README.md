<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=200&section=header&text=Eduardo%20Ramirez&desc=Backend%20Developer%20%C2%B7%20C%23%20%2F%20.NET&descAlignY=62&fontSize=40&type=waving&fontColor=fefefe&animation=fadeIn" alt="Eduardo Ramirez · Backend Developer · C# / .NET"/>

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=0860D0&center=true&vCenter=true&width=620&lines=REST+APIs+with+ASP.NET+Core+%2B+EF+Core;Consistent+data+under+concurrency;Microservices%2C+Docker+and+CI+on+every+project" alt="REST APIs with ASP.NET Core + EF Core · Consistent data under concurrency · Microservices, Docker and CI on every project"/>

  <p>
    <img src="https://img.shields.io/badge/Open%20to%20work-Backend%20.NET-2ea44f?style=for-the-badge" alt="Open to work: Backend .NET"/>
    <a href="mailto:edualf55@gmail.com"><img src="https://img.shields.io/badge/Email-edualf55%40gmail.com-0860D0?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
    <img src="https://img.shields.io/badge/Location-Mexico%20City%20area-08C4D0?style=for-the-badge" alt="Location: Mexico City area"/>
  </p>
</div>

## 👋 About me

Backend developer focused on **C# and .NET**. I build REST APIs with **ASP.NET Core**,
**Entity Framework Core** and **SQL Server**, and real-time features with **SignalR**.
I care about business rules living in the right place, consistent data under concurrency,
and shipping with automated tests, Docker and CI.

- 🎯 Looking for **Backend Developer (.NET)** roles — on-site in the north of the Mexico City area, hybrid or remote.
- 🧪 Every project here ships with **xUnit tests and a green GitHub Actions pipeline**.
- 🌱 Currently learning **Azure (AZ-900)**, Redis and OpenTelemetry.

## 🧰 Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,azure,docker,githubactions,git&theme=dark" alt="C#, .NET, Azure, Docker, GitHub Actions, Git"/>
  <br/>
  <img src="https://skillicons.dev/icons?i=react,ts,postman,visualstudio,vscode&theme=dark" alt="React, TypeScript, Postman, Visual Studio, VS Code"/>
</p>

| Area | Technologies |
|---|---|
| Backend | ASP.NET Core Web API, Razor Pages, ASP.NET Core MVC, SignalR, BackgroundService |
| Data | SQL Server, Entity Framework Core (Code First, migrations, Fluent API), LINQ, stored procedures |
| Security | JWT Bearer, role-based authorization, PBKDF2 password hashing, rate limiting, CORS |
| Testing | xUnit, WebApplicationFactory, integration tests against SQL Server, Vitest, Postman/Newman |
| DevOps | Docker, Docker Compose, GitHub Actions, OpenAPI / Swagger |

## 🚀 Featured projects

### ⚡ Live Auction — real-time auction platform
[![CI](https://github.com/edu-tech220/live-auction/actions/workflows/ci.yml/badge.svg)](https://github.com/edu-tech220/live-auction/actions) &nbsp; [API](https://github.com/edu-tech220/live-auction) · [Web](https://github.com/edu-tech220/live-auction-web)

Bids are validated on the server and broadcast instantly to everyone watching.

- Optimistic concurrency with `rowversion` + retries, verified with 20 simultaneous bidders.
- SignalR hub with one group per auction, caller-only rejections and resync on reconnect.
- Idempotent auction closing in a `BackgroundService` that survives restarts.
- JWT, PBKDF2 password hashing, rate limiting; 71 backend tests and 32 frontend tests; Docker Compose and CI.

`ASP.NET Core` `SignalR` `EF Core` `SQL Server` `xUnit` `Docker` `GitHub Actions` `React` `TypeScript`

### ⚙️ JobFlow — background job orchestrator
[![CI](https://github.com/edu-tech220/jobflow/actions/workflows/ci.yml/badge.svg)](https://github.com/edu-tech220/jobflow/actions) &nbsp; [Repo](https://github.com/edu-tech220/jobflow)

Queue slow work over HTTP and run it outside the request, safely.

- Concurrent-safe job claiming with `UPDLOCK` / `READPAST` and leases.
- Retries with backoff, a record of every attempt and recovery of jobs left by a crashed worker.
- Clean Architecture (Domain / Application / Infrastructure / Api), central package management, Docker and CI.

`ASP.NET Core` `EF Core` `SQL Server` `BackgroundService` `Clean Architecture` `xUnit` `Docker`

### ✅ TaskFlow — habit tracking API
[![CI](https://github.com/edu-tech220/TaskFlow/actions/workflows/ci.yml/badge.svg)](https://github.com/edu-tech220/TaskFlow/actions) &nbsp; [API](https://github.com/edu-tech220/TaskFlow) · [Web](https://github.com/edu-tech220/TaskFlow.Web)

Users schedule recurring activities, record daily completion and plan rest days.

- Versioned schedules: changing a routine never rewrites history.
- Monthly calendar computed with a fixed number of SQL queries (no N+1).
- Per-user data isolation, JWT with an admin role, ProblemDetails errors.
- 51 tests against a real SQL Server in CI; ASP.NET Core MVC client with a cookie-based session.

`ASP.NET Core` `EF Core` `SQL Server` `LINQ` `JWT` `xUnit` `ASP.NET Core MVC` `GitHub Actions`

## 🧩 Microservices series

Domain-driven business apps, each one a **Razor Pages frontend + ASP.NET Core Web API** with its own tests,
Docker Compose (frontend, API and SQL Server) and CI.

| Project | Business problem | Highlights |
|---|---|---|
| [StayDesk](https://github.com/edu-tech220/staydesk) | Hotel reservations | No overbooking under concurrency, seasonal / weekend rates, reservation state machine with cancellation policy |
| [BloodLink](https://github.com/edu-tech220/bloodlink) | Blood bank | ABO/Rh compatibility rules, FEFO allocation, safe reservation of scarce units across hospitals |
| [FleetDesk](https://github.com/edu-tech220/fleetdesk) | Fleet maintenance | Preventive service by mileage *and* time, work orders, spare-part stock under concurrent mechanics |

More business APIs (clinic scheduling, inventory, ticketing, parking, leave management…) are in my
[repositories](https://github.com/edu-tech220?tab=repositories).

<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=100&section=footer&type=waving" alt=""/>
</div>
