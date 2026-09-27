# prim-cleanup

Living **plan** for Prim Foundation org cleanup and consolidation.

This repository is **not product code**. It holds the org-wide plan: what to keep, what to merge, what to archive, and the order of work. Grok fills in the issue bodies; Paseo Prims executes approved slices; PrimsDrive proves mount/path truth where storage is involved.

## Why this exists

Brand assets, ownership, and build lanes are scattered across `primfoundation` and upstream `eidos-agi` repos. Duplicated folio/fonts, parallel brand kits, and unclear handoffs slow every product. This repo is the single place that tracks the consolidation plan until the map is clean.

## Plan skeleton (issues)

| # | Theme | Outcome |
|---|--------|---------|
| 1 | Brand consolidation | Canonical brand pack under primfoundation; kill duplicate assets |
| 2 | Repo ownership audit | Every repo belongs here or is archived/moved; purpose documented |
| 3 | Build lane definition | Grok plans · Paseo Prims executes · PrimsDrive proves |
| 4 | SSO-first sequencing | `prims-sso` / login.prims.sh before `primsdrive-cloud` / drive.prims.sh |
| 5 | Scattered-asset map | Full inventory + per-item dedup plan |

Open issues are the working backlog. Update them in place; do not fork parallel plan docs elsewhere.

## Related repos

- [primfoundation/prims-sso](https://github.com/primfoundation/prims-sso) — human IdP (OIDC/OAuth); login.prims.sh
- [primfoundation/primsdrive-cloud](https://github.com/primfoundation/primsdrive-cloud) — drive.prims.sh edge → mini → Sandisk king
- Upstream brand source today: [eidos-agi/prim.brand](https://github.com/eidos-agi/prim.brand) (to be transferred/mirrored — see issue 1)

## Rules

- **No application code** in this repo. Markdown + issues only.
- One plan of record. Cross-link product repos; do not copy the plan into each product README.
- Sandisk on `daniels-mac-mini` remains king for Prim data. Cleanup never invents a parallel store.
