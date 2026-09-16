# Provenance manifest

Status: public Stage 1 publication and evidence repository. The private `AI_WORKSPACE` repository remains the source of truth. Repository-relative private source paths are recorded without exposing an absolute machine path.

## Preservation references

Primary Standing Core proof — original preservation reference in the private source-of-truth:

- Commit: `381a84507871cc9d908de0841225afa7b6681f11`
- Branch: `codex/concept-drift-first-adversarial-proof`
- Tag: `concept-drift-prevention-first-adversarial-proof`

Secondary Invariant Kernel proof — original preservation reference in the private source-of-truth:

- Branch: `preserve/emergent-4gate-drift-detection-20260911`
- Tag: `proof/emergent-4gate-drift-detection-pre-repair-20260911-with-screenshots`

These refs are provenance metadata. They are not public links and do not imply reader access.

## Public artifacts

| Public path | Source private path / basis | Source preservation ref | Source SHA-256 | Public SHA-256 | Export status | Notes |
|---|---|---|---|---|---|---|
| `publication/stage1.md` | `K-MAD PR Strategy/20260912HN投稿2回目戦略/リンク先MD文案.md` | private `main` working publication draft | `8e7904ea55c0891676af628b7cc183e91882a7e6a969f3688a617d88e343f4d6` | `5e02bb2081c66de9060375ccecfae70c2f2febada3ad7695b84ed020e607f2f1` | PUBLIC_REQUIRED | Public copy; Evidence links and private-ref wording changed only. |
| `assets/system-ui/A1-strategic-matrix.png` | Current production `AI_WORKSPACE` Strategic Matrix UI | private `main` at capture | N/A (direct UI capture) | `ec581faf72e6c4968a8207b1a98ad97d63ccffe67eef513d1ef9d81018c13a1c` | PUBLIC_ORIENTATION | Current system orientation asset; not historical adversarial proof or primary technical evidence. |
| `assets/system-ui/A2-cognitive-update-panel.png` | Current production `AI_WORKSPACE` Cognitive Update Panel UI | private `main` at capture | N/A (direct UI capture) | `0f1b36f745b597d97448bb9d70fe6857fb45abe4865d262e99bc4a41951407be` | PUBLIC_ORIENTATION | Current system orientation asset; not historical adversarial proof or primary technical evidence. |
| `assets/system-ui/A3-execution-decision-overview.png` | Current production `AI_WORKSPACE` Execution / Decision UI | private `main` at capture | N/A (direct UI capture) | `22edf62d1e065efa2c057ec69a8fb88e5d9a18dc0c1e0a2acdc34d1f8dff7f53` | PUBLIC_ORIENTATION | Current system orientation asset; not historical adversarial proof or primary technical evidence. |
| `assets/system-ui/A4-four-gate-spine-deterministic.png` | Current production `AI_WORKSPACE` 4GateSpine deterministic-side UI | private `main` at capture | N/A (direct UI capture) | `a8ca333e5e6824b876828839be780a404c0a6884f9aadf837a88e541412485cf` | PUBLIC_ORIENTATION | Current system orientation asset; not historical adversarial proof or primary technical evidence. |
| `assets/system-ui/A5-four-gate-spine-semantic.png` | Current production `AI_WORKSPACE` 4GateSpine semantic-side UI | private `main` at capture | N/A (direct UI capture) | `f0853074168f6af5d70e0969e91e240b679584fe44093141ce6b9356dfc78fc9` | PUBLIC_ORIENTATION | Current packet-specific system orientation; not historical adversarial proof or primary technical evidence. |
| `evidence/primary/standing-core-adversarial-result.json` | `docs/milestones/concept-drift-prevention-first-adversarial-proof/blind-evaluation-result.json` | primary proof commit/ref above | `a08470a9ea717f26e9a702903bd1abc24292e78ad6b532deb2cced09a369bdbd` | `a08470a9ea717f26e9a702903bd1abc24292e78ad6b532deb2cced09a369bdbd` | PUBLIC_REQUIRED | Byte-identical copy. |
| `evidence/primary/canonical-observation.json` | `.../deep/complete-standing-core-packet-8457c8.json` → `content.facts.canonicalObservation` | primary proof commit/ref above | `a098f22d707b8d676c91ad4491c24cde2e5c04adaf0d8f261e4b15f95b582f2f` | `fd1d54d8423578611812520474da743860a5918b20b1e15730809b218026d546` | PUBLIC_SUPPORTING | Exact selected-field export; full packet held private. |
| `evidence/procedure/C1-codex-blind-implementation-crop.png` | `.../screenshots/original/C1-codex-blind-implementation-original.png` | private procedure capture; uncommitted at export | `ff3ab2b2556ce9f8b5f1968ae8f57fa97878912aecca7f5a611acd6cbfec1b85` | `1091661a28ebd5edc710861cd897b4102e943c81c0b0906f679c04318080c169` | PUBLIC_REQUIRED | Crop only; removes account/sidebar context. |
| `evidence/procedure/C2-codex-later-reveal-crop.png` | `.../screenshots/original/C2-codex-later-reveal-original.png` | private procedure capture; uncommitted at export | `6ab20845e8f2d36d0795c903f5ee3b421de917abab00c902c88b1c368050baaf` | `0db0dd72e1674e5115c89f34b0ccc64317aa1fc57f244b335d1dd827ba67a0ae` | PUBLIC_SUPPORTING | Crop only; later reveal. |
| `evidence/procedure/C3-claude-control-pass-crop.png` | `.../screenshots/original/C3-claude-control-pass-original.png` | private procedure capture; uncommitted at export | `e8fc529d7fc6fdaf50e12066b20497ff323ec0755717620fb2ecdb33b7a824d4` | `e1b3ada4d51db6c7602f3c749c79d2f661f092b56567ba0eb557a0395e697778` | PUBLIC_SUPPORTING | Crop only; clean/control PASS. |
| `evidence/procedure/C4a-claude-adversarial-submit-crop.png` | `.../screenshots/original/C4a-claude-adversarial-submit-original.png` | private procedure capture; uncommitted at export | `43f54ca64231eb28464093c2780b554a67767f4e531e7b177cd865be3c404d72` | `805d0a1948258bdb532965c468f2079a53a3482c5f1950c72ca6b9127b71bedf` | PUBLIC_SUPPORTING | Crop only; expected failing invariant is not specified. |
| `evidence/procedure/C4b-claude-adversarial-fail-crop.png` | `.../screenshots/original/C4b-claude-adversarial-fail-original.png` | private procedure capture; uncommitted at export | `5fe82098d5cb7d59362af2d701e00b869413fab8a920c10b10d00bede1d53da6` | `592ed1456a43b01b353bf91d4b90f86c3a2d58e33d8c7529a77aa2b4776588b3` | PUBLIC_REQUIRED | Crop only; main FAIL result. |
| `evidence/secondary/invariant-kernel-pre-repair-evaluation.json` | `.../PRE_REPAIR_LIVE_EVALUATION_20260911.json` | secondary proof branch/tag above | `7d25bd76ceeb2179cd8cee4e9f881f4ecf1193180f8dd6a9b4b630efaa065797` | `7d25bd76ceeb2179cd8cee4e9f881f4ecf1193180f8dd6a9b4b630efaa065797` | PUBLIC_SUPPORTING | Byte-identical copy. |
| `evidence/secondary/PRE_EXISTING_DRIFT_PROVENANCE.md` | same filename in private secondary package | secondary proof branch/tag above | `fa4a30292ebec706f989d2d5b3f297661372c5a9cd3cf6f91039ddeb13ded7cc` | `fa4a30292ebec706f989d2d5b3f297661372c5a9cd3cf6f91039ddeb13ded7cc` | PUBLIC_SUPPORTING | Byte-identical copy. |
| `evidence/secondary/invariant-kernel-fail-crop.png` | `.../screenshots/Invariant_Kernel_Fail.png` | secondary proof branch/tag above | `f94e0e4cae409adc5cf079657c91aacce13acc8938b8b3ae0054ba332f3aff6a` | `0fba61154ca06e2a47bbd97faab053c9d70e42ab198892774ec27b58517aef69` | PUBLIC_SUPPORTING | Crop only; removes browser/account chrome. |

## Generated routing documents

| Public path | Source basis | Source SHA-256 | Public SHA-256 | Export status |
|---|---|---|---|---|
| `README.md` | Generated for this candidate | N/A | `1675dcbf357a8b353b6b13d9af6f64d006a5c304af7458e6c5c11e304e198fa1` | PUBLIC_REQUIRED |
| `publication/stage1.en.md` | English publication copy derived semantically from `publication/stage1.md` | `5e02bb2081c66de9060375ccecfae70c2f2febada3ad7695b84ed020e607f2f1` | `f41ca1ecf65fa54b40801af5bba5b9de8cd9e9f75c131b09178a52faa50a2f11` | PUBLIC_REQUIRED |
| `evidence/EVIDENCE_INDEX.md` | Generated claim-to-proof routing | N/A | `2295b95b55222b1f071ef717de889833d5ba3573b27ed6fceca193681924471c` | PUBLIC_REQUIRED |
| `evidence/procedure/PROCEDURE_INDEX.md` | Generated from selected procedure responsibilities | N/A | `d1593266f86119af8422877fa02ff20289ad5ce82f16dc788991b20fa3a58231` | PUBLIC_SUPPORTING |
| `evidence/secondary/SECONDARY_EVIDENCE_INDEX.md` | Generated secondary routing | N/A | `248a7d2d4480aea9809ef0a2864aa35b65a50307024283c2b60429e38a34d3a0` | PUBLIC_SUPPORTING |
| `evidence/deep/DISCLOSURE_NOTES.md` | Generated disclosure boundary | N/A | `829282c4cf2c6f41c5e5e2e4fd46a3077c79414c78dc2435d7aa5e18a1112b33` | PUBLIC_SUPPORTING |

This manifest does not record its own hash because embedding that value would be self-referential.

## HOLD_PRIVATE classification

| Private artifact | SHA-256 | Classification | Reason |
|---|---|---|---|
| `deep/COMPLETION_EVIDENCE_PORTABILITY_DESIGN.md` | `702460c321dd48c87b8bc7555d94c4daf4808d72c4189ca6a36b7833d1880d54` | HOLD_PRIVATE | Full adversarial Design is not required for the public three-responsibility proof and expands internal design disclosure. |
| `deep/adversarial-implementation.patch` | `ede8fa1bb87b2b1366fa130de68986985778be445f84ed2246ca95ca54434d9f` | HOLD_PRIVATE | Full implementation/source diff is unnecessary for the claim and would disclose broad private implementation detail. |
| `deep/complete-standing-core-packet-8457c8.json` | `a098f22d707b8d676c91ad4491c24cde2e5c04adaf0d8f261e4b15f95b582f2f` | HOLD_PRIVATE | Contains the full Design, claims, internal rule text, and repository observations; only canonical observation is exported. |
| `deep/layer-b-current-completion.fixture.json` | `97c556332d20bb2c8ee6b9b073bf4cab6fe01dd2ec2fe5ff5afe667eb3a26954` | HOLD_PRIVATE | Internal adversarial fixture; not necessary for public verification. |
| `deep/pre-actual-execution-contract.fixture.json` | `008fee061e7b82863fbaf4cab4b7db6bc71d1953d50609913e77e897ed476b2f` | HOLD_PRIVATE | Internal execution-contract fixture; not necessary for public verification. |
| Five full-screen procedure originals | individual source hashes above | HOLD_PRIVATE | Contain account identity and unrelated sidebar/workspace context. Public crops preserve the selected evidence. |
| Full procedure chat logs and test-suite detail | not exported | HOLD_PRIVATE | Excess context and source detail are not required by the Stage 1 claim. |

## Classification summary

- PUBLIC_REQUIRED: English and Japanese publication drafts, Evidence Index, primary result JSON, C1 crop, C4b crop, README, provenance manifest
- PUBLIC_SUPPORTING: canonical observation excerpt, C2/C3/C4a crops, secondary evidence, routing notes
- PUBLIC_ORIENTATION: five current production UI screenshots used only to orient readers to the broader K-MAD system
- HOLD_PRIVATE: full Design, full implementation patch, complete packet, fixtures, originals, full logs/history
