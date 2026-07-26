# Event Conclave — Google Form field spec

**Purpose:** Standardised post-fight / post-martial-event minutes (conclave), fillable on a phone immediately after the debrief. Supports constitution requirements for meeting minutes after martial events.

**Implementation:** Google Form → responses Sheet under `02 Operational Records/Event Conclave/`.

## Form settings

- Title: `Event Conclave Minutes — Pilgrim Souldiours`
- Description: “Complete before leaving the site when possible.”
- Mobile-friendly: keep fields short; prefer multiple choice over long prose where possible
- Collect email if Workspace login available

## Fields

| # | Field label | Type | Required | Options / notes |
|---|---|---|---|---|
| 1 | Event date | Date | Yes | |
| 2 | Venue | Short text | Yes | |
| 3 | Event name / type | Short text | Yes | e.g. Training, show fight, tourney |
| 4 | Recorder name | Short text | Yes | Person writing minutes |
| 5 | Marshal of the day | Short text | Yes | |
| 6 | Conclave start time | Time | Yes | |
| 7 | Number of combatants | Number | Yes | |
| 8 | Number of officials / marshals | Number | Yes | |
| 9 | Inspections completed | Multiple choice | Yes | Yes — all / Yes — with exceptions / No |
| 10 | Inspection exceptions | Paragraph | If exceptions | Link Marshal’s Log entries if known |
| 11 | Injuries or incidents | Multiple choice | Yes | None / Minor (first aid) / Report required |
| 12 | Incident summary | Paragraph | If not None | No unnecessary medical detail; Tier A follow-up offline |
| 13 | Safety observations | Paragraph | No | Kit, ground, weather, crowd |
| 14 | Fighting / drill notes | Paragraph | No | What was practised; issues to coach |
| 15 | Decisions / actions | Paragraph | Yes | Who owns each follow-up |
| 16 | Next training / event reminder | Short text | No | |
| 17 | Attendees (optional list) | Paragraph | No | Or “see sign-in sheet in Drive” |
| 18 | Confirmation | Checkboxes | Yes | “Minutes reflect the conclave discussion” |

## Practice

- Submit from the field; tidy wording later in the Sheet if needed
- If an incident report is required, open the separate incident template the same day; do not rely on this form alone
- Share view access with committee; restrict incident narrative exports
