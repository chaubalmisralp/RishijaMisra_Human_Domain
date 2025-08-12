# Rishija Misra — Personal Domain (Static Site)

This is a **static, single-page site** that loads all content from small JSON files under `/data`.
No build tools required. Just host the folder on Netlify, GitHub Pages, Vercel, or any static host.

## Files
- `index.html` – page markup and loader
- `style.css` – page styles
- `data/header.json` – name, tagline, LinkedIn, email, short bio
- `data/photo.json` – profile image path/alt
- `data/career.json` – professional timeline
- `data/education.json` – education timeline
- `assets/placeholder.jpg` – replace with a real photo

## How to edit
1. Replace values in `/data/*.json` with your own.
2. Put your headshot in `/assets` and update `data/photo.json` → `"src": "./assets/yourphoto.jpg"`.
3. Add more timeline entries by appending objects to the arrays in `career.json` and `education.json`.

## Deploy
- **Netlify**: drag this folder to Netlify Drop, done.
- **GitHub Pages**: push to a repo, enable Pages.
- **Vercel**: import the repo and deploy as static.

## Notes
- We did not scrape LinkedIn (they block bots). Copy relevant details manually into the JSON files.
- The site does not track or store data; it just reads local JSON files at load time.
