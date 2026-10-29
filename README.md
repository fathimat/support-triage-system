
# Support Triage System

A full-stack web application for managing, tracking, and troubleshooting customer support tickets.

Built using React, Java Spring Boot, and PostgreSQL.

## Technology Stack

- Frontend: React, JavaScript, CSS, Vite
- Backend: Java, Spring Boot, REST APIs
- Database: PostgreSQL
- Build Tools: npm, Gradle
- Version Control: Git and GitHub

## Features

- Dashboard with ticket statistics
- Create new support tickets
- View ticket details
- Edit existing tickets
- Delete tickets with confirmation
- Update ticket status
- Search tickets
- Filter by status, priority, and category
- Sort tickets by priority
- Automatic rule-based ticket classification
- Persistent ticket storage using PostgreSQL
- Responsive user interface

## Architecture

React Frontend
      |
      | HTTP REST API
      v
Spring Boot Backend
      |
      | Spring Data JPA
      v
PostgreSQL Database

## Project Structure

support-triage/
  - React frontend application

support-triage-backend/
  - Java Spring Boot backend application

## Prerequisites

- Java 21
- Node.js and npm
- PostgreSQL
- Git

## Running the Backend

1. Create the PostgreSQL database configured in
   `application.properties`.
2. Open PowerShell in `support-triage-backend`.
3. Set the database password and start Spring Boot:

```powershell
$env:DB_PASSWORD = Read-Host "Enter PostgreSQL password"
.\gradlew.bat bootRun
```

Backend URL: http://localhost:8080

## Running the Frontend

Open another terminal in `support-triage`:

```powershell
npm.cmd install
npm.cmd run dev
```

Frontend URL: http://localhost:5173

## Production Build

Frontend:

```powershell
npm.cmd run build
```

Backend:

```powershell
.\gradlew.bat build
```

## Ticket Classification

New tickets can be classified using predefined rules
based on keywords in the ticket title and description.

This is currently a rule-based implementation,
not an AI-powered classification service.

## Future Improvements

- AI-powered ticket classification
- Authentication and role-based access
- Automated ticket assignment
- Advanced reporting and analytics

## Author

Full-stack Java and React portfolio project.
