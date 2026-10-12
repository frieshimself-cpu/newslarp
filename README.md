# newslarp

A single-page, made-up Lithuanian news article from the made-up portal **„Šiaurės Pulsas“** ("Northern Pulse"): **"Atrasta nauja begemotų rūšis: naktį švytinti Genny nustebino mokslininkus"**. It reports the discovery of *Choeropsis nyctolumen*, a pygmy hippo species whose skin glows in moonlight, and Genny, the first of its kind to be described.

It's a plain static site. There's no build step and nothing to install.

## Deploy on Vercel

1. Go to [vercel.com/new](https://vercel.com/new) and import this GitHub repo.
2. Leave every setting as it is (Framework Preset: **Other**, no build command) and click **Deploy**.

`vercel.json` sends visitors from the home page to a news-style article URL:

```
https://<your-project>.vercel.app/  →  /mokslas/2026/10/12/atrasta-nauja-begemotu-rusis-genny
```

Vercel deploys from the repo's production branch (usually `main`). Merge this branch into it, or set the branch under Project → Settings → Git.

## Files

- `index.html`: the whole page (styles, illustrations and scripts inline; fonts from Google Fonts)
- `favicon.svg`: the "Šiaurės Pulsas" tab icon
- `vercel.json`: redirect and rewrite for the article URL
- `.vercelignore`: keeps this README out of the deploy

## What's on the page

- News-portal layout: masthead, section nav, breaking-news ticker, sidebar with "most read" and "latest"
- Hand-drawn SVG illustration of Genny at night, plus a camera-trap frame
- Fact box, pull quote, tags and related stories
- Working extras: copy link / share, text size A−/A+, comment form and likes

"Šiaurės Pulsas", the journalist and the scientists are all invented.
