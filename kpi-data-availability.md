# KPI Data Availability Assessment

Generated from samples on hand: TherapyNotes contacts, Bloomerang donor export.

## What We Can Track Now

### Bloomerang (Fundraising)
File: `bloomerang.csv` / `.xlsx`
- Donor retention rate
- Revenue trends (YTD, last year, lifetime)
- Engagement scoring
- Interaction counts

Blocked: Cost per dollar raised (no campaign spend data).

### TherapyNotes (Counseling)
File: `TN_Practice-Contacts-List_created-5-15-2026.csv`
- Billable activity by clinician (Date, Service Code, Units, Rate)
- Insurance vs patient payment split
- Note completion status (field exists, needs validation)

Blocked or too thin to trust:
- Scheduled vs completed appointments (all rows show Type=Appointment; no cancellations visible)
- Weekly capacity percentage (only one day of data)
- Client demographics beyond DOB
- Goal achievement, supervision, documentation lag
- Employee turnover

## What's Blocked on ExtendedReach

No export present. This is the critical path for:
- IFP: hours per home, therapist vs skillbuilder hours
- Foster Care: kids per home, licensing timelines, medical/dental on-time rates, discharge summaries, mileage/efficiency
- Supervision: days behind in documentation across all programs

## Next Actions

1. **ExtendedReach**: Confirm whether the Zoho Analytics Query Tables add-on is available. Without it, case management data is trapped.
2. **TherapyNotes**: Request a wider date range export to check if no-show/cancel data is captured.
3. **Bloomerang**: Await data rows; headers alone confirm schema but not data quality.
