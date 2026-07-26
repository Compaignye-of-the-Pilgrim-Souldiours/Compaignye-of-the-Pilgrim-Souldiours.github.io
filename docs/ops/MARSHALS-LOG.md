# Marshal’s Log — Google Form field spec

**Purpose:** Digital ledger of weapon and armour inspections. Primary record if an insurer asks what was checked and when.

**Implementation:** Google Form → responses Google Sheet stored under `02 Operational Records/Marshals Log/`.

**Who submits:** Armorum or designated marshal.  
**Who can view the Sheet:** Committee; Prior + Armorum own edits.

## Form settings

- Collect email addresses (Workspace users) if available
- Limit to one response: **off** (many inspections over time)
- Edit after submit: **on** for the marshal account if needed
- Title: `Marshal’s Log — Pilgrim Souldiours`

## Fields

| # | Field label | Type | Required | Options / validation |
|---|---|---|---|---|
| 1 | Inspection date | Date | Yes | |
| 2 | Inspection time | Time | No | |
| 3 | Event / venue | Short text | Yes | e.g. Training — venue name |
| 4 | Marshal name | Short text | Yes | |
| 5 | Owner / bearer name | Short text | Yes | Member preferred name |
| 6 | Item category | Multiple choice | Yes | Weapon / Armour / Other kit |
| 7 | Item description | Short text | Yes | e.g. Spear, 9ft ash |
| 8 | Tip dimensions (mm) | Short text | If weapon | Free text; note gauge used |
| 9 | Shaft / structure integrity | Multiple choice | Yes | Pass / Pass with note / Fail — removed from use |
| 10 | Edges / points condition | Multiple choice | If weapon | Pass / Pass with note / Fail |
| 11 | Armour coverage / fastenings | Multiple choice | If armour | Pass / Pass with note / Fail / N/A |
| 12 | Defects or notes | Paragraph | No | |
| 13 | Action taken | Multiple choice | Yes | Cleared for use / Restricted use / Quarantined / Retired |
| 14 | Follow-up date | Date | No | If restricted |
| 15 | Photo link (optional) | Short text | No | Drive URL only — no uploads of sensitive content to public folders |

## Sheet columns

Mirror the field labels in row 1. Add computed columns if useful:

- `year_month` for filtering
- `fail_flag` = Yes if any Fail or Quarantined/Retired

## Backup

Export CSV to `02 Operational Records/Marshals Log/exports/` at least quarterly (Arca calendar).
