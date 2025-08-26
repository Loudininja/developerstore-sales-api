# DeveloperStore Sales API

## 📌 Overview
This project is part of the **Developer Evaluation Project**.  
It implements a **Sales API (CRUD)** following **DDD principles**, with business rules and optional domain events.

---

## 🚀 Tech Stack
- .NET 8 / C#
- Entity Framework Core
- xUnit (or NUnit/MSTest) for testing
- Swagger / OpenAPI for API documentation
- SQL Server (or PostgreSQL)

---

## 📂 Project Structure
src/
├── Domain/ # Entities, Value Objects, Rules
├── Application/ # Services, Use Cases
├── Infrastructure/ # Persistence, API Controllers
└── Tests/ # Unit and Integration Tests

yaml
Copiar código

---

## ⚙️ Setup & Run

### Prerequisites
- .NET 8 SDK
- Docker (optional for database)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/developerstore-sales-api.git
   cd developerstore-sales-api
Install dependencies:

bash
Copiar código
dotnet restore
Run database migrations:

bash
Copiar código
dotnet ef database update
Start the application:

bash
Copiar código
dotnet run --project src/Infrastructure
Open API docs at:

bash
Copiar código
http://localhost:5000/swagger
🧪 Testing
Run all tests with:

bash
Copiar código
dotnet test
📜 Business Rules
4+ items → 10% discount

10–20 items → 20% discount

20 items → not allowed

< 4 items → no discount

📡 Domain Events (Optional)
SaleCreated

SaleModified

SaleCancelled

ItemCancelled

Events are logged in the application console/logs.

✅ Checklist
See the Kanban Board for progress tracking.
