# MAPS

**Map. Assess. Prioritize. Sustain.** The AI Tech Pros operating system for NIST SP 800-171, SPRS scoring, and CMMC readiness.

**Version 1.1.0, revised September 29, 2026.** Check the [changelog](CHANGELOG.md) for what changed.

> **Staleness warning.** Cybersecurity regulation moves. This framework is current as of September 2026: CMMC Phase 2 suspended July 13, 2026 pending a reform task force review, DFARS 252.204-7012 still enforced, SPRS self-assessment scores still posted. Before you rely on it, confirm nothing material has changed: check DoD announcements, the current 32 CFR Part 170, and the NIST SP 800-171 revision in force. Subscribe to [The Readiness Room](https://thereadinessroom.substack.com) (free) for framework updates.

Most contractors treat their SPRS score like a grade. It is not a grade. It is a map, and right now the Department of Justice is checking it. Announced DOJ cyber False Claims Act settlements already top $16 million across five cases, from contractors whose paperwork did not match their controls.

MAPS is the operating system a defense contractor installs to fix that gap and keep it fixed:

1. **Map** all 110 NIST SP 800-171 controls to the environment and the evidence
2. **Assess** the true SPRS score (not the aspirational one)
3. **Prioritize** gaps by contract risk, starting with the six never-deferrable controls
4. **Sustain** the score, the evidence, and the POA&Ms so the next look survives

## What's in this repo

- `sprs-cmmc-readiness-field-guide.md` (also `.html`, `.pdf`) — the full field guide: current status as of September 2026, complete 5/3/1 weight tables for all 110 controls, the 32 CFR 170.21 conditional gate, and the MAPS priority order including the 3.13.11 encryption play
- `evidence-index.csv` / `evidence-index.md` — all 110 controls with SPRS weights and fill-in columns for status, evidence, owner, and review date. Step 1: Map.
- `scoring-validation-checklist.md` — the checklist every calculated score must pass. Step 2: Assess.
- `remediation-tracker.csv` / `remediation-tracker.md` — the POA&M log with milestones, owners, and closeout evidence. Steps 3 and 4: Prioritize and Sustain.
- `independent-review-gate.md` — the independent review that must pass before attestation and SPRS posting.
- `CHANGELOG.md` — version history and sources.

## The never-deferrable six

These controls can never sit on a POA&M: **3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4.** If any of them are aspirational in your environment, your score is fiction.

## Ground rules

- SPRS starts at 110 and bottoms at -203. POA&Ms do not raise the score.
- No SSP means no valid score.
- Partial implementation scores as not implemented, except 3.5.3 and 3.13.11.
- Every invoice under a DFARS cybersecurity contract certifies your controls are real. No breach is required. Your own people can file the case and take 15 to 30 percent.

## Before you post to SPRS

Do not post a score to SPRS until: the evidence index is complete for all 110 controls, the scoring validation checklist passes, the independent review gate passes, and management has attested in writing. Posting a score you cannot evidence is a False Claims Act risk.

## What MAPS is not

MAPS is an operating framework, not a certification. It does not make you CMMC certified, it does not replace a C3PAO assessment, and it is not legal advice. If you want this operating system installed in your company in one day, that is the [AI Tech Pros Readiness Sprint](https://aitechpros.ai).

## Attribution

MAPS (Map, Assess, Prioritize, Sustain) by [AI Tech Pros, Inc.](https://aitechpros.ai), Augusta, GA. Nehemiah Harvard, CEO. From [The Readiness Room](https://thereadinessroom.substack.com): SPRS and CMMC readiness for CSRA defense contractors. Subscribe free for framework updates.

## License

MIT. Use it, share it, build on it. See [LICENSE](LICENSE).
