# Deployment steps (concise)

1. Create Supabase project (Postgres) and get `DATABASE_URL`. Run SQL from `backend/schema.sql`.
2. Sign up for Adzuna, get `ADZUNA_APP_ID` and `ADZUNA_API_KEY`.
3. Push this repo to GitHub.
4. Configure GitHub secrets as listed in README.
5. Frontend:
   - Connect your repo to Vercel, set environment variables (if any) and deploy.
6. Backend:
   - Deploy to Render (or Railway) using Dockerfile in `backend/` OR use GitHub Actions to build and push Docker image.
7. Enable GitHub Actions schedule or Render cron to run crawler.
8. Open site and test filters.

If you'd like, paste your Vercel/Render URLs here and I will provide final tweaks.

