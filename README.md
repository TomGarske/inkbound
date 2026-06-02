# Inkbound — wireframe / stencil

A static one-page wireframe of an NYC Midnight–style writing competition site.

**Live:** https://tomgarske.github.io/inkbound/

## What this is

A placeholder brand ("Inkbound") and a stencil for what the site needs to do:

- **Hero** with pitch, dual CTAs, and a live-stats strip
- **Challenges grid** — 8 challenge formats (100-word micro through 5-page screenplay), each with status (Open / Closed / Coming Soon), next dates, and entry fee
- **How it works** — 3-step funnel mechanic (prompt → anonymous judging → advance + publish)
- **Publishing pathways** — annual anthology, online lit journal, agent intros
- **Recent winners** — placeholder cards (replace with real data after first cycle)
- **Charity callout** — 2% donation framing
- **Testimonials** — placeholder quotes
- **Newsletter signup** — mockup form
- **Footer** — 4-column nav graveyard

## Companion analysis project

[nycm-2026](https://github.com/TomGarske/nycm-2026) — full analytics dashboard on the real NYC Midnight 500-Word Fiction Challenge 2026 field (3,456 writers researched, competitive density scoring, per-writer publishing history). That project's findings shaped what's needed in this stencil.

## What to fill in if this becomes real

- Replace `Inkbound` placeholder with the real brand name (single string, ~15 spots)
- Wire Register / Sign in buttons to a real signup flow
- Set real challenge calendar (current dates are placeholders patterned on NYC Midnight)
- Swap placeholder winner data once a cycle wraps
- Add real testimonial quotes
- Hook newsletter form to an email provider

Pure static HTML + a small inline script, no build step.
