# Ledger Status

**Project:** `L_BEHAVIOR1K`  
**Tier:** TIER_5_WORLD_NEURO_EMBODIED  
**Identity:** Upstream `StanfordVL/BEHAVIOR-1K` @ `bd049de3119a` (MIT)

## Chain state

| Fact | Value |
| --- | --- |
| Upstream | `StanfordVL/BEHAVIOR-1K` |
| Commit | `bd049de3119acdcdf2334fe9e1ebe060fa20c108` |
| Upstream licence | MIT |
| Licence class | permissive |
| Clone size | 547.57 MB |
| Ledger | 0 blocks, chain verified |
| Current TRL | NOT YET MEASURED |
| Post-optimisation TRL | NOT YET MEASURED |
| II budget cap | 1000.0 IIU |
| Verified upstream edits | 1 |

- Blocks: **0**
- Head digest: `None`
- Chain verification: **verified**

## Independent verification

The chain is verifiable without trusting this project's tooling:

```
anticloud ledger verify
anticloud ledger export > ledger.jsonl
```

Each block carries the previous block's digest, so removing or reordering an
entry invalidates every block after it. That property is the reason the
ledger can stand in for a claim of what happened.
