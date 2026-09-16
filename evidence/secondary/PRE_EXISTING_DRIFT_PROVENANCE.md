# Pre-existing Kernel binding-name drift — provenance evidence

This document reconstructs, from Git evidence, that the current Kernel `FAIL` observed against
`execution-contract-completion-admission-outcome-specific-4gate-clearance@2` is caused by a
binding-name mismatch that existed **before** today's Completion-admission implementation began,
and that today's implementation diff does not touch the affected code.

## 1. The mismatch

`Get-OutcomeSpecificFourGateEvaluation` in `matrix-server.ps1` evaluates the Outcome-specific
Invariant Kernel responsibility using a fixed `$owners` array that maps **four literal Kernel
binding-name strings** to concrete owner function names. The array's binding-name strings are the
exact Kernel binding names authored for the **predecessor** Outcome
(`outcome-specific-4gate-plan-decision-basis-binding@1`, Contract @4):

```
Exact current authority at Plan Decision admission
Exact fixed-basis identity at consequential downstream writer/admission boundaries
Authority-domain and governed-target isolation
Gate non-authority at consequential admission
```

The **current** Contract's (`execution-contract-completion-admission-outcome-specific-4gate-clearance@2`)
fixed §9 Kernel section uses four **different** binding names, authored for this Outcome's own subject
matter:

```
Exact current authority at Completion admission
Required Outcome-specific clearance at the consequential writer
Independent Standing Core prerequisite
Gate non-authority and governed-target isolation
```

None of these four current strings are substring-matches for the four hardcoded predecessor strings,
so the evaluator's `$bindingPresent` check is `False` for all four bindings against the current basis,
and the Kernel responsibility reports `FAIL` for every binding — independent of whether the referenced
owner functions themselves exist.

## 2. This predates today's implementation — Git evidence

The repository's `HEAD` commit at the start of today's Completion-admission implementation work is:

```
752cafd Create COMPLETION_ADMISSION_OUTCOME_SPECIFIC_4GATE_CLEARANCE_DESIGN.md
```

All of today's Completion-admission implementation exists only as uncommitted working-tree changes on
top of this commit. Reading the `$owners` array **as it exists in `HEAD`** (i.e., before any of today's
changes):

```
$ git show HEAD:matrix-server.ps1 | grep -n "Exact current authority at Plan Decision admission\|Set-CurrentCompletionDecision'"
2128:        @('planDecision','Set-CurrentCompletionDecision',@('Assert-CurrentImplementationBasisTarget'),'decisionCurrent'),
2129:        @('bCheck','Set-CurrentCompletionDecision',@('ExpectedBCheckRevision','PASS'),'bCheckCurrent')
2554:        @('Exact current authority at Plan Decision admission','Set-CurrentPlanDecision','Assert-CurrentExecutionTarget'),
2557:        @('Gate non-authority at consequential admission','Set-CurrentPlanDecision','Set-CurrentCompletionDecision')
```

The predecessor-specific binding-name strings are **already present verbatim in `HEAD`**, i.e. before
today's implementation touched anything. This confirms the evaluator was never generalized to read
binding names from whichever Outcome's basis happens to be current — it has always been hardcoded to
the specific Outcome it was written for.

## 3. Today's implementation diff does not touch this code

```
$ git diff HEAD -- matrix-server.ps1 | grep -n "Exact current authority at Plan Decision admission\|owners=@("
(no output)
```

Today's diff against `matrix-server.ps1` (the Completion-admission connection: `Get-CurrentOutcomeSpecificFourGate`,
`Get-OutcomeSpecificCompletionClearance`, the new guard in `Set-CurrentCompletionDecision`, and the
`completionAdmission` projection on `Get-MinimumFourGate`'s response) contains **zero** lines touching
`Get-OutcomeSpecificFourGateEvaluation`'s body or its `$owners` array. The function is byte-for-byte
unchanged by today's work.

## 4. Conclusion

The current Kernel `FAIL` is a pre-existing repository-reality characteristic of
`Get-OutcomeSpecificFourGateEvaluation`, introduced when it was authored for the predecessor Outcome
and never generalized, and it already applied to Contract @2's basis from the moment that Contract's
Operator Plan Decision was fixed — independent of, and unmodified by, today's Completion-admission
implementation. Today's implementation's only effect was to correctly connect this pre-existing,
already-non-clear evaluation result to the Completion writer as a required admission prerequisite,
which is exactly what the Reviewed Design specified.

Repair of the evaluator's binding-name generalization is out of scope for the current Outcome's fixed
Plan / Acceptance Criteria / Test Plan (see the accompanying scope assessment) and is not undertaken by
this preservation snapshot.
