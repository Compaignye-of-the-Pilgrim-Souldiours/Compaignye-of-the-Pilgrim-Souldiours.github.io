# Training Sign-In — Google Form field spec

**Purpose:** Digital attendance register for training sessions. Records who attended, whether insurance was sighted, and whether safety inspection was completed. Primary operational record for the session gate.

**Implementation:** Google Form → responses Google Sheet stored under `02 Operational Records/Training Sign-In/`.

**Who submits:** Each participant, on their own phone (shared Form link or QR at the session).  
**Who can view the Sheet:** Chapter; Yeoman + Host own edits.

**Website front:** [training.html](../../training.html) — public sign-in CTA and officer-only archive index (no names or insurance flags in git).

## Temporary custody (until Workspace for Nonprofits)

Personal Google accounts are **not** the long-term system of record ([ACCESS-TIERS.md](../governance/ACCESS-TIERS.md)). Until association Workspace is available:

1. Create the Form and response Sheet on a **designated officer** account (prefer Host or Yeoman).
2. Share the Sheet immediately with the rest of the Chapter (view) and Yeoman + Host (edit).
3. When Workspace Shared Drive is ready, **transfer** Form, Sheet, and session exports into `02 Operational Records/Training Sign-In/` and revoke personal-only ownership the same week.

## Form settings

- Title: `Training Sign-In — Pilgrim Souldiours`
- Description: “Sign in once when you arrive. Confirm insurance and inspection with the Yeoman at the gate before submitting.”
- Mobile-friendly: keep fields short; prefer multiple choice over long prose
- Collect email addresses (Workspace users) if available; optional while on a personal account
- Limit to one response: **off** (many participants and sessions)
- Edit after submit: **off** (correct errors in the Sheet if needed)
- Confirmation message: short thank-you; remind non-martial attendees to choose N/A where appropriate

## Live links (temporary custody)

| Asset | URL |
|---|---|
| Public Form (site CTA + QR) | https://docs.google.com/forms/d/e/1FAIpQLSf6cxppGEHiE6rOKVCy5IaETdNV_4YOIDMeMbOMT3GZFqBehg/viewform |
| Responses Sheet (Chapter / Yeoman) | https://docs.google.com/spreadsheets/d/1K0x86Mi6JbaFJfz1T_2xkc3EJqX2I5vNd3rQ5lp9NGc/edit |

Keep the Sheet shared to **Chapter view / Yeoman + Host edit** — do not rely on “anyone with the link” for the live Sheet. The public site links only to the Form; past-session archive rows on `training.html` use separate restricted export links.

Printable QR (encodes the Form URL above): [`assets/images/training-signin-qr.png`](../../assets/images/training-signin-qr.png). Also shown on `training.html`.

## Fields

| # | Field label | Type | Required | Options / notes |
|---|---|---|---|---|
| 1 | Training date | Date | Yes | Session date |
| 2 | Venue / session name | Short text | Yes | e.g. Maryborough training — oval |
| 3 | Participant name | Short text | Yes | Preferred name as used in the company |
| 4 | Insurance sighted | Multiple choice | Yes | Yes / No / N/A (non-martial) |
| 5 | Safety inspection completed | Multiple choice | Yes | Yes / No / N/A (non-martial) |
| 6 | Notes | Paragraph | No | Optional; no health detail |

## Field practice

- Participant still submits their own row.
- Yeoman (or duty marshal) **confirms** insurance sighting and kit/safety inspection with the participant at the gate before or as they submit.
- Item-level weapon/armour inspections remain in the [Marshal’s Log](MARSHALS-LOG.md); this register only records that the session safety check was completed for that person.

## Sheet columns

Mirror the field labels in row 1. Add computed columns if useful:

- `year_month` for filtering
- `gap_flag` = Yes if Insurance sighted or Safety inspection completed is **No**

## Per-session archive

After each training session:

1. Filter the Sheet by training date (and venue if needed).
2. Export PDF or CSV named `YYYY-MM-DD-training-signin` (ISO date).
3. Store the export in `02 Operational Records/Training Sign-In/` (or a `session-exports/` subfolder).
4. Share the export (or a filtered Sheet view) with **Chapter / Yeoman only** — not “anyone with the link”.
5. Add one row to the **Past sessions** list on [training.html](../../training.html): date, venue, and the restricted “Open register (officers)” link. Do **not** commit participant names or insurance/inspection answers to git.

## Backup

Export full Sheet CSV to `02 Operational Records/Training Sign-In/exports/` at least quarterly (Franklin calendar), same rhythm as the Marshal’s Log.
