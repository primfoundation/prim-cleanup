# prims-cleanup

Living **plan** for Prim Foundation org cleanup and consolidation.

This repository is **not product code**. It holds the org-wide plan: what to keep, what to merge, what to archive, and the order of work. Grok fills in the issue bodies; Paseo Prims executes approved slices; PrimsDrive proves mount/path truth where storage is involved.

## Scope: physical and conceptual

Cleanup here covers **both**:

- **Physical** — repos, brand assets, duplicated code/config, ownership, build lanes, SSO→drive sequencing.
- **Conceptual** — a single definition of Prim (product / entity / protocol / pack), Prim Foundation mission, and a coherent map of Prim-named surfaces (PrimsDrive, Prims SSO, Paseo, and the rest).

Neither half alone is enough. Conflicting READMEs and a clean asset tree still leave the org incoherent; a pretty mission statement with five folio copies still wastes work.

## Why this exists

Brand assets, ownership, definitions, and build lanes are scattered across `primfoundation` and upstream `eidos-agi` repos. Duplicated folio/fonts, parallel brand kits, unclear Prim wording, and fuzzy handoffs slow every product. This repo is the single place that tracks the consolidation plan until the map is clean.

## Plan skeleton (issues)

| # | Theme | Layer | Outcome |
|---|--------|--------|---------|
| 1 | Brand consolidation | Physical | Canonical brand pack under primfoundation; kill duplicate assets |
| 2 | Repo ownership audit | Physical | Every repo belongs here or is archived/moved; purpose documented |
| 3 | Build lane definition | Both | Grok plans · Paseo Prims executes · PrimsDrive proves |
| 4 | SSO-first sequencing | Physical | `prims-sso` / login.prims.sh before `primsdrive-cloud` / drive.prims.sh |
| 5 | Scattered-asset map | Physical | Full inventory + per-item dedup plan |
| 6 | Prim definition consolidation | Conceptual | Canonical Prim definition, mission, surface map; align all READMEs |

Open issues are the working backlog. Update them in place; do not fork parallel plan docs elsewhere.

## Related repos

- [primfoundation/prims-sso](https://github.com/primfoundation/prims-sso) — human IdP (OIDC/OAuth); login.prims.sh — [account model #1](https://github.com/primfoundation/prims-sso/issues/1) depends on a clear Prim definition (#6)
- [primfoundation/primsdrive-cloud](https://github.com/primfoundation/primsdrive-cloud) — drive.prims.sh edge → mini → Sandisk king — [README](https://github.com/primfoundation/primsdrive-cloud/blob/main/README.md) architecture assumes the same Prim definition (#6)
- Upstream brand source today: [eidos-agi/prim.brand](https://github.com/eidos-agi/prim.brand) (to be transferred/mirrored — see issue 1)

## Rules

- **No application code** in this repo. Markdown + issues only.
- One plan of record. Cross-link product repos; do not copy the plan into each product README.
- Sandisk on `daniels-mac-mini` remains king for Prim data. Cleanup never invents a parallel store.