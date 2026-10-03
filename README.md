# Anime Hub Admin Panel

GitHub Pages-ready admin panel for the Anime Hub Supabase project.

## Files
- `admin.html` — Admin login + dashboard + Anime/Season/Episode CRUD.
- `config.js` — Supabase project URL + **publishable** key only.
- `.nojekyll` — keeps the folder simple on GitHub Pages.

## Deploy
Upload all files in this folder to the same GitHub repository as the Anime Hub site.

Then open:
`https://samiul145.github.io/anime-hub/admin.html`

Do not open `admin.html` directly from a `content://` file URL for testing.

## Security
Never put `sb_secret_...` or `service_role` keys in this repository. The browser app uses only the publishable key and relies on Supabase Auth + RLS.

The admin user must exist in `auth.users` and its UUID must also exist in `public.admins`.
