# nerom.site

The portfolio of **nerom**, a product engineer who builds AI agents, web apps, payment flows and on-chain systems. Live at **[nerom.site](https://nerom.site)**.

## What's here

It's one static page with no build step:

- **Hero:** the `nerom.` wordmark assembles from masked slices, next to a 3D stack of live product screens.
- **Selected work:** featured projects. Each live site scrolls inside its frame as you scroll past.
- **Built for clients:** client builds.
- **The archive:** every project, ranked, with filters and a cursor preview.
- **How a build runs:** the process, followed by a project-brief builder that writes the email for you.
- **Palettes:** four of them (Mono, Cobalt, Acid, Light), switched from the header with a circular reveal.
- **Case pages:** each project has a full-screen page you can link to, e.g. `nerom.site/#ropes`.

## Structure

```
index.html   page, styles, data (CARDS) and behaviour
shots/       800×500 thumbnails (archive preview)
full/        1440×900 images (case pages)
long/        full-page captures that scroll inside featured frames
og.png       social preview image
vercel.json  headers
```

Projects live in the `CARDS` array in `index.html`. Ranking is the `BEST` list, featured projects are in `FEAT`, and client builds are in `CLIENTS`.

## Run locally

```bash
python3 -m http.server 4178
```

## Deploy

Hosted on Vercel:

```bash
npx vercel@latest deploy --prod
```

Smooth scrolling uses [Lenis](https://github.com/darkroomengineering/lenis) from a CDN. Fonts: Inter Tight, Cormorant Garamond, JetBrains Mono.
