# BISA × Hendrick Automotive Group — Partnership Proposal

Single-page sponsorship pitch site built for BILU International Soccer Academy (BISA),
proposing a field-naming partnership with Hendrick Automotive Group.

No build step — it's one static `index.html` with inline CSS/JS, using GSAP + ScrollTrigger
for scroll-driven reveals and Lenis for smooth scrolling.

## Structure

```
bisa-video/
├── index.html          ← the whole site (styles + markup + script)
├── vercel.json          ← static deploy config
└── public/
    ├── hero.mp4          ← looping background video behind the hero headline
    └── images/           ← photos used across the page (before/after field, gallery, etc.)
```

## Sections

1. Hero — headline + BISA × Hendrick lockup
2. Who Is BISA — tactical-board stat diagram (grid of stats on mobile)
3. Champions Moment — cinematic photo break
4. Vision — before/after field reveal + "Why This Location" (Ladson growth/visibility stats)
5. Impact — financial aid growth, Projeto BILU, country flags
6. Social — Instagram/Facebook growth metrics with animated sparkline cards
7. Field Moment — cinematic photo break
8. Invest — sponsorship tiers
9. CTA — contact

## Running locally

Just open `index.html` in a browser, or serve it so relative paths behave consistently:

```bash
npx serve
```

## Deploying

`vercel.json` is already set up for a static deploy (Vercel: import the repo, no build
command needed, output directory is `.`).

## Notes

- `.gitignore` excludes a handful of legacy image files in `public/images/` that aren't
  referenced anywhere in `index.html` (leftovers from earlier design iterations). They're
  left on disk but not tracked, to keep the repo lean.
