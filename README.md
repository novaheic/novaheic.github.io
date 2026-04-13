# Nova Heidt Portfolio

Mobile-first portfolio site built as plain static HTML/CSS/JS for GitHub Pages.

## Files You Will Edit Most

- `assets/data/projects.json` - profile details + all project cards/content
- `assets/css/style.css` - theme, spacing, cards, responsive styling
- `assets/js/main.js` - rendering logic, detail-page loading, reveal animations

## Project Data Shape

`projects.json` contains:

- `profile`: name, tagline, focus areas, email, profile image path
- `projects[]`: one object per project
- `publications[]`: compact text-first paper/publication entries

Each project supports:

- `slug`
- `title`
- `date`
- `status` (`live`, `concept`, or `prototype`)
- `oneLiner`
- `bannerImage`
- `iconImage`
- `primaryUrl`
- `backupUrl`
- `socials` (optional array)
- `details`
- `pitchDeckUrl` (optional)

Each publication supports:

- `title`
- `date`
- `venue`
- `oneLiner`
- `primaryUrl`
- `backupUrl` (optional)

## Local Preview

Serve with any static server from repo root.

Example with Python:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## GitHub Pages Deployment

1. Push this repo to GitHub on your publishing branch (commonly `main`).
2. In GitHub: **Settings -> Pages**.
3. Set source to **Deploy from a branch**.
4. Select your branch and folder **`/ (root)`**.
5. Save and wait for Pages to publish.

If you use a custom domain, add or keep a root `CNAME` file with your domain value.
