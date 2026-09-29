# MAPS

**Map. Assess. Prioritize. Sustain.** The AI Tech Pros operating system for NIST SP 800-171, SPRS scoring, and CMMC readiness.

Most contractors treat their SPRS score like a grade. It is not a grade. It is a map, and right now the Department of Justice is checking it. In FY2025 alone, DOJ collected $52 million in cyber False Claims Act settlements from contractors whose paperwork did not match their controls.

MAPS is the one-day operating system a defense contractor installs to fix that gap and keep it fixed:

1. **Map** all 110 NIST SP 800-171 controls to the environment and the evidence
2. **Assess** the true SPRS score (not the aspirational one)
3. **Prioritize** gaps by contract risk, starting with the six never-deferrable controls
4. **Sustain** the score, the evidence, and the POA&Ms so the next look survives

## What's in this repo

- `sprs-cmmc-readiness-field-guide.md` — the full field guide: current status as of September 2026, complete 5/3/1 weight tables for all 110 controls, the 32 CFR 170.21 conditional gate (score 88+, only 1-pointers on POA&M, the never-deferrable six), and the MAPS priority order including the 3.13.11 encryption play
- `sprs-cmmc-readiness-field-guide.html` / `.pdf` — the same guide as a printable page and PDF

## The toolkit: use it, don't just read it

Three working files that turn the framework into something you can run:

- `controls-assessment.csv` — all 110 controls with their DoD weights (42 at 5 points, 14 at 3, 52 at 1, plus the two special-scored controls 3.5.3 and 3.13.11). Open it in any spreadsheet, fill in the `status` column (Implemented, Planned, or N/A) for each control, note your evidence, and flag POA&M items. Your SPRS score is 110 minus the weights of everything not implemented.
- `self-assessment-checklist.md` — the same 110 controls as a plain-English checklist grouped by family, each with its weight and a line on what an assessor actually looks for. Check a box only when you have evidence you could show an assessor.
- `poam-template.csv` — a POA&M template with three example rows: two showing what a credible entry looks like (specific weakness, real dates, named owner, resourced milestones) and one showing the vague style that fails scrutiny. Delete the examples and write your own.

How to run your self-assessment in an afternoon:

1. Download `controls-assessment.csv`.
2. For each control, mark Implemented only if you can point to evidence today. Everything else is Planned or N/A.
3. Score: 110 minus the weights of every non-implemented control. Floor is -203.
4. Every Planned control gets a row in the POA&M. Remember: POA&Ms do not raise the score, and the six never-deferrable controls below can never sit on one.

## The never-deferrable six

These controls can never sit on a POA&M: **3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4.** If any of them are aspirational in your environment, your score is fiction.

## Ground rules

- SPRS starts at 110 and bottoms at -203. POA&Ms do not raise the score.
- No SSP means no valid score.
- Every invoice under a DFARS cybersecurity contract certifies your controls are real. No breach is required. Your own people can file the case and take 15 to 30 percent.

Built by [AI Tech Pros](https://aitechpros.ai), Augusta, GA. From *The Readiness Room*: SPRS and CMMC readiness for CSRA defense contractors.

## License

MIT. Use it, share it, build on it.
