# newslarp

A single-page, made-up Lithuanian news article from the made-up portal **„Šiaurės Pulsas“** ("Northern Pulse"): **"Atrasta nauja begemotų rūšis: naktį švytinti Genny nustebino mokslininkus"**. It reports the discovery of *Choeropsis nyctolumen*, a pygmy hippo species whose skin glows in moonlight, and Genny, the first of its kind to be described.

It's a plain static site: no framework, no build step, nothing to install.

## Deploy on Vercel

**From the dashboard**

1. Go to [vercel.com/new](https://vercel.com/new) and import the `newslarp` GitHub repo.
2. Click **Deploy**. Leave the settings as they are: `vercel.json` sets the framework, build command and output folder.

**From the command line**

```bash
npx vercel          # preview deploy
npx vercel --prod   # production deploy
```

Opening the site's home page takes you to a news-style article URL:

```
https://<your-project>.vercel.app/  →  /mokslas/2026/10/12/atrasta-nauja-begemotu-rusis-genny
```

Vercel deploys the repo's default branch, which is currently `claude/festive-noether-rwtjml`.

## Files

```
public/index.html    the article page (styles, illustrations and scripts inline; fonts from Google Fonts)
public/404.html      "page not found" page in the same style
public/favicon.svg   the „Šiaurės Pulsas“ tab icon
vercel.json          static-site settings, plus the redirect and rewrite for the article URL
```

Only `public/` is served, so this README and `vercel.json` are not published.

## Preview locally

```bash
npx serve public
```

Or open `public/index.html` directly in a browser.

## What's on the page

- News-portal layout: masthead, section nav, breaking-news ticker, sidebar with "most read" and "latest"
- Hand-drawn SVG illustration of Genny at night, plus a camera-trap frame
- Fact box, pull quote, tags and related stories
- Working extras: copy link / share, text size A−/A+, comment form and likes

„Šiaurės Pulsas“, the journalist and the scientists are all invented.
