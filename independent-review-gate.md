# Independent Review Gate

Nobody grades their own homework. Before a SPRS score is attested or posted, it passes through this gate. The reviewer must be qualified to assess NIST SP 800-171 and must not be the person who performed the self-assessment.

## What the reviewer does

1. **Re-perform the scoring.** Independently re-score a sample of at least 20 controls spanning all 14 families, including every control the assessment marked Implemented at 5 points. If the re-performed sample disagrees with the assessment on any control, expand the sample until the disagreement is explained or the assessment is redone.
2. **Test the evidence.** For each sampled Implemented control, open the recorded evidence artifact. Confirm it exists, is current, and actually demonstrates the control. Evidence older than the last significant environment change gets flagged.
3. **Challenge every Not Applicable.** Read each justification. Confirm the control genuinely cannot apply to the environment. A weak justification becomes a finding.
4. **Verify the never-deferrable six.** Confirm 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, and 3.12.4 are Implemented with real evidence and absent from the POA&M.
5. **Check the specials.** Confirm 3.5.3 and 3.13.11 were scored on degree of implementation, not as all-or-nothing.
6. **Check the POA&M.** Confirm no POA&M item exceeds its allowed weight for the status being claimed, milestones are dated and owned, and the 180-day clock (for Conditional status) is tracked.
7. **Confirm the arithmetic.** Recompute the score from the evidence index. Confirm it falls between -203 and 110.

## Gate decision

- **Pass**: all checks hold. The reviewer signs and dates the review record, and the score moves to management attestation.
- **Pass with findings**: minor issues documented with owners and due dates. The score moves forward only after findings close.
- **Fail**: any never-deferrable gap, any Implemented control without evidence, any arithmetic error, or a pattern of weak justifications. The assessment goes back for rework. A failed gate is cheaper than a False Claims Act case.

## The review record

Keep one page per review: date, reviewer name and qualification, scope sampled, findings, decision, signature. Store it with the score, the evidence index, and the management attestation. If the government ever asks how you know your score is real, this page is the answer.

## Why this exists

Every invoice under a DFARS cybersecurity contract certifies your controls are real. No breach is required for liability, and your own people can file the case and take 15 to 30 percent. An independent review is the difference between a score you believe and a score you can defend.

---

MAPS (Map, Assess, Prioritize, Sustain) by AI Tech Pros, Inc., Augusta, GA. https://aitechpros.ai
Framework updates: The Readiness Room, https://thereadinessroom.substack.com (free)
