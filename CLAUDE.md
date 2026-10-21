# CLAUDE.md — Zyean portfolio site

## What this is
Personal portfolio for Abdullah Al Numan Zyean (licensed architect, founder of Spaceverse Ltd., Dhaka) aimed at
English-speaking 3D ArchViz / architecture employers in Germany. Relocating to Germany in 2027.
Hosted free on GitHub Pages from the `main` branch root.

## Rules
- Single static page: `index.html` (inline CSS + JS). No build step, no frameworks, no npm.
- Every visible string exists in BOTH English and German: `<span lang="en">…</span><span lang="de">…</span>`.
  German must be natural, professional German (Sie-form), not word-for-word translation.
- Practice projects live in `data.js` (generated from the spaceverseltd.com source: `src/constants.ts` + `src/content-de.ts`
  in repo abnZyean/spaceverse-website). Images: `images/<project-id>/00.webp` (cover, 1600 px), `01…` (gallery, 1400 px),
  `thumb.webp` (720×540 card). Academic/competition items are in the "Academic & competitions" list in `index.html`.
- German rule G7: "Architekt/in", "Innenarchitekt/in" and "Landschaftsarchitekt/in" are protected titles in Germany.
  In German text name the discipline (Architektur, Innenarchitektur, Freiraumplanung), never the title for Zyean.
- Never invent facts: no made-up project sizes, years, clients, awards or employers. If a detail is missing,
  leave it out and list it in the PR description as a question for Zyean.
- Keep it fast: WebP images ≤ 400 KB each, max width 1920 px. Lazy-load everything below the fold.
- Must work at 360 px phone width with no horizontal scroll, and in dark mode.

## Facts you may use
- B.Arch, Khulna University · IAB accredited · RAJUK enlisted · 7+ years (residential, mixed-use, institutional)
- Founder, Spaceverse Ltd. (2022), in-house building, interior, landscape teams — spaceverseltd.com
- Part-time teaching staff, Architecture Discipline, Khulna University
- Certified Rhinoceros Professional · D5 Certified User · Rhino/Grasshopper, AutoCAD, D5 Render
- IELTS Academic 7.0 (C1) · German: A2 course level, working towards B2
- Projects: High Tech Park Mymensingh (thesis, 2026 degree show) · "Pause in a Motion" metro station ·
  Bamiyan Cultural Centre (competition, shortlisted, UNESCO) · Berger Award (shortlisted) · Ma Matin Library ·
  Ma O Shishu Hospital (PM + construction detailing, JV) · Spaceverse: Silicon Europa, Rasel Residence,
  BISC Nirjhor, CMTD, Dostogir House, Residence Triplex expansion

## Good next tasks (one per session)
1. Mark which projects Zyean personally led / modelled / rendered (ask him) and show that role in the gallery panel.
2. Add academic work images (High Tech Park, Pause in a Motion, Bamiyan) once Zyean supplies them.
3. Generate `cv.pdf` from a CV he provides, linked from the contact section.
4. Add a German-HOAI-phase label (LP 1–9) to each project once he confirms which phases he did.
5. Lighthouse pass: performance, accessibility, SEO ≥ 95.
