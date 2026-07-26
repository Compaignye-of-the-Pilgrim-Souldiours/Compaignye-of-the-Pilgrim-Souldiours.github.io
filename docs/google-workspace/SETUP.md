# Google Workspace setup

Prefer **Google Workspace for Nonprofits** once the association is eligible (typically registered non-profit / ACNC pathways — confirm current Google for Nonprofits criteria for Australia).

Until the real domain exists, do not invent a production domain in DNS. Use this checklist when ready.

## 1. Eligibility and tenancy

1. Confirm legal entity name and eligibility for Nonprofit discount/gratis tier
2. Apply via Google for Nonprofits
3. Claim the **association** domain (after registration) — not a personal Gmail
4. Designate **two Super Admins** (recommend Prior + Arca)

## 2. Role mailboxes

Create users or Google Groups routed to officers:

| Address | Role | Purpose |
|---|---|---|
| `prior@YOUR-DOMAIN` | Prior | Governance, general official mail |
| `armorum@YOUR-DOMAIN` | Armorum | Arms, inspections, martial safety |
| `arca@YOUR-DOMAIN` | Arca | Treasurer, Workspace billing, Drive stewardship |

Optional later: `website@`, `enquiries@` as groups.

**Do not** rely on personal Gmail for council or insurer correspondence.

## 3. Org units and 2FA

- Place officers in an `Officers` org unit; members (if licensed) in `Members`
- Enforce 2FA for all Workspace users
- Store backup codes in the association’s offline recovery process (see SUCCESSION.md)

## 4. After mail is live

1. Update `join.html` and any docs still using `@example.com`
2. Set role signatures (association name, role title, ABN if applicable — no personal mobile required)
3. Forwarding: prefer Workspace login over auto-forward-only to personal mail (so history stays in the tenancy)

## 5. Related docs

- [DRIVE-STRUCTURE.md](DRIVE-STRUCTURE.md)
- [../membership/SCHEMA.md](../membership/SCHEMA.md)
- [../ops/MARSHALS-LOG.md](../ops/MARSHALS-LOG.md)
- [../ops/EVENT-CONCLAVE.md](../ops/EVENT-CONCLAVE.md)
