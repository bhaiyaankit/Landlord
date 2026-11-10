# Landlord Desk

A working demo of a property-management app for a landlord with tenants in both the UK and India. It covers the full tenancy, from first enquiry to move-out.

Open `app/index.html` in any browser. No install or server is needed. It starts with sample data for 7 properties (London, Manchester, Bristol, Bengaluru, Pune, Mumbai) and 8 tenants. Changes are saved in the browser, and **Setup → Reset sample data** starts the demo again.

## What it covers

| Area | What the landlord can do |
| --- | --- |
| Overview | Rent due and collected this month, arrears, occupancy, urgent repairs, expiring certificates, upcoming move-ins and move-outs |
| Onboarding | Pipeline board (Enquiry → Application → Checks → Agreement and deposit → Ready to move in) with a checklist for each country. UK: Right to Rent, referencing, deposit protection, Gas Safety, EPC, EICR, How to Rent. India: KYC, police verification, rent agreement registration and stamp duty, society NOC |
| Rent and payments | Monthly rent raised automatically. Payments matched to the oldest unpaid month. Part payments, extra charges (late fee, utilities), days-late tracking, gentle/firm/final reminders (copy or WhatsApp), rent receipts (India HRA format) |
| Maintenance | Repair board with priority and target response times, contractor, cost and notes |
| Issues and notices | Dated log of complaints, neighbour or society disputes, arrears talks, notices and renewals |
| Compliance | Certificate and renewal expiry tracking for each property |
| Move-out | Notice, a check-out checklist for each country, deductions, the deposit return calculation, and closing the tenancy |
| Expenses and reports | Costs per property, 12-month income against costs, combined GBP/INR totals at your own exchange rate, CSV export, UK and India tax notes |
| Tenant portal | The tenant's view: balance, how to pay, receipts, reporting a repair, giving notice |

Legal and tax notes in the app are general guidance for England and India as of late 2026 and are not advice.

## Design system

`design-system/` holds the tokens and brand book the app follows (colours for light and dark, type, spacing, status pills, writing rules).

## Next steps for a real product

Logins for the landlord, tenants and contractors; a hosted database; Open Banking and UPI AutoPay for automatic payment matching; email, SMS and WhatsApp sending; e-signing and document storage.
