# Digital platform map

Working name: **The Compaignye of the Pilgrim Souldiours**

This repository holds the **public website** and the **specifications** for association-owned digital systems. Prefer existing platforms (especially Google Workspace for Nonprofits) over custom software unless a clear need appears in [ROADMAP.md](ROADMAP.md).

## Suite overview

### 1. Essential infrastructure

| Asset | Platform | Notes |
|---|---|---|
| Public website | GitHub Pages (this repo) | Transfer to org `pilgrim-souldiours` ASAP; custom domain later |
| Role email | Google Workspace | `Prior@`, `Armorum@`, `Arca@` on the confirmed domain |
| Cloud storage | Google Drive | Public Assets / Operational Records / Research Library |
| Membership tracking | Protected Google Sheet | Schema in `docs/membership/SCHEMA.md` |

### 2. Operational record-keeping

| Asset | Platform | Spec |
|---|---|---|
| Marshal’s Log | Google Form → Sheet | `docs/ops/MARSHALS-LOG.md` |
| Event Conclave minutes | Google Form (mobile) → Sheet | `docs/ops/EVENT-CONCLAVE.md` |
| Insurance certificates, incident templates | Drive → Operational Records | `docs/google-workspace/DRIVE-STRUCTURE.md` |

### 3. Presence and engagement

| Asset | Platform | Notes |
|---|---|---|
| Private member hub | Discord (or Signal / private FB) | Setup notes in `docs/member-hub/README.md` |
| Public social | Chosen network | Museum aesthetic; education and recruitment only |

## Access tiers (summary)

Full detail: [docs/governance/ACCESS-TIERS.md](docs/governance/ACCESS-TIERS.md)

- **Prior + Armorum:** sensitive member health / insurance columns; incident files
- **Committee (incl. Arca):** membership status, ops folders, Workspace admin as assigned
- **All members:** Research Library (read); member hub; public site

## Governance checklist (Arca & Prior)

1. Create a **stand-alone** GitHub Organization — never under `riverbend-medieval` ([docs/governance/CREATE-GITHUB-ORG.md](docs/governance/CREATE-GITHUB-ORG.md)).
2. Org Owners = association custodians; website admin gets repo access, not sole ownership.
3. Prefer Google Workspace for Nonprofits once eligible (ACNC / registered non-profit).
4. Create role mailboxes; stop using personal Gmail for official correspondence.
5. Apply Drive folder structure and sharing rules.
6. Build Membership Sheet and Forms from the specs in this repo.
7. Minute digital-asset ownership ([docs/governance/DIGITAL-ASSET-OWNERSHIP.md](docs/governance/DIGITAL-ASSET-OWNERSHIP.md)).
8. Keep at least two GitHub org Owners and two Workspace admins ([docs/governance/SUCCESSION.md](docs/governance/SUCCESSION.md)).

## Explicit non-goals (v1)

- Custom CRM or member login on this website
- Storing PII, health data, or insurance PDFs in git
- Discord bots or automated social posting from this repo
