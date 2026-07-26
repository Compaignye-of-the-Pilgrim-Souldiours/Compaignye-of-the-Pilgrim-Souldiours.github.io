# Succession and recovery

**Purpose:** Keep the website and digital platform runnable when officers change.

**Rule:** Passwords and 2FA codes do **not** live in this repository. This file lists *what* exists and *who* should hold access.

## Critical principle

At least **two people** must be able to:

1. Administer the GitHub Organization
2. Administer Google Workspace (when live)
3. Publish website updates (push or approve)
4. Recover domain DNS (when registered)

## Asset register (fill in as systems go live)

| Asset | Location / identifier | Primary custodian | Backup custodian | Status |
|---|---|---|---|---|
| GitHub Organization | `pilgrim-souldiours` (working slug) | Prior or designated web admin | Second org owner | **Create ASAP** — see [CREATE-GITHUB-ORG.md](CREATE-GITHUB-ORG.md) |
| Website repo | Currently `MedievalSteve/pilgrim-souldiours` (transfer to org) | Web admin | Second collaborator | Bootstrapped; transfer pending |
| GitHub Pages | Interim: `https://medievalsteve.github.io/pilgrim-souldiours/` → org URL after transfer | Web admin | Second owner | Enable after each transfer |
| Custom domain | TBD | Arca | Prior | Not registered |
| Google Workspace | TBD domain | Arca | Prior | Not started |
| Role mailboxes | Prior / Armorum / Arca | Role holder | Prior | Placeholders only |
| Membership Sheet | Drive link TBD | Prior + Armorum (restricted cols) | Arca (non-restricted) | |
| Marshal’s Log | Form/Sheet TBD | Armorum | Prior | |
| Event Conclave | Form/Sheet TBD | Armorum | Prior | |
| Member hub | Discord (or other) TBD | Designated moderator | Prior | |
| Public social | TBD | Comms officer | Prior | |

## Dual-owner reminder (GitHub)

Create the organization with **two owners** as soon as a second trusted member has a GitHub account. A single-owner org is a succession risk (account lockout loses the website and history).

Recommended: Prior (or web admin) + Arca, or Prior + Secretary.

## On officer change (checklist)

1. Add new officer to GitHub org / Workspace / Drive shares
2. Transfer ownership roles where required
3. Remove departing officer’s elevated access
4. Confirm recovery email and 2FA backup location with Prior + Arca
5. Update this register (status column and custodians)
6. Note the handover in committee minutes (no secrets)
