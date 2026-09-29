# Remediation Tracker

**MAPS, steps 3 and 4: Prioritize and Sustain.** Gaps get sequenced by contract risk and closed on a schedule. This tracker is the schedule.

## How to use it

`remediation-tracker.csv` is the POA&M log. One row per open gap:

- **poam_id**: your own tracking number (for example POAM-2026-014).
- **control**: the control number, for example 3.8.8.
- **weight**: 5, 3, or 1 (or 5/3 for the specials). This sets the priority.
- **gap_description**: what is missing, in one sentence.
- **milestones**: dated, verifiable steps. "Draft procedure Oct 15; train staff Nov 30." Not "work on it."
- **scheduled_close_date**: the date the control will be Implemented with evidence.
- **owner**: one named person. Not a team, a person.
- **status**: Open, In Progress, Awaiting Evidence, Closed.
- **closeout_evidence**: the artifact proving the control is now implemented. Closing a POA&M without evidence just moves the fiction.
- **notes**: blockers, dependencies, context.

## Rules that actually matter

1. **The never-deferrable six can never be on a POA&M**: 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4. Close them outright, with evidence, before anything else.
2. **Conditional status has a clock.** Under 32 CFR 170.21, POA&M items must be closed within 180 days of the Conditional status date and confirmed by a closeout assessment, or the status expires.
3. **Conditional status has a weight limit.** Every open item on the POA&M must be worth 1 point. One exception: 3.13.11 at minus 3 (encryption in use but not FIPS-validated) may be deferred. If your POA&M holds anything heavier, you do not qualify.
4. **A POA&M does not change your SPRS score.** The score reflects what is implemented today. The tracker is how you get from today's score to the target score. Do not confuse the two.
5. **Sequence by the MAPS priority order**: never-deferrable six first, then open 5-point controls (family with the most gaps first), then the 3.13.11 encryption play (implement encryption now even before FIPS validation to convert a disqualifying 5-point hit into a deferrable 3-point item), then 3-point controls, then 1-point controls.
6. **Review open items weekly.** A POA&M nobody looks at is a plan to miss the 180-day clock.

## Closing an item

An item is closed when all three are true: the control is implemented, evidence is recorded in the evidence index, and the closeout evidence is linked in this tracker. Two out of three is still open.

---

MAPS (Map, Assess, Prioritize, Sustain) by AI Tech Pros, Inc., Augusta, GA. https://aitechpros.ai
Framework updates: The Readiness Room, https://thereadinessroom.substack.com (free)
