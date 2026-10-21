# HemoTrace — public assignment record

This repository holds only fingerprints of the explore/confirm assignment for the HemoTrace study, so that
anyone can later check the assignment was fixed before any outcome variable was opened (proposal Aim 1, 9.1).
No data, no code and no person identifiers are published here.

| Item | Value |
|---|---|
| Assignment rule | `u = int(sha256(f"{seed}|{dataset}|{person}").hexdigest()[:15], 16) / 16**15`; explore if `u < explore_frac` (per-dataset plan in the code repository, `config/split_plan.tsv`) |
| Seed | `hemotrace-split-2026-10-21` |
| Code-repository commit holding the tables | `b483d1a` (recorded 2026-10-21 13:42:15 -0400) |
| sha256 `splits/persons.tsv` | `3c1bf33dd622b0237faee47c9e6c055c1174fcd7b85865c311100238463f1f3d` |
| sha256 `splits/runs.tsv` | `c693414572ea97e78b0d038b5309e75cec89c62bbf3ae56bc72ec111251b143c` |
| Synthetic-pair split seed (Aim 3) | `hemotrace-synth-2026-10-21` |

Datasets assigned: GSE107011, GSE118165, GSE70068, SRP429744, GSE97590, GSE45735, GSE239282, GSE223613, GSE206505.
GSE154918 (admission samples only) will be added with its own hashes when assigned.

The GitHub commit time of this file is the public timestamp. Later additions are appended below, never edited.

## Log
- 2026-10-21: initial assignment hashes (above).
