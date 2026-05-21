# eddy

Research Program: 2 (Epistemic Failure and Correction)
Status: Published / DOI
Relationship to other work: Companion to ploidy (Program 2 anchor)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19074337.svg)](https://doi.org/10.5281/zenodo.19074337)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Build PDF](https://github.com/heznpc/eddy/actions/workflows/build-pdf.yml/badge.svg?branch=main)](https://github.com/heznpc/eddy/actions/workflows/build-pdf.yml)

**Position: ADHD as Competitive Advantage in AI-Augmented Multi-Project Orchestration**

In AI-augmented multi-session workflows, the remaining cognitive step after switching is re-engagement. ADHD brains may perform this step *faster* than neurotypical brains because their attentional system is optimized for rapid stimulus-locking. When AI context retention removes the context-reconstruction bottleneck, only the step where ADHD has an advantage remains. This position paper proposes the hypothesis, specifies boundary conditions (AI context quality, medication effects, switch propensity), and outlines a falsifiable experimental design.

## Paper

- `paper/main.tex` — position paper (no experimental results yet; pilots forthcoming)
- Published artifact: [10.5281/zenodo.19074337](https://doi.org/10.5281/zenodo.19074337)
- Venue targets: ASSETS 2026 (deadline 2026-06-24), then CHI 2027

## Repository structure

```
eddy/
  paper/                      Domain -- manuscript source of truth (main.tex, figures/)
  experiments/                Application -- skeleton; pilots forthcoming
  literature/                 Reading notes, gap analysis
  planning/                   TODO, review, decisions log, drafts
  submissions/                Venue adaptations (e.g. assets-2026/)
  .github/workflows/          CI: build PDF on push to paper/**
```

## Design intent

- ADHD framed as **environment-adaptation mismatch**, not deficit.
- Boundary conditions are specified up front rather than treated as caveats.
- Position paper first, clinical-population pilots forthcoming — falsifiability before fieldwork.

## Status

Published as a Zenodo position paper. Seeking collaborators with access to clinical ADHD populations for empirical validation. Venue work tracked in `submissions/` and `planning/TODO.md`.

## License

CC-BY 4.0
