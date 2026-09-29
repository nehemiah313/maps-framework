# Evidence Index

**MAPS, step 1: Map.** Every control needs evidence, or the control is not implemented. This index is the inventory.

## How to use it

`evidence-index.csv` lists all 110 NIST SP 800-171 Rev. 2 controls with their SPRS weights. Fill in one row per control:

- **status**: Implemented, Partial, Planned, or Not Applicable.
- **evidence_artifact**: the document, screenshot, config export, log sample, or ticket that proves the control. Be specific. "Firewall rules export 2026-09-15" beats "firewall."
- **evidence_location**: where the artifact lives (share path, ticket system, repo). If an auditor cannot find it in five minutes, it does not exist.
- **evidence_owner**: the person who keeps it current.
- **last_reviewed**: date the evidence was last confirmed still true.
- **notes**: anything the next reviewer needs to know.

## Rules

1. **Partial counts as not implemented**, except for the two special controls (3.5.3 and 3.13.11), which score on degree of implementation.
2. **Not Applicable needs a written justification** in the notes column. "Does not apply" is not a justification. Explain why the control cannot apply to the environment.
3. **The never-deferrable six must be Implemented with evidence**: 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4. If any of these lacks evidence, stop. Your score is fiction and nothing else in this repo matters yet.
4. **No SSP, no score.** Control 3.12.4 is the System Security Plan itself. Without it, the assessment cannot be completed.
5. Review the whole index at least quarterly. Stale evidence is how good scores become False Claims Act cases.

## Status values and what they do to the score

- **Implemented**: full weight kept. Evidence required.
- **Partial**: full weight lost, except 3.5.3 and 3.13.11, which lose 3 instead of 5 when partially implemented as defined in the field guide.
- **Planned**: full weight lost. A POA&M does not change the score. Plans are for the remediation tracker, not the score.
- **Not Applicable**: nothing lost, but only with a documented justification.

## Before you post to SPRS

Do not post a score to SPRS until every row has a status, every Implemented row has evidence, the independent review gate has passed, and management has attested. See `independent-review-gate.md`. Posting a score you cannot evidence is a False Claims Act risk. Announced DOJ cyber settlements already top $16 million across five cases.

---

MAPS (Map, Assess, Prioritize, Sustain) by AI Tech Pros, Inc., Augusta, GA. https://aitechpros.ai
Framework updates: The Readiness Room, https://thereadinessroom.substack.com (free)
