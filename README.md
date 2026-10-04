# DDR4 & DDR5 - Learning

A complete, beginner-friendly course on DDR memory - from "what is a RAM stick" all the way
to DDR4 internals, the DDR5 upgrades, reading the JEDEC specs, hands-on practice, and picking
a specialization. **49 short, illustrated lessons** across 6 phases.

## Read it as a website

The lessons are a static HTML site (hosted with GitHub Pages):

**→ https://hashinisraq.github.io/ddr-study-roadmap/**

Open that link, start at Phase 0 / Lesson 1, and click **Next** through the whole course. Every
lesson has Previous / Next links and inline diagrams, circuits, and waveforms.

> If the link 404s, GitHub Pages isn't enabled yet: in the repo go to
> **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `root`**,
> then wait a minute for the first build.

## The phases

| Phase | What it covers |
|-------|----------------|
| 0 - Foundations | What memory is, the stick/chips/rank/bank big picture, then the physics of a DRAM bit |
| 1 - DDR4 Core | Organization, commands, the bank state machine, timings, refresh, training, electrical |
| 2 - DDR5 Delta | What DDR5 changed over DDR4 and why (sub-channels, BL16, on-die ECC, DFE, PMIC, ...) |
| 3 - Specs & Datasheets | How to read the JEDEC specs and real datasheets without drowning |
| 4 - Hands-on | Exercises: trace a transaction, run a simulator, change timings and predict |
| 5 - Specialization | Pick a track: controller / validation / signal integrity / firmware / architecture |

## Repository layout

```
index.html              the course home page (links every lesson)
assets/lesson.css        shared styling for all lesson pages
phase-N-.../lessons/     the lesson pages (.html) for that phase
```

Each lesson is a self-contained HTML page with inline SVG diagrams - no build step, no
dependencies. To read offline, just open `index.html` in any browser.

## A note on the JEDEC specs

The official DDR4/DDR5 standards (JESD79-4, JESD79-5) are **copyrighted** and are **not**
included in this public repository (see [`.gitignore`](.gitignore)). Download them for free,
with an account, from [jedec.org](https://www.jedec.org). Phase 3 explains how to read them.

## License / use

Educational material written for self-study. The explanations and diagrams here are original;
the JEDEC standards they describe belong to JEDEC and are not distributed here.
