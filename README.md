<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=200&section=header&text=Eduardo%20Ramirez&desc=Backend%20Developer%20%C2%B7%20C%23%20%2F%20.NET&descAlignY=62&fontSize=40&type=waving&fontColor=fefefe&animation=fadeIn" alt="Eduardo Ramirez · Backend Developer · C# / .NET"/>

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=0860D0&center=true&vCenter=true&width=680&lines=REST+APIs+%E2%80%94+ASP.NET+Core+%2B+EF+Core+%2B+SQL+Server;Concurrency+problems+solved%2C+tests+prove+it;10%2B+domain+apps+shipped+with+Docker+%26+CI;Available+now+%E2%80%94+Backend+.NET+roles" alt="REST APIs — ASP.NET Core + EF Core + SQL Server · Concurrency problems solved, tests prove it · 10+ domain apps shipped with Docker & CI · Available now — Backend .NET roles"/>

  <p>
    <img src="https://img.shields.io/badge/%F0%9F%9F%A2%20Available%20now-Backend%20.NET-2ea44f?style=for-the-badge" alt="Available now: Backend .NET"/>
    <a href="mailto:edualf55@gmail.com"><img src="https://img.shields.io/badge/Email-edualf55%40gmail.com-0860D0?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
    <img src="https://img.shields.io/badge/Location-CDMX%20north%20%7C%20hybrid%20%7C%20remote-08C4D0?style=for-the-badge" alt="Location: CDMX north | hybrid | remote"/>
  </p>
</div>

## 👋 About me

Backend developer specialised in **C# and .NET**, building production-grade REST APIs
with **ASP.NET Core**, **Entity Framework Core** and **SQL Server**. I focus on correctness
under concurrency, clean domain boundaries and shipping with automated tests, Docker and CI.
Every repository here has a green pipeline and integration tests that hit a real database.

- 🎯 Looking for **Backend Developer (.NET)** roles — on-site north of CDMX, hybrid, or remote.
- 🧪 Every project ships with **xUnit integration tests** running against SQL Server in GitHub Actions.
- 🌱 Currently deepening: **Azure (AZ-900)**, Redis and OpenTelemetry.
- 🌐 Comfortable reading and writing technical English.


## 🧰 Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,docker,githubactions,git,postman,visualstudio,vscode&theme=dark" alt="C#, .NET, Docker, GitHub Actions, Git, Postman, Visual Studio, VS Code"/>
  <br/>
  <img src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" alt="Microsoft SQL Server"/>
</p>

| Area | Technologies |
|---|---|
| Backend | C#, ASP.NET Core Web API, ASP.NET Core MVC, Razor Pages, SignalR, BackgroundService |
| Database | SQL Server, T-SQL, Entity Framework Core, LINQ, Stored Procedures, Code First, Migrations |
| Security | JWT Bearer, Role-based authorization, PBKDF2 password hashing, Rate Limiting, CORS |
| Testing | xUnit, WebApplicationFactory, Integration Testing, Postman/Newman |
| DevOps | Docker, Docker Compose, GitHub Actions, Git, OpenAPI / Swagger |
| Tools | Visual Studio, VS Code, Postman |

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

## 🧩 Domain apps series

Business apps, each a **Razor Pages frontend + ASP.NET Core Web API** with domain rules,
integration tests, Docker Compose (frontend · API · SQL Server) and a green CI pipeline.

| Project | Business problem | Highlights |
|---|---|---|
| [StayDesk](https://github.com/edu-tech220/staydesk) | Hotel reservations | No overbooking under concurrency, seasonal / weekend rates, reservation state machine with cancellation policy |
| [BloodLink](https://github.com/edu-tech220/bloodlink) | Blood bank | ABO/Rh compatibility rules, FEFO allocation, safe reservation of scarce units across hospitals |
| [FleetDesk](https://github.com/edu-tech220/fleetdesk) | Fleet maintenance | Preventive service by mileage *and* time, work orders, spare-part stock under concurrent mechanics |
| [PayDesk](https://github.com/edu-tech220/paydesk) | Payroll | Salary computation, overtime, deductions and payroll period closing |
| [EnrollDesk](https://github.com/edu-tech220/enrolldesk) | Academic enrollment | Course capacity, prerequisites, enrollment windows and schedule conflict detection |
| [BillFlow](https://github.com/edu-tech220/billflow) | Billing & invoicing | Invoice lifecycle, payment matching, overdue tracking and partial payments |
| [DineDesk](https://github.com/edu-tech220/dinedesk) | Restaurant orders | Table management, kitchen queue, order state machine and split-bill support |
| [RepairDesk](https://github.com/edu-tech220/repairdesk) | Repair workshop | Work orders, parts reservation, technician assignment and repair status tracking |
| [HelpQueue](https://github.com/edu-tech220/helpqueue) | IT help desk | Ticket triage, SLA timers, escalation rules and agent workload balancing |
| [ClaimFlow](https://github.com/edu-tech220/claimflow) | Insurance claims | Claim intake, adjudication workflow, document checklist and settlement tracking |

<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=100&section=footer&type=waving" alt=""/>
</div>
