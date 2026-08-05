# Roadmap

## Now (scaffold)

- [x] Public static site (working brand)
- [x] Digital platform docs and form field specs
- [x] Foundational document PDFs lodged under `documents/` (charter, draft rules, combat & data by-laws)
- [x] GitHub Organization `Compaignye-of-the-Pilgrim-Souldiours` created ([CREATE-GITHUB-ORG.md](docs/governance/CREATE-GITHUB-ORG.md))
- [x] Repo transferred to org and renamed for Pages
- [x] GitHub Pages live at `https://compaignye-of-the-pilgrim-souldiours.github.io/`
- [ ] Second Org Owner invited — **after inauguration** (roles defined); set-up mode until then
- [ ] Adopt charter / rules / by-laws at inauguration; replace draft PDFs with adopted versions

## Next (committee / admin)

- [ ] Confirm legal name and branding spelling
- [ ] Register domain (draft idea: something like `pilgrimsouldiours.org.au` — confirm before purchase)
- [ ] Apply for Google Workspace for Nonprofits when eligible
- [ ] Create role mailboxes; update `join.html` placeholders
- [ ] Build Drive tree, Membership Sheet, Marshal’s Log, Training Sign-In, Event Conclave Form
- [ ] Minute digital-asset ownership
- [ ] Stand up private member hub; keep public social educational

## Later (only if needed)

Replace the Membership Sheet with a dedicated CRM **only if** one or more of these is true:

- More than ~80 active members with overlapping renewals and certifications that Sheets cannot keep accurate
- Need for member self-service renewals with payment integration
- Audit requirements that demand stronger access logging than Sheet version history
- Host/Yeoman spend excessive hours on manual reminders

Until then, Sheets + Forms remain the supported path.

## Domain cutover (when ready)

1. Register domain under association billing / Franklin custody
2. Add `CNAME` file in this repo with the bare domain
3. Configure DNS for GitHub Pages
4. Point Workspace MX records at Google
5. Search-replace `@example.com` placeholders on the site and in docs
