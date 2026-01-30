# Technology Stack

This stack follows the product goals and architecture described in [concept.md](concept.md) and provides the web UI + API control plane for a Kubernetes-first platform. See [README.md](README.md) for the project overview.

## Core Platform
- Backend: Spring Boot (REST API, auth/RBAC, orchestration control plane).
- Database: PostgreSQL (tenants, servers, templates, RBAC, audit).
- Frontend: React (single-page app for operators and automation UI).
- UI Library: Mantine (admin dashboards, forms, file manager, editor UI).

## API & Contracts
- OpenAPI: API contract for UI, integrations, and automation.
- OpenAPI Generator: produces client/server stubs and SDKs from the contract.

## CI/CD & Distribution
- CI/CD: GitHub Actions (build, test, package, publish).
- Container Registry: publish backend images to GitHub Container Registry (GHCR).
- Packages: publish generated API artifacts to GitHub Packages:
  - npm package for JavaScript/TypeScript clients.
  - Maven package for JVM clients.

## Deployment Target
- Kubernetes-first orchestration, with Docker support for local or small deployments.
