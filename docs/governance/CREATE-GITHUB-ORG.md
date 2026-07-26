# Create the GitHub Organization (required)

GitHub does **not** allow creating a consumer Organization via API. Create it once in the browser, then transfer this repository into it.

## Hard rules

1. **Stand-alone association org.** The Organization belongs to The Compaignye of the Pilgrim Souldiours (working name), not to any other medieval group.
2. **Never use `riverbend-medieval`.** Do not create this org, transfer this repo, or add Riverbend accounts as owners. If the browser is signed in as `riverbend-medieval`, sign out first.
3. **Website admin ≠ association owner.** `MedievalSteve` is the **website administrator** (push / Pages / day-to-day site work). Org **Owners** should be association custodians (e.g. Prior + Arca, or a club-controlled GitHub user plus one officer) — not a personal “I own the club” arrangement.

## Current interim state (safe)

| Item | Value |
|---|---|
| Repo | https://github.com/MedievalSteve/pilgrim-souldiours |
| Owner today | `MedievalSteve` (bootstrap only) |
| Site | https://medievalsteve.github.io/pilgrim-souldiours/ |

Nothing in this project is under the Riverbend GitHub account.

## Before you click Create

Confirm the avatar/username in the GitHub header is **not** `riverbend-medieval`. Prefer:

- a **club-controlled** GitHub user created for this association, **or**
- an officer account that will remain an org Owner

Then open [Create a free organization](https://github.com/account/organizations/new?plan=free).

1. Organization name: **`pilgrim-souldiours`** (working slug)
2. Contact email: association-controlled when available
3. Complete creation

If you already started an org while logged into the wrong account: **delete/cancel that draft** and start again under the correct login.

### Roles after creation

| GitHub role | Who | Purpose |
|---|---|---|
| **Owner** (at least two) | Association custodians (Prior / Arca / club login) | Billing, ownership, recovery, member admin |
| **Admin** or write on the website repo | `MedievalSteve` (website admin) | Edit site, manage Pages, PRs |
| Members | Other trusted editors as needed | Content only |

Invite `MedievalSteve` as org member with permission to administer the website repo — **do not** make the website admin the sole Owner.

### Transfer and rename this repository

1. While signed in as `MedievalSteve`, open https://github.com/MedievalSteve/pilgrim-souldiours → **Settings → General → Danger Zone → Transfer ownership**
2. New owner: org `pilgrim-souldiours` (must already exist and accept transfers)
3. Keep the name `pilgrim-souldiours` for the transfer
4. After transfer (as an org Owner), **rename** the repo to `pilgrim-souldiours.github.io` so the site is at `https://pilgrim-souldiours.github.io/`
5. Confirm **Settings → Pages** deploys from branch `main` path `/`
6. Update local remote:

```bash
cd /Users/SkeightleyPersonal/Documents/GitHub/pilgrim-souldiours.github.io
git remote set-url origin https://github.com/pilgrim-souldiours/pilgrim-souldiours.github.io.git
git remote -v
```

7. Update [SUCCESSION.md](SUCCESSION.md) with the two Owners and the website admin.
