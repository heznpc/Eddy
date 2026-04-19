# Research Decisions Log

Records non-obvious choices with rationale. Append-only; don't rewrite history.

Format: `## YYYY-MM-DD -- <short title>` with **Context**, **Decision**, **Why**.

---

## 2026-04-19 -- Repository restructure to DDD-style layout + paper/latex flattening

**Context**: Manuscript lived at `paper/latex/main.tex` with CI triggered on `paper/latex/**`. The extra `latex/` directory served no purpose and deviated from the portfolio convention.

**Decision**: Flatten to `paper/main.tex`. Update `.github/workflows/build-pdf.yml` paths (trigger, working_directory, PDF output). Update .gitignore to `**/acmart.cls` (allowing acmart anywhere under paper/).

**Why**: Consistency with the rest of the portfolio. CI behavior is preserved; only paths change.

---

## 2026-04-19 -- PDF continues to be committed by CI

**Context**: Most portfolio repos gitignore paper/main.pdf. Eddy's CI force-adds and commits the PDF after build.

**Decision**: Leave this behavior untouched for now.

**Why**: Changing CI publishing policy is a separate decision. The PDF in git history serves a preprint-distribution purpose (arXiv submission pipeline).
