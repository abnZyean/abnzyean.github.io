# CLAUDE.md — Xyean portfolio site

## What this is
Personal portfolio for Abdullah Al Numan Xyean (licensed architect, founder of Spaceverse Ltd., Dhaka) aimed at
English-speaking 3D ArchViz / architecture employers in Germany. Relocating to Germany in 2027.
Hosted free on GitHub Pages from the `main` branch root.

## Rules
- Single static page: `index.html` (inline CSS + JS). No build step, no frameworks, no npm.
- Every visible string exists in BOTH English and German: `<span lang="en">…</span><span lang="de">…</span>`.
  German must be natural, professional German (Sie-form), not word-for-word translation.
- Practice projects live in `data.js`, synced from the spaceverseltd.com source (`src/constants.ts` + `src/content-de.ts` in repo
  abnZyean/spaceverse-website; all 21 projects, titles/locations/briefs as there; `lead` = its `architectLead`). Re-sync with
  the script pattern in git history (commit "Sync all 21 Spaceverse projects"): EN/DE text and images come from the source,
  the portfolio keeps its own `year`, `status`, `role`, `area` (m²), `by`. Per language each project has `t, loc, d, b, client, area (m²),
  scope, year (period, e.g. "2023 –"), status ("In construction" / "Completed" …), role` (what Xyean personally did —
  shown first in the gallery panel when set). Images: `images/<project-id>/00.webp` (cover, 1600 px), `01…` (gallery, 1400 px),
  `thumb.webp` (720×540 card). Top-level `by` is the credit line in the gallery panel (defaults to Spaceverse Ltd.).
  Academic (`cat: "Academic"`) and competition (`cat: "Competition"`) projects are in `data.js` too, with galleries cropped
  from Xyean's A3 portfolio boards (Drive: ACADEMIC / COMPETITION / PROFESSIONAL PORTFOLIO.pdf). Items without images
  (Bamiyan, Berger Award) stay in the "Also shortlisted & exhibited" list in `index.html`.
- `cv.pdf` is generated from `cv.src.html` (public version: no address, phone, DOB, referees' contacts). Regenerate with
  `google-chrome --headless=new --no-pdf-header-footer --print-to-pdf=cv.pdf cv.src.html`. Keep it at 2 A4 pages.
- `images/og.jpg` (1200×630) is the link-preview image; `favicon.svg` is the tab icon.
- After changing `data.js`, bump the `?v=` on its `<script>` tag in `index.html` (GitHub Pages caches files for 10 min).
- German rule G7: "Architekt/in", "Innenarchitekt/in" and "Landschaftsarchitekt/in" are protected titles in Germany.
  In German text name the discipline (Architektur, Innenarchitektur, Freiraumplanung), never the title for Xyean.
- Never invent facts: no made-up project sizes, years, clients, awards or employers. If a detail is missing,
  leave it out and list it in the PR description as a question for Xyean.
- Keep it fast: WebP images ≤ 400 KB each, max width 1920 px. Lazy-load everything below the fold.
- Must work at 360 px phone width with no horizontal scroll, and in dark mode.

## Facts you may use
- B.Arch, Khulna University · IAB accredited · RAJUK enlisted · 7+ years (residential, mixed-use, institutional)
- Founder, Spaceverse Ltd. (2022), in-house building, interior, landscape teams — spaceverseltd.com
- Teaching: External Lecturer (part-time), Department of Architecture, HSTU Dinajpur, Jan–Apr 2026 (past). No Khulna University
  teaching on the site — Xyean's decision 2 Nov 2026: the signed CV (22 Sep 2026) is authoritative for every conflict.
- Certified Rhinoceros Professional · D5 Certified User · Rhino/Grasshopper, AutoCAD, D5 Render
- IELTS Academic 7.0 (C1) · German: A2 course level, working towards B2
- Projects: High Tech Park Mymensingh (thesis, 2026 degree show) · "Pause in a Motion" metro station ·
  Bamiyan Cultural Centre (competition, shortlisted, UNESCO) · Berger Award (shortlisted) · Ma Matin Library ·
  Ma O Shishu Hospital (PM + construction detailing, JV) · Spaceverse: Silicon Europa, Rasel Residence,
  BISC Nirjhor, CMTD, Dostogir House, Residence Triplex expansion
- From Xyean's signed CV (22 Sep 2026) and employer letters: Spaceverse Ltd. founder & lead architect Jul 2022– ·
  External Lecturer (part-time) HSTU Dinajpur Jan 2026– ("Computer Graphics" ARC-222) · Architect (part-time) Nippon Koei
  Bangladesh Ltd. Feb 2024–Feb 2025 (SCRDP for LGED; 2,260 h) · Architect, VolumeZero Ltd. Feb 2020–Jul 2022 (6,215 h) ·
  Assistant Architect, Age & Edge Sep 2019–Jan 2020 · Intern, Bose & Partners Aug 2017–Sep 2018 · B.Arch graduated Jul 2019,
  202.5 credits · IAB Accredited Member & RAJUK enlisted since Dec 2022 · Rhino Certified Professional L1 Oct 2020 ·
  D5 Certified User Sep 2025 · IELTS 7.0 Dec 2024 · German courses A1.1–A2.1 (Deutsch Akademie) · PICC competition
  shortlisted Apr 2024 · Berger Award Mar 2023 · Dolpur housing exhibition Nov 2019 · IEB Convention Centre 2017 ·
  Bamiyan Feb 2015 · IJMRAP paper 2021 (co-author) · AAKAr sports & cultural manager Feb 2022– · founder of Smart Home
  Mentor (smarthomentor.com). Project roles with dates: Silicon Heights (Sep 2024–), Divisional Training Centre
  (Feb 2024–Feb 2025, for Nippon Koei), Ma Matin Library (Feb 2023–), Single-family Triplex, Mymensingh (Feb 2025–),
  Ma O Shishu Healthcare Clinic (Feb 2025–). Where older CVs or portfolio boards disagree, the signed CV wins.
  The CV's "Single Family Triplex, Mymensingh" is mapped to spaceverseltd.com's Chayabithi Triplex (Gazipur, client Dostogir
  Family) — location shown as Gazipur per the project source; Xyean to confirm whether the CV's "Mymensingh" is a typo.
- From the portfolio boards: thesis "High Tech Park" Studio X, supervisor Dr. Anirban Mostafa, physical model ·
  "Pause in Motion" Studio V metro station · PICC 2024: concept development, plan/presentation drawings · IEB Convention
  Centre 2017 (Agargaon): 3D visualisation + graphic post-production, team Ratul/Yasmin/Imam/Riyadh · Public Library
  Shahbag 2017: same role, team Ratul/Emran/Riyadh · "Land is More" Affordable Housing Dolpur, Savar 2019: same role,
  team Ratul/Yasmin/Abbas · Ma O Shishu board: Uttara, 670 m² site, FAR 5.5, JV with MAIN Arch, PM + construction
  detail drawings (board; CV dates used) · Ma Matin board says project year 2018–19 (CV Feb 2023– used).
- Live LinkedIn URL: https://www.linkedin.com/in/architect-zyean/ (abdullah-numan-architecture redirects to it).
- Name: Abdullah Al Numan Xyean (legal spelling on passport/certificates; Xyean's decision 2 Nov 2026: use Xyean on the site
  and CV). The GitHub handle/URL abnzyean and the email abnzyean@gmail.com keep the old spelling.

## Good next tasks (one per session)
1. Fill `role` and `year` for the 10 practice projects that still have none (ask Xyean) — see the PR questions list.
2. Add Bamiyan Cultural Centre and Berger Award images once Xyean supplies them (not in the Drive portfolios).
3. Add process material for the ArchViz target: clay/wireframe → final pairs, day/night of one view, a Grasshopper study, a short reel.
4. Add a one-line work-permit/visa status in the hero summary once Xyean confirms it.
5. Add a German-HOAI-phase label (LP 1–9) to each project once he confirms which phases he did.
6. Lighthouse pass: performance, accessibility, SEO ≥ 95.
