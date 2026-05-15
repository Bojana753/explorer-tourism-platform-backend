# Explorer Tourism Platform — Backend

> A modular, gamified tourism API built with .NET (C#) — connecting tour authors with adventurous tourists through XP, encounters, smart tour planning and an integrated chatbot.

---

## Overview

**Explorer** is a full-featured tourism platform developed as a collaborative team project using agile methodology. The backend exposes a RESTful API built on a **modular monolith architecture**, covering everything from tour management and real-time execution to payments, gamification, and social features.

Key capabilities:
- Tour discovery, purchase, and execution with GPS key points
- Gamification engine — XP, levels, badges, and coupons
- Integrated chatbot for in-tour assistance
- Tour conflict detection in the planner
- Emergency assistance module
- Club and leaderboard social system
- Author analytics and tour statistics

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | C# (.NET) |
| Architecture | Modular Monolith |
| Database | SQL Server |
| ORM | Entity Framework Core |
| Testing | Unit & Integration Tests |

---

## Modules

| Module | Responsibility |
|--------|---------------|
| **Tours** | Tour creation, key points, bundles, execution tracking, statistics |
| **Encounters** | Gamified challenges tied to tour locations |
| **Payments** | Shopping cart, purchases, wallet, coupons, notifications |
| **Blog** | Content publishing for authors and tourists |
| **Stakeholders** | User management across all roles |

---

## User Roles

| Role | Capabilities |
|------|-------------|
| **Tourist** | Browse, purchase, and execute tours; earn XP and rewards |
| **Author** | Create and manage tours; access analytics dashboard |
| **Administrator** | Platform oversight and administration |

---

## Development Process

- Developed in **agile sprints** as part of a collaborative student team
- Task and sprint management via **Trello** and **ClickUp**
- Version control with **Git**

---

## Getting Started

### Prerequisites

- .NET SDK
- SQL Server

### Run

```bash
# Restore dependencies
dotnet restore

# Apply migrations
dotnet ef database update

# Start the API
dotnet run --project Explorer.API
```

The API will be available at `https://localhost:{port}`.

> Seed scripts for each module are located in the `TestData` folder (`.sql` files).
