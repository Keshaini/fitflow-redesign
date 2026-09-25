# Weighted Technology Decision Matrix

| Criteria | Weight | Flutter (Frontend) | NestJS (Backend) | PostgreSQL (DB) | Firebase Auth |
|---|---|---|---|---|---|
| Performance | 25% | 9 | 8 | 8 | 8 |
| Scalability | 20% | 8 | 8 | 9 | 9 |
| Development speed | 20% | 8 | 8 | 6 | 9 |
| AI/ML support | 15% | 7 | 7 | 6 | — |
| Security/compliance | 15% | 8 | 8 | 9 | 8 |
| Cost | 5% | 7 | 6 | 7 | 8 |
| **Weighted total (/10)** | | **8.05** | **7.65** | **7.65** | **8.3** |

## Recommended Stack

- **Frontend:** Flutter
- **Backend:** NestJS (core API) + FastAPI (AI microservice)
- **Database:** PostgreSQL
- **Authentication:** Firebase Auth
- **Real-time layer:** Firebase Realtime Database / Socket.io (via NestJS)
- **AI/ML:** TensorFlow Lite (on-device) + Python-based cloud models
- **Caching:** Redis

## Rationale

This combination scores highest on performance and development speed while maintaining a strong security posture, which is critical given FitFlow's handling of personal health data. The stack closely mirrors proven choices from the original FitFlow case study redesign, adapted for stronger animation performance (Flutter) and better backend structure at scale (NestJS).