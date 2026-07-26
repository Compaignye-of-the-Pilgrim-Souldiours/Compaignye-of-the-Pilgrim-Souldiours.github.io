# Create the GitHub Organization (required)

GitHub does **not** allow creating a consumer Organization via API. An officer must create it once in the browser, then we transfer this repository into it.

## Why

Association ownership and succession need an **Organization** with **two owners**, not a personal user account. This repo was bootstrapped under `MedievalSteve` only so the scaffold could be pushed immediately.

## Steps (about 5 minutes)

1. Sign in to GitHub as the intended first owner (preferably a club-controlled account, not a throwaway).
2. Open [Create a free organization](https://github.com/account/organizations/new?plan=free).
3. Organization account name: **`pilgrim-souldiours`** (working slug — rename later if the legal name changes).
4. Contact email: association-controlled address when available.
5. This organization belongs to a business: choose what fits (often “My personal account” for a small club is fine at creation; you can adjust later).
6. Complete creation.

### Add a second owner immediately

Organization → People → Invite member → change role to **Owner**.  
Recommended pairing: web admin + Prior or Arca.

### Transfer this repository

1. Repo **Settings → General → Danger Zone → Transfer ownership**
2. New owner: `pilgrim-souldiours`
3. Confirm the repository name remains `pilgrim-souldiours.github.io`
4. After transfer, Pages URL becomes `https://pilgrim-souldiours.github.io/`
5. Update local remote:

```bash
cd /Users/SkeightleyPersonal/Documents/GitHub/pilgrim-souldiours.github.io
git remote set-url origin https://github.com/pilgrim-souldiours/pilgrim-souldiours.github.io.git
git remote -v
```

6. Tick the dual-owner row in [SUCCESSION.md](SUCCESSION.md).

## After transfer

Ask the web admin (or re-run agent) to verify Pages is enabled on the org repo (`Settings → Pages → Deploy from branch main /`).
