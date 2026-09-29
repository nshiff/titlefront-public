# Titlefront Website

The public marketing site for Titlefront, a one-page site built with [Astro](https://astro.build). It's fully static and ships no client-side JavaScript.

## Requirements

- Node.js 22 or newer
- npm

## Getting started

```bash
npm install
npm run dev
```

The dev server runs at http://localhost:4321 and reloads as you edit.

## Commands

| Command           | What it does                                        |
| ----------------- | --------------------------------------------------- |
| `npm run dev`     | Start the local dev server                          |
| `npm run build`   | Type-check (`astro check`) and build to `dist/`     |
| `npm run preview` | Serve the built `dist/` folder locally              |

## Deployment

The build output is plain static files in `dist/`, so any static host works.

- **Build command:** `npm run build`
- **Publish directory:** `dist`

On Render, create a Static Site with those two settings. On Cloudflare Pages, use the same build command and output directory.

## Adding interactivity later

Nothing here needs JavaScript today. If a contact form or other interactive piece is added later, Astro can use React components as islands:

```bash
npx astro add react
```

Then use the component with a `client:*` directive so only that piece ships JavaScript.
