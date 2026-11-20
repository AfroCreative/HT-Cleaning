# HT Cleaning

Website and admin dashboard for a commercial cleaning business in Columbus, Ohio.

## What's here

| Path | What it is |
|---|---|
| `index.html` | Public marketing website: services, industries, how it works, service area, quote request form |
| `admin/index.html` | Admin dashboard: clients, workers, jobs, expenses and business stats |
| `docs/launch-checklist.md` | Steps to launch the business |

Both pages are single, self-contained HTML files with no build step. Open them in a browser or host them on any static host (GitHub Pages, Netlify, Vercel).

## Publishing the website with GitHub Pages

1. Go to **Settings → Pages** in this repo.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
3. The site will appear at `https://afrocreative.github.io/HT-Cleaning/`. You can add a custom domain on the same page.

## Important notes

- **Admin dashboard storage:** the dashboard saves data through Claude's artifact storage, which only works when it's opened as the Claude artifact. Opened from GitHub Pages or a local file, it runs in **preview mode**, where nothing is saved. Don't publish `admin/` as your live admin tool until it's connected to a real backend (for example Supabase or Firebase) with a login.
- **Website placeholders:** replace "Your Cleaning Co.", `(614) 555-0123` and `hello@yourcleaningco.com` with your real details. Remove "Insured & bonded" and "background-checked" until they're true.
- **Quote form:** it isn't connected to anything yet. Visitors are asked to copy their details and email or call. To have requests land in your inbox, connect the form to a service such as Formspree.
