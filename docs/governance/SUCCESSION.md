# Succession and recovery

**Purpose:** Keep the website and digital platform runnable when officers change.

**Rule:** Passwords and 2FA codes do **not** live in this repository. This file lists *what* exists and *who* should hold access.

## Critical principle

At least **two people** must be able to:

1. Administer the GitHub Organization
2. Administer Google Workspace (when live)
3. Publish website updates (push or approve)
4. Recover domain DNS (when registered)

## Separation from other groups

This project is **stand-alone**. Do not place the Organization, repo, Pages, or domain under `riverbend-medieval` or any other society’s GitHub account.

**Website admin** (`MedievalSteve`) maintains the public site. That role is custodial technical admin — not ownership of the association. Org **Owners** should be association officers (or a club-controlled login), with at least two Owners.

## Asset register (fill in as systems go live)

| Asset | Location / identifier | Primary custodian | Backup custodian | Status |
|---|---|---|---|---|
| GitHub Organization | `Compaignye-of-the-Pilgrim-Souldiours` | Website admin (`MedievalSteve`) during set-up | Second org Owner (post-inauguration) | Live — set-up mode; second Owner deferred until roles defined |
| Website repo | `Compaignye-of-the-Pilgrim-Souldiours/Compaignye-of-the-Pilgrim-Souldiours.github.io` | Website admin (`MedievalSteve`) | Second collaborator | Transferred to org |
| GitHub Pages | `https://compaignye-of-the-pilgrim-souldiours.github.io/` | Website admin | Second Owner | Live |
| Custom domain | TBD | Franklin | Host | Not registered |
| Google Workspace | TBD domain | Franklin | Host | Not started |
| Role mailboxes | Host / Clerk / Yeoman / Franklin | Role holder | Host | Placeholders only |
| Membership Sheet | Drive link TBD | Host + Franklin (restricted cols) | Clerk (non-restricted) | |
| Marshal’s Log | Form/Sheet TBD | Yeoman | Host | |
| Event Conclave | Form/Sheet TBD | Yeoman | Host | |
| Member hub | Discord (or other) TBD | Designated moderator | Host | |
| Public social | TBD | Comms officer | Host | |

## Dual-owner reminder (GitHub)

Create the organization with **two Owners** who represent the association (Host + Franklin, or club-controlled login + Host). A single-owner org is a succession risk.

Invite the website admin (`MedievalSteve`) for repository admin / write access so site work continues without making that personal account the association’s sole Owner.

## On officer change (checklist)

1. Add new officer to GitHub org / Workspace / Drive shares
2. Transfer ownership roles where required
3. Remove departing officer’s elevated access
4. Confirm recovery email and 2FA backup location with Host + Franklin
5. Update this register (status column and custodians)
6. Note the handover in committee minutes (no secrets)
