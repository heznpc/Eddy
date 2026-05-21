# Security Policy

## Scope

This repository contains the LaTeX source of a position paper (Zenodo DOI
[10.5281/zenodo.19074337](https://doi.org/10.5281/zenodo.19074337)) and a
GitHub Actions workflow that builds the PDF.

There is no runtime service, no user-data pipeline, and no third-party
package manifest. The relevant trust surfaces are therefore narrow:

- The build workflow (`.github/workflows/build-pdf.yml`) — pinned to
  third-party action commit SHAs and constrained to least-privilege scopes.
- The secret-scan workflow (`.github/workflows/gitleaks.yml`) — runs on push,
  PR, and weekly cron as a defense-in-depth layer over GitHub-native push
  protection.
- The published PDF artifact — signed with SLSA build provenance via
  `actions/attest-build-provenance` on every push to `main`.

## Reporting a vulnerability

Please report security issues by emailing **heznpc@gmail.com** with the
subject line `[security] eddy <short title>`.

You can expect:

- Acknowledgement within 7 days.
- A disposition (fix planned / no-fix with rationale / out of scope) within
  30 days for verifiable supply-chain or workflow issues.

For issues that are about the **research content** of the paper rather than
the repository (e.g., factual errors in the manuscript, citation problems,
methodological concerns), please open a public GitHub Issue or email the
address above with the subject line `[research] eddy <short title>`. Those
are tracked alongside the manuscript revisions, not under this security
policy.

## Out of scope

- General LaTeX rendering quirks that do not affect the published PDF on
  Zenodo.
- Reproducibility of an as-yet-unrun pilot study — see `planning/TODO.md` for
  the experimental roadmap.

## Disclosure preference

Coordinated disclosure preferred. Public disclosure after a fix is published
or after the 30-day window above, whichever comes first.
