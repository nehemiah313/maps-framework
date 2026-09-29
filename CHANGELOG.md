# Changelog

All notable changes to the MAPS framework. Dates are publication dates.

## 1.1.0 - 2026-09-29

The operational pack. The framework now covers the full lifecycle: map, assess, prioritize, sustain.

Added:

- `evidence-index.csv` and `evidence-index.md`: all 110 NIST SP 800-171 Rev. 2 controls with SPRS weights, never-deferrable flags, and special scoring notes, plus fill-in columns for status, evidence artifact, location, owner, and review date.
- `remediation-tracker.csv` and `remediation-tracker.md`: POA&M log template with milestone, owner, and closeout-evidence fields, plus the rules that govern POA&Ms under 32 CFR 170.21.
- `scoring-validation-checklist.md`: the MAPS Assess gate. Run it on every calculated score.
- `independent-review-gate.md`: the review that must pass before management attestation and SPRS posting.
- Staleness warnings and revision dates across the repo.
- Explicit warning: do not post a score to SPRS without complete evidence review, a passed independent review gate, and management attestation.
- Non-certification notice: MAPS is an operating framework, not a certification path, with a Readiness Sprint call to action.

Corrected:

- README now cites the verified figure: announced DOJ cyber False Claims Act settlements top $16 million across five cases. The earlier $52 million FY2025 figure could not be verified and has been removed everywhere.

## 1.0.0 - 2026-09-28

Initial release. The field guide: current status as of September 2026, complete 5/3/1 weight tables for all 110 controls, the 32 CFR 170.21 conditional gate (score 88+, only 1-pointers on POA&M, the never-deferrable six), the MAPS priority order including the 3.13.11 encryption play, and the DFARS clause cheat sheet. Published as markdown, HTML, and PDF under the MIT license.

## Sources (all versions)

- NIST SP 800-171 Rev. 2 and the DoD Assessment Methodology (scoring weights and methodology)
- 32 CFR Part 170, including 170.21 (POA&M and Conditional status) and 170.24 (scoring methodology)
- DFARS 252.204-7012, 252.204-7019, 252.204-7020, 252.204-7021; FAR 52.204-21
- DoD CIO memorandum, July 13, 2026 (Phase 2 suspension and reform review)
