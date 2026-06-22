# Karolina Kordas — Marketing Portfolio

A single-page React site: a Moroccan door entry, an About page, an
Experience page, and three marketing-campaign deep dives.

## Going live — Vercel (recommended, free)

1. Go to https://vercel.com and sign up (you can sign in with GitHub,
   Google, or email — no credit card needed).
2. Once you're in, click **Add New → Project**.
3. You'll be asked to import a Git repository. The simplest path:
   - Go to https://github.com and create a free account if you don't
     have one.
   - Create a **new repository** (e.g. `karolina-portfolio`), and
     upload all the files in this folder to it (GitHub's website lets
     you drag-and-drop files directly — no command line needed).
   - Back in Vercel, click **Import** next to that repository.
4. Vercel will auto-detect this is a Vite project. Leave all settings
   on default and click **Deploy**.
5. After about a minute, you'll get a live link like
   `https://karolina-portfolio.vercel.app` — that's your website.

Every time you (or I) update the code and re-upload it to the same
GitHub repository, Vercel automatically rebuilds and updates the live
site within a minute or two.

## Going live — Netlify (alternative, also free)

1. Go to https://app.netlify.com and sign up.
2. Click **Add new site → Import an existing project**, and connect
   the same GitHub repository as above.
3. Build command: `npm run build`. Publish directory: `dist`.
4. Click **Deploy** — you'll get a link like
   `https://karolina-portfolio.netlify.app`.

## Custom domain (optional, later)

Both Vercel and Netlify let you attach a real domain (e.g.
`karolinakordas.com`) for free if you buy one separately from a
registrar like Namecheap or Google Domains — you'd add it under each
project's **Domains** settings and follow their DNS instructions.

## Running it locally (optional)

If you ever want to preview changes on your own computer before
pushing them live:

```bash
npm install
npm run dev
```

This starts a local server (usually at `http://localhost:5173`) where
you can see the site update live as files change.

To produce the production build manually:

```bash
npm run build
```

This creates a `dist/` folder containing the finished static site,
which is what actually gets hosted.
