# FitFlow Redesign

A redesign of the FitFlow fitness tracking app, built as part of IT3060 – Human Computer Interaction (SLIIT, Semester 2, 2026). This project addresses key usability pain points identified in user research — poor progress visualization, cumbersome workout logging, and limited personalization — through AI-powered workout plans, social community features, and simplified nutrition tracking.

## Tech Stack

- **Frontend:** Flutter (iOS, Android, Web)
- **Backend API:** Node.js with NestJS
- **AI Microservice:** Python with FastAPI
- **Database:** PostgreSQL
- **Authentication:** Firebase Auth
- **Real-time layer:** Firebase Realtime Database
- **Caching:** Redis

Full comparison and justification for these choices are documented in [`/docs/tech-stack-summary.md`](./docs/tech-stack-summary.md) and [`/docs/decision-matrix.md`](./docs/decision-matrix.md).

## Folder Structure

fitflow-redesign/
├── frontend/ # Flutter mobile & web app
├── backend/ # NestJS API gateway and core business logic
├── ai-service/ # FastAPI microservice for AI workout/nutrition models
└── docs/ # Architecture diagram, ADR, tech stack docs, decision matrix


## Architecture

The high-level system architecture — including data flows for personalized workout plans, social sharing, and nutrition tracking — is available in [`/docs/architecture-diagram.png`](./docs/architecture-diagram.png), with the accompanying rationale documented in [`/docs/adr-001-tech-stack.md`](./docs/adr-001-tech-stack.md).