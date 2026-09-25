# Tech Stack Summary

## Frontend Comparison

| Criteria | Flutter | React Native | Kotlin Multiplatform | Swift/SwiftUI |
|---|---|---|---|---|
| Development speed | Fast — single codebase, hot reload | Fast — single codebase, huge community | Moderate — shares logic, not UI | Slow — iOS-only |
| Code reusability | Very high (~90%+) | Very high (~80-90%) | Moderate (logic shared, UI native) | None (iOS only) |
| Performance | Near-native | Good, can lag on heavy animation | Native performance | Best possible |
| Ecosystem support | Strong, Google-backed | Very mature, Meta-backed | Smaller, JetBrains-backed | Mature, Apple-only |
| Learning curve | Moderate (Dart) | Easier (JS/React) | Steep | Steep if new |
| Web compatibility | Yes (Flutter Web) | Yes (via RN Web) | Limited/experimental | No |
| AI/ML integration | Good (TFLite, ML Kit) | Good (TensorFlow.js) | Good (native ML Kit/Core ML) | Best (Core ML) |
| Real-time features | Good | Good | Good | Excellent |
| Maintenance cost | Low (one codebase) | Low (one codebase) | Medium | High (separate codebases) |
| Security | Good | Good | Good | Excellent |

**Selected: Flutter** — best balance of near-native performance for animated fitness UI, single codebase across iOS/Android/Web, and mature AI/ML plugin support.

## Backend Comparison

| Criteria | Node.js/NestJS | Python/FastAPI | Go |
|---|---|---|---|
| Development speed | Fast, huge ecosystem | Fast, strong for AI/ML work | Moderate, more verbose |
| Performance | Good (event-loop) | Good (async support) | Excellent (compiled, concurrent) |
| AI/ML integration | Moderate (via API calls) | Excellent (native Python ML ecosystem) | Moderate |
| Real-time capability | Excellent (Socket.io) | Good (async WebSocket) | Excellent (goroutines) |
| Learning curve | Moderate | Easy | Steep if unfamiliar |

**Selected: NestJS (core API) + FastAPI (AI microservice)** — NestJS for structured, scalable API development; FastAPI isolated specifically for AI/ML workloads given Python's superior ML ecosystem.

## Database Comparison

| Criteria | PostgreSQL | MongoDB | Firebase (Firestore) | DynamoDB |
|---|---|---|---|---|
| Scalability | Good (vertical + replicas) | Excellent (horizontal sharding) | Excellent (managed) | Excellent (managed) |
| Query performance | Excellent for structured data | Good for flexible/nested data | Good, limited complex queries | Good, limited complex queries |
| Health data handling | Strong (relational integrity) | Good (flexible schema) | Good (real-time sync) | Good (high write throughput) |
| Real-time support | Requires add-ons | Good (change streams) | Excellent (native) | Moderate (via Streams) |

**Selected: PostgreSQL** — strong relational integrity is critical for structured, sensitive health/fitness data.

## Authentication Comparison

| Criteria | Firebase Auth | AWS Cognito | Auth0 | Supabase |
|---|---|---|---|---|
| Ease of integration | Excellent | Moderate | Excellent | Excellent |
| Security/compliance | Good, GDPR-compliant | Strong, HIPAA-eligible | Strong (SOC2, GDPR, HIPAA add-ons) | Good, GDPR-compliant |
| Cost for mid-size team | Free tier generous | Pay-as-you-go | Can get expensive at scale | Free tier generous |
| Social/OAuth support | Excellent | Good | Excellent | Good |

**Selected: Firebase Auth** — fastest integration and generous free tier, sufficient GDPR compliance for current scale, with a documented migration path to AWS Cognito if HIPAA-level compliance is later required.