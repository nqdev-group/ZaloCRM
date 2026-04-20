# AI Agent Instructions for ZaloCRM

This file provides essential guidance for AI coding agents working in the ZaloCRM codebase. It summarizes key conventions, build/test commands, and links to detailed documentation. Update this file as project conventions evolve.

## Project Overview
- **Monorepo**: Contains both backend (Node.js/Fastify/Prisma) and frontend (Vue 3/Vuetify/Vite) apps.
- **Main docs**: See [README.md](README.md) for features, setup, and architecture.

## Build & Development Commands

### Backend
- **Dev server**: `cd backend && npm run dev`
- **Build**: `cd backend && npm run build`
- **Start**: `cd backend && npm start`
- **DB migrate**: `cd backend && npm run db:migrate`
- **DB seed**: `cd backend && npm run db:seed`

### Frontend
- **Dev server**: `cd frontend && npm run dev`
- **Build**: `cd frontend && npm run build`

### Docker Compose (full stack)
- **Start all**: `docker compose up -d --build`

## Key Conventions
- **.env setup**: Copy `.env.example` to `.env` and set secrets before running.
- **API keys**: Use `X-API-Key` header for API authentication (see [HUONG-DAN-SU-DUNG.md](HUONG-DAN-SU-DUNG.md)).
- **Prisma**: All DB schema changes require migration and push.
- **Frontend**: Uses Vue 3 `<script setup>` SFCs and Pinia for state management.

## Documentation Links
- [README.md](README.md): Features, quickstart, architecture
- [HUONG-DAN-CAI-DAT.md](HUONG-DAN-CAI-DAT.md): Detailed installation guide
- [HUONG-DAN-SU-DUNG.md](HUONG-DAN-SU-DUNG.md): API & usage guide
- [backend/prisma/schema.prisma](backend/prisma/schema.prisma): Database schema

## Tips for AI Agents
- Prefer linking to docs over duplicating content
- Use provided scripts for setup and development
- Ask for clarification if conventions are unclear

---
_Last updated: 2026-04-20_
