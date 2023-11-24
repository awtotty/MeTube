# Overview
A proof-of-concept clone of YouTube. 

# Learnings
- Prisma and DATABASE_URL env variable is required.
    - Depolying with Vercel requires this env var.
    - The supabase docs don't use this variable by default.
    - There is a distinction between DATABASE_URL and NEXT_PUBLIC_SUPABASE_URL.
    - The DATABASE_URL should start with the db language (e.g. postgresql://...)
- Vercel has integrations with db services like planetscale and supabase.
    - Don't forget to setup the integration on setup.
- Deploy to production as early and often as possible.
    - This was in Theo's guide for the twitter clone. 
    - This allows for immediate testing in prod environment. 

# Deployment
- Hosted serverless on Vercel
- postgres database on supabase with prisma ORM
- Auth with ...
- Logging with ...
