# Tagsmith — Taylers University

This folder is maintained by Tagsmith. Office documents (xlsx / docx) are not stored here;
Tagsmith renders them from these files when someone downloads them.

| File | What it is | Who edits it |
|---|---|---|
| `brd.md` | Business requirements (one row per requirement, stable IDs) | **People** — edits here drive automatic regeneration |
| `sdr.json` | Solution Design Reference: variables + sheet layout | Tagsmith (generated) |
| `blueprint.json` | Data-layer Blueprint rows | Tagsmith (generated) |
| `tagging/launch-spec.json` | Tagging requirements derived from SDR + Blueprint | Tagsmith (generated) |
| `tagging/rules.json` | Adobe Tags rules generated for deployment | Tagsmith (generated) |
| `tsd.json` | Technical Specification content | Tagsmith (generated) |
| `manifest.json` | Content hashes and provenance | Tagsmith (generated) |

Edits to generated files are overwritten on the next update. Change `brd.md` instead —
Tagsmith regenerates the SDR, TSD and tagging rules from it. Deploying to Adobe Launch
always waits for approval in Tagsmith.
