# Scoring Validation Checklist

**MAPS, step 2: Assess.** Run this checklist every time you calculate a SPRS score. A score that fails any check is not a score, it is a guess.

## Before calculating

- [ ] A System Security Plan exists and describes the environment being scored (3.12.4). No SSP, no score.
- [ ] The evidence index has a status for all 110 controls.
- [ ] Every control marked Implemented has an evidence artifact recorded.
- [ ] Every control marked Not Applicable has a written justification.
- [ ] The environment being scored matches the SSP: same systems, same boundary, same CUI flow. A score for a different environment is fiction.

## The arithmetic

- [ ] Start at 110.
- [ ] Subtract 5 for each unimplemented 5-point control (42 of them).
- [ ] Subtract 3 for each unimplemented 3-point control (14 of them).
- [ ] Subtract 1 for each unimplemented 1-point control (52 of them).
- [ ] Score 3.5.3 (MFA): minus 5 if MFA is absent entirely, minus 3 if implemented for remote and privileged users but not all users, 0 if fully implemented.
- [ ] Score 3.13.11 (FIPS-validated encryption): minus 5 if no FIPS-validated cryptography, minus 3 if encryption is in use but not FIPS-validated, 0 if fully implemented.
- [ ] Partial implementation scores as not implemented, except the two specials above.
- [ ] Controls marked Not Applicable subtract nothing.
- [ ] POA&M items subtract their full weight. Plans do not raise the score.
- [ ] Sanity check: the result is between -203 and 110. If it is not, the arithmetic is wrong.

## The never-deferrable six

- [ ] 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, and 3.12.4 are all marked Implemented.
- [ ] Each of the six has evidence recorded.
- [ ] None of the six appears on the POA&M.

## The Conditional gate (only if targeting Conditional status)

- [ ] Score is 88 or higher.
- [ ] Every open POA&M item is worth 1 point, except 3.13.11 at minus 3 which may be deferred.
- [ ] No 5-point or 3-point control sits on the POA&M.
- [ ] The 180-day closeout clock has a named owner watching it.

## After calculating

- [ ] The score was re-performed independently (see `independent-review-gate.md`).
- [ ] Management attested to the score in writing.
- [ ] The score, the evidence index, and the attestation are stored together with the same date.

Only then is the score ready to post to SPRS.

---

MAPS (Map, Assess, Prioritize, Sustain) by AI Tech Pros, Inc., Augusta, GA. https://aitechpros.ai
Framework updates: The Readiness Room, https://thereadinessroom.substack.com (free)
