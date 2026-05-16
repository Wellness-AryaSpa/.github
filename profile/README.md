<p align="center">
  <img src="https://aryaspa.eu/logo.png" alt="AryaSpa" width="140" />
</p>

<h1 align="center">AryaSpa</h1>

<p align="center">
  Private wellness platform for booking, vouchers, content management and digital spa operations.
</p>

<p align="center">
  <a href="https://aryaspa.eu">Website</a>
  ·
  <a href="https://staging.aryaspa.eu">Staging</a>
  ·
  <a href="https://api.aryaspa.eu/actuator/health">API Health</a>
</p>

---

## About the project

**AryaSpa** is a private wellness platform built around a calm booking experience, gift vouchers, media-driven content and a dedicated administration panel.

The system is split into several applications:

| Area | Repository | Purpose |
|---|---|---|
| Public website | `aryaspa_frontend` | User-facing website, booking flow, vouchers and content pages |
| Backend API | `aryaspa_backend` | Java/Spring Boot API, business logic, storage integration and deployment workflows |
| Admin panel | `aryaspa_admin` | Backoffice interface for content, media, packages, vouchers and operations |
| Production audit | `AryaSpa-prod-audit` | Production readiness checks, audits and release documentation |

---

## Technology stack

### Frontend

- Next.js
- TypeScript
- React
- Vitest
- ESLint / Prettier
- CDN-ready media layer

### Backend

- Java
- Spring Boot
- MySQL
- Redis
- Flyway
- Docker
- GitHub Actions

### Infrastructure

- Cloudflare
- Nginx reverse proxy
- Docker Compose
- GHCR
- SeaweedFS
- imgproxy
- Separate staging and production environments

---

## Environments

| Environment | Public site | API | Admin |
|---|---|---|---|
| Production | `aryaspa.eu` | `api.aryaspa.eu` | `admin.aryaspa.eu` |
| Staging | `staging.aryaspa.eu` | `staging-api.aryaspa.eu` | `staging-admin.aryaspa.eu` |

---

## Development principles

- Staging and production are separated.
- Backend, frontend and admin are deployed as independent applications.
- Server runtime uses Docker images, not source-code builds.
- Public website does not expose admin API routes.
- Secrets and environment files are never stored in public repositories.
- Infrastructure and storage are isolated from other projects.

---

## Project status

AryaSpa is currently under active development.

Current focus:

- public frontend stabilization;
- backend API integration;
- admin panel development;
- CMS/content editing flow;
- booking and voucher flow;
- production readiness and security hardening.

---

<p align="center">
  Built for AryaSpa · Prague, Czech Republic
</p>
