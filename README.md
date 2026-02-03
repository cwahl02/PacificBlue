# Coding Challenge Website

## Description
An in development platform for solving coding problems. Users will be able to submit code, receive real-time feedback, and track their progress. The project includes backend job processing, a real-time feedback system, and a responsive web UI.

## Getting Started
#### 1. Clone the repository
```bash
git clone https://github.com/cwahl02/CPW-226-Portfolio
cd CPW-226-Portfolio
```
#### 2. Restore dependencies
```bash
dotnet restore
```

#### 2. Set up the database
Ensure SQL Server is installed and running.

Apply migrations:
```bash
dotnet ef database update
```

#### 4. Build & Run
```bash
dotnet build
dotnet run
```
## Planned Features
- **User Management**: Authentication and profiles
- **Classes**: Create and manage school classes for students and instructors
- **Groups**: Real-time collaborative problem-solving with multiple participants
- **Coding Problems**: Solve problems using an online editor (powered by Monaco Editor)
- **Real-Time Execution Feedback**: Compilation time, runtime output, and partial results streamed via SignalR
- **Progress Tracking**: Track user and class progress on challenges
- **Responsive UI**: Built with Blazor and Tailwind CSS

## Tech Stack
- .NET 10 - Backend framework handling API endpoints, business logic, and job orchestration
- ASP.NET Blazor - Frontend framework for interactive UI
- Monaco Editor - In-browser code editor for solving code problems
- Redis - Job queue for sending code execution jobs to workers and general messaging between services
- SignalR - Real-time feedback of execution feedback and collaborative group activity to the web client
- SQL Server - Persistent storage for user submissions, classes, groups, and more
- Tailwind CSS - Styling and responsive design
