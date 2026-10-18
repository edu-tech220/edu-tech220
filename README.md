<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=200&section=header&text=Eduardo%20Ramirez&desc=Backend%20Developer%20%C2%B7%20C%23%20%2F%20.NET&descAlignY=62&fontSize=40&type=waving&fontColor=fefefe&animation=fadeIn" alt="Eduardo Ramirez · Backend Developer · C# / .NET"/>
</div>

## 👋 About me

Backend developer focused on **C# and .NET**. I build REST APIs with **ASP.NET Core**,
**Entity Framework Core** and **SQL Server**, and real-time features with **SignalR**.
I care about business rules living in the right place, consistent data under concurrency,
and shipping with automated tests, Docker and CI.

Currently looking for **Backend Developer (.NET)** opportunities.

## 🚀 Projects

### ⚡ Live Auction — real-time auction platform
[API](https://github.com/edu-tech220/live-auction) · [Web](https://github.com/edu-tech220/live-auction-web)

Bids are validated on the server and broadcast instantly to everyone watching.

- Optimistic concurrency with `rowversion` + retries, verified with 20 simultaneous bidders.
- SignalR hub with one group per auction, caller-only rejections and resync on reconnect.
- Idempotent auction closing in a `BackgroundService` that survives restarts.
- JWT, PBKDF2 password hashing, rate limiting; 71 backend tests and 32 frontend tests; Docker Compose and CI.

`ASP.NET Core` `SignalR` `EF Core` `SQL Server` `xUnit` `Docker` `GitHub Actions` `React` `TypeScript`

### ✅ TaskFlow — habit tracking API
[API](https://github.com/edu-tech220/TaskFlow) · [Web](https://github.com/edu-tech220/TaskFlow.Web)

Users schedule recurring activities, record daily completion and plan rest days.

- Versioned schedules: changing a routine never rewrites history.
- Monthly calendar computed with a fixed number of SQL queries (no N+1).
- Per-user data isolation, JWT with an admin role, ProblemDetails errors.
- 51 tests against a real SQL Server in CI; ASP.NET Core MVC client with a cookie-based session.

`ASP.NET Core` `EF Core` `SQL Server` `LINQ` `JWT` `xUnit` `ASP.NET Core MVC` `GitHub Actions`

## 🛠️ Tech I use in my projects

| Area | Technologies |
|---|---|
| Languages | C#, SQL, TypeScript |
| Backend | .NET 10, ASP.NET Core Web API, SignalR, ASP.NET Core MVC |
| Data | SQL Server, Entity Framework Core (Code First, migrations, Fluent API), LINQ |
| Security | JWT Bearer, role-based authorization, password hashing (PBKDF2), rate limiting, CORS |
| Testing | xUnit, WebApplicationFactory (integration tests against SQL Server), Vitest, Postman/Newman |
| DevOps | Docker, Docker Compose, GitHub Actions |
| API docs | OpenAPI, Swagger UI |
| Tools | Visual Studio, VS Code, Git, Postman |

## 📚 Learning next

- **Azure** fundamentals — preparing for **AZ-900**.
- **Redis** as a SignalR backplane to scale real-time features across instances.
- **Observability** with structured logging (Serilog) and OpenTelemetry.
- **Testcontainers** for disposable databases in integration tests.

<div align="center">
  <img src="https://capsule-render.vercel.app/api?color=0:1408d0,50:0860d0,100:08c4d0&height=100&section=footer&type=waving" alt=""/>
</div>
