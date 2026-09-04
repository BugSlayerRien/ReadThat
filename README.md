# ReadThat

A book discovery and review web app. Browse books, write reviews, track reading progress, and manage content from an admin dashboard. Backend powered by [Supabase](https://supabase.com).
--------------------------
## Features

- **Auth** — sign up, log in, and role-based access (user / admin)
- **Browse** — explore books with covers and details
- **Reviews** — ratings, review text, spoiler flags, and helpful votes
- **Reading progress** — wishlist, currently reading, finished, DNF
- **Community** — recent reviews from other readers
- **Admin** — manage books, moderate reviews, edit users/roles, site settings

## Stack

- React + Vite
- React Router
- Supabase (Auth + Postgres)

## Setup

1. Clone the repo and install dependencies:

   ```bash
   npm install
   ```

2. Create your env file from the example:

   ```bash
   cp .env.example .env
   ```

3. Fill in `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` from your Supabase project settings (Project Settings → API).

4. Start the dev server:

   ```bash
   npm run dev
   ```

5. Production build:

   ```bash
   npm run build
   npm run preview
   ```

## Environment variables

| Variable | Description |
|----------|-------------|
| `VITE_SUPABASE_URL` | Supabase project URL |
| `VITE_SUPABASE_ANON_KEY` | Supabase anon / publishable key (safe for client apps if RLS is configured) |

Do **not** commit `.env` or service-role keys.

## Project status

This repository should contain the app source (`src/`, `package.json`, and related config). If those files are missing from a local copy, restore them before developing or deploying — `dist/` and `node_modules/` are intentionally not tracked.

## License

Private / unlicensed unless otherwise noted.
