# Student Management Portal — Backend API

A **RESTful ASP.NET Core API** for managing student records — including personal details, addresses, gender classification, and profile image storage.

## Tech Stack

- **ASP.NET Core Web API** (.NET)
- **Entity Framework Core** — Code-First with SQL Server
- **AutoMapper** — with custom AfterMap configurations
- **Repository Pattern** — `IStudentRepository`, `IImageRepository`

## Key Features

- Student CRUD (create, read, update, delete)
- Gender classification management
- Address data embedded with each student record
- Profile image upload and retrieval
- AutoMapper AfterMaps for complex DTO transformations
- Swagger / OpenAPI documentation

## API Endpoints

| Method | Route | Description |
|---|---|---|
| GET | `/api/students` | List all students |
| GET | `/api/students/{id}` | Get student by ID |
| POST | `/api/students` | Add a new student |
| PUT | `/api/students/{id}` | Update student details |
| DELETE | `/api/students/{id}` | Delete a student |
| GET | `/api/genders` | List genders |

## Getting Started

1. Set connection string in `appsettings.json`.
2. Apply migrations: `dotnet ef database update`
3. Run the API: `dotnet run`

> The Angular frontend is in [Student-Management-Portal-UI](https://github.com/AhmedElneziliiy/Student-Management-Portal-UI).
