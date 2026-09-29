# Score Honestly: Your SPRS Submission Is a Sworn Statement

> **Created by AI Tech Pros (aitechpros.ai).** Free 90-second SPRS estimator: https://aitechpros.ai/sprs-score. The Readiness Room newsletter: https://thereadinessroom.substack.com

Read this before you fill in a single status cell in `controls-assessment.csv`. An inflated SPRS score does not just lose you a contract. It can become the government's Exhibit A.

## The LOGZONE cautionary tale

In 2021, a defense contractor self-reported a perfect SPRS score of 110. In February 2024, the Defense Industrial Base Cybersecurity Assessment Center (DIBCAC) assessed the same environment and scored it at negative 170. On June 18, 2026, the company settled False Claims Act allegations for $507,144.

The gap between the claimed score and the real score was the case. Nobody had to prove a breach. Nobody had to prove an adversary exploited anything. The paperwork did not match the controls, and that mismatch was enough.

## The legal reality

Your SPRS score is not a marketing number. When you post a score to SPRS under DFARS 252.204-7019 and 7020, your company is attesting that the score reflects an actual assessment of the 110 NIST SP 800-171 controls against your System Security Plan.

That attestation follows you:

- Every invoice you submit under a contract containing DFARS 252.204-7012 is a claim for payment that implies your cybersecurity representations were true.
- The False Claims Act allows the government to pursue treble damages for knowing misrepresentations, and it allows private whistleblowers (qui tam relators, including your own employees) to file the case and collect 15 to 30 percent of the recovery.
- "Knowing" under the FCA includes reckless disregard. You do not have to intend fraud. Scoring controls you never tested, or marking Planned work as Implemented, can qualify.
- Recent cyber FCA settlements in 2025 and 2026 include multi-million-dollar cases, all whistleblower-initiated.

## The five score-inflation traps

These are the five patterns that turn a self-assessment into an FCA exhibit. Check yourself against each one before you post.

### 1. Marking Planned controls as Implemented

Implemented means the control is in place and working today, with evidence you could show an assessor this afternoon. If the firewall rule is "on the roadmap," the MFA rollout is "in progress," or the logging "mostly works," the control is Planned, not Implemented. Aspirational scoring is the most common trap and the easiest for an assessor to disprove.

### 2. Treating POA&M items as Implemented

A Plan of Action and Milestones is a promise to fix something, not proof that it is fixed. POA&Ms do not raise your score. If a control has an open POA&M item, it is not implemented. Full stop. Six controls can never sit on a POA&M at all: 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4.

### 3. Scoring without an SSP

No System Security Plan means no valid score. The assessment methodology assesses the SSP; without one, there is nothing to assess against. If you do not have an SSP yet, your first job is writing one (this repo includes `ssp-template.md`), not picking a number.

### 4. Taking partial credit wrong on the specials

Two controls have special scoring: 3.5.3 (multifactor authentication) and 3.13.11 (FIPS-validated encryption). Each scores 5 points if fully implemented or 3 if partially implemented. Partial is not full. MFA on email but not on workstation logons is partial. Encryption that is not FIPS-validated is partial. Claiming the full 5 when you earned the 3 is inflation.

### 5. Scoring controls you never tested

A control that exists on paper but was never validated is not implemented. If you have never tested your incident response plan, never verified that your backups restore, or never confirmed that terminated users actually lose access, those controls are aspirational. Assessors test. Score only what you have proven.

## What this toolkit is

This toolkit organizes your self-assessment. It does not verify it. The CSV structures your scoring, the checklist structures your evidence review, and the templates structure your SSP and POA&M. Verification is a separate job, and it is the job that matters.

If you want an independent set of eyes on your score before you post it, AI Tech Pros runs a one-day Readiness Sprint: we map your controls to your environment, assess your true score, and hand you a POA&M prioritized by contract risk. Start with the free 90-second estimator at https://aitechpros.ai/sprs-score, or reach us through https://aitechpros.ai.

Score what is real. Post what you can prove.
