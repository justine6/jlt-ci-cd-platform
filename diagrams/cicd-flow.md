# JLT CI/CD Platform — Delivery Flow

This diagram shows how code moves from developer commit to production deployment within the JLT Platform.

```mermaid
flowchart LR

    A[Developer]
    B[GitHub Repository]
    C[GitHub Actions CI]
    D[Build & Test]
    E[Security Scan]
    F[Artifact / Container Image]
    G[Deploy Pipeline]
    H[Cloud Platform / Kubernetes]
    I[Monitoring & Alerts]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I