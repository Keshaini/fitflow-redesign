# ADR-001: Technology Stack Selection for FitFlow Redesign

**Status:** Accepted

## Context

FitFlow requires a cross-platform mobile/web application with AI-powered personalization, real-time social features, and secure health data handling, to be built by a mid-sized team under time-to-market pressure.

## Decision

Adopt the following stack:
- **Frontend:** Flutter
- **Backend:** NestJS (API gateway and business logic)
- **AI Microservice:** FastAPI (Python)
- **Database:** PostgreSQL
- **Authentication:** Firebase Auth
- **Real-time layer:** Firebase Realtime Database
- **Caching:** Redis

## Consequences

This stack maximizes code reuse and development speed while isolating AI/ML workloads into a specialized Python service, keeping the main API lightweight and maintainable. The trade-off is added operational complexity from running two backend services (NestJS and FastAPI) instead of one, requiring clearly defined API contracts between them. PostgreSQL's relational structure adds some rigidity compared to NoSQL alternatives, but this is justified by the need for strong data integrity around health-related records.