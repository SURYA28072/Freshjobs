# Bangalore CSE Freshers Job Board

This repository contains a production-ready job board for **B.Tech CSE freshers in Bangalore**:
- Frontend: Next.js (React) (folder: `frontend`)
- Backend: FastAPI (folder: `backend`)
- Crawler: Simple Adzuna fetch script (folder: `crawler`)
- CI: GitHub Actions workflow for builds and scheduled crawling (folder: `.github/workflows`)

## How to use

1. Create the required accounts and secrets (see `.env.example`).
2. Initialize the Postgres DB (Supabase recommended), run the `schema.sql`.
3. Push the repo to GitHub.
4. Set GitHub secrets and connect to Vercel (frontend) and Render (backend) or deploy via Docker.
5. Enable the scheduled workflow (runs every 15 minutes) or use Render Cron.

Secrets required (store as GitHub secrets / platform env vars):
- DATABASE_URL
- ADZUNA_APP_ID
- ADZUNA_API_KEY
- VERCEL_TOKEN (optional for GH Actions deploy)
- VERCEL_PROJECT_ID
- VERCEL_ORG_ID
- DOCKERHUB_USERNAME (optional)
- DOCKERHUB_TOKEN (optional)

For step-by-step deployment instructions, open `DEPLOYMENT.md`.

