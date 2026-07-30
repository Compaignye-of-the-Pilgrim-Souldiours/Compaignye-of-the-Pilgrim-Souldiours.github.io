# Membership sheet schema

Use one Google Sheet as the membership register. Protect restricted columns so only **Host** and **Franklin** can edit/view them (Sheet → Data → Protect sheets and ranges, or a separate hidden tab with restricted share). Yeoman needs combat-clearance dates but not Tier A medical detail.

## Tab: Members

| Column | Example | Notes |
|---|---|---|
| member_id | PS-0042 | Stable ID; do not reuse |
| legal_name | | Legal name for insurance |
| preferred_name | | |
| email | | Prefer personal contact email for reminders |
| phone | | Optional |
| status | active / lapsed / honorary / applicant | |
| joined_on | 2026-08-01 | ISO date |
| membership_year | 2026 | |
| fees_paid_on | 2026-08-01 | |
| insurance_renewal_on | 2027-07-01 | Reminder driver |
| marshal_cert_expiry | 2027-01-15 | Blank if not certified |
| roles | member, armorum | Comma-separated |
| emergency_contact_name | | |
| emergency_contact_phone | | |
| notes_public_to_committee | | Non-sensitive |
| health_notes_restricted | | **Tier A only** |
| insurance_policy_ref_restricted | | **Tier A only** |

## Tab: Reminders (optional)

Use formulas or a monthly Franklin/Host review to list rows where:

- `insurance_renewal_on` is within 60 days
- `marshal_cert_expiry` is within 60 days
- `status` is `active` but `fees_paid_on` is empty for the membership year

## Practices

- Do not publish this Sheet on the website
- Do not paste exports into Discord
- Version history in Google is the audit trail; avoid parallel Excel copies on laptops
- When in doubt, upgrade path is documented in [../../ROADMAP.md](../../ROADMAP.md)
