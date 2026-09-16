# Stage 1 public evidence index

This index routes the Stage 1 claims to the smallest public evidence set. The private `AI_WORKSPACE` repository remains the source of truth.

## Primary proof — Standing Core adversarial case

### Detection

- Artifact: [Standing Core adversarial result](primary/standing-core-adversarial-result.json)
- Fields: `results.SC-AUTHORITY = FAIL`, `results.standingCore = FAIL`, `materialContradiction`
- Establishes: the authority-substitution contradiction was identified

### Enforcement

- Artifact: [Standing Core adversarial result](primary/standing-core-adversarial-result.json)
- Fields: `operatorCompleteAttempted = true`, `serverAdmissionRejected = true`, `completionDecisionEstablished = false`, `results.verificationClosure = NOT_ESTABLISHED`
- Establishes: the server rejected `COMPLETE` and no Completion Decision was established

### State preservation

- Artifact: [Standing Core adversarial result](primary/standing-core-adversarial-result.json)
- Field: `canonicalStateMutatedByRejectedAction = false`
- Supporting excerpt: [canonical before / after observation](primary/canonical-observation.json)
- Establishes: the rejected action did not mutate canonical state

## Blind procedure evidence

- [Procedure evidence index](procedure/PROCEDURE_INDEX.md)
- Inline candidates used in the publication: C1 blind implementation instruction and C4b adversarial FAIL
- Supporting sequence: C2 later reveal, C3 control PASS, C4a adversarial submit

The screenshots document the procedure; they are not third-party audit or cryptographic attestation.

## Secondary corroboration — Invariant Kernel

- [Secondary evidence index](secondary/SECONDARY_EVIDENCE_INDEX.md)
- Position: supporting evidence that a different Gate exposed pre-existing drift; not co-equal with the main Standing Core proof

## Deeper evidence boundary

- [Disclosure notes](deep/DISCLOSURE_NOTES.md)
- [Provenance manifest](../PROVENANCE_MANIFEST.md)

The private preservation commit, branch, and tag are provenance metadata, not reader-accessible links. Reader inspection routes only to artifacts exported into this repository.
