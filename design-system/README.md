# Landlord Desk

Calm, exact tools for a landlord who lets homes in two countries.

Landlord Desk is a property-management app for one landlord with tenants in the UK and India. It covers the whole tenancy: enquiry, checks, agreement, rent, repairs, certificates, notices and move-out. This system describes how it looks and speaks. The reference build is `app/index.html` in the repository.

## Content fundamentals

- **Write like a careful letting agent.** Plain, specific and polite. "Rent of £1,450 is 9 days late", never "Payment issue detected".
- **Name things as landlords do.** Tenancy deposit, Gas Safety certificate, Section 13 notice, rent agreement, society NOC, police verification. Keep the local term for each country and do not translate one into the other.
- **Money always carries its currency.** £ amounts use en-GB grouping (£2,350). ₹ amounts use Indian grouping (₹1,35,000). Never mix currencies in one figure. A combined total is converted at the landlord's own rate and labelled with it.
- **Dates are written out.** "4 Dec 2026", in day-month-year order for both countries.
- **Buttons say what happens.** "Record payment", "Mark moved in", "Close tenancy". Each action ends with a toast that confirms it: "Payment of £900 recorded for Daniel Okafor".
- **Rules are stated, then sourced.** Guidance notes give the rule in one sentence and name the law or document behind it, for example "Capped at 5 weeks' rent (Tenant Fees Act)". Tax and legal notes end with "general guidance, not advice".

## Visual foundations

- **Ground.** `surface` is a neutral with a slight green bias. Work sits on `raised` panels with a `line` border and `radius-lg` corners. There are no shadows except `shadow-1` on the drawer and the selected segmented button.
- **Brand.** `brand` (deep green) marks the primary action, the active nav item and progress. Use it for one primary button per view at most.
- **Accent.** `accent` is saffron, a nod to the India side of the portfolio. It appears as fills only: cost bars, the door in the logo. As text it becomes `accent-ink` on `accent-soft`.
- **State.** Status always shows as a pill: a soft background, a matching dot and text. `ok` is Paid, Valid and Resolved. `info` is Due and In progress. `warn` is Due soon, Part paid and On notice. `bad` is Overdue, Expired and Emergency. The words always name the state, so colour is never the only signal.
- **Country.** Every tenant and property row carries a small mono `UK` or `IN` tag (`tag` style, `radius-sm`, `line` border). A top-bar segmented control filters the whole app to All, UK £ or India ₹.
- **Type.** Sora (`display`) is used for headings and stat figures only. Inter (`sans`) is used for everything else. IBM Plex Mono (`mono`) with tabular numerals is used for money in tables, counts and references.
- **Layout.** A 232px sidebar groups the work areas: Tenancies, Money, Property, Other. On phones it becomes a scrolling strip. Content runs to a maximum of 1240px with a `space-6` gutter (`space-4` on phones). Tables scroll inside their panel and never scroll the page.
- **Boards.** Pipelines (Onboarding, Maintenance) are columns on `sunken` with `raised` cards, each card showing a progress bar or priority pill in the same place.

## Patterns

- **Checklists per country.** Onboarding and move-out are checklists, and each step has a hint line with the rule behind it. UK onboarding: Right to Rent, referencing, deposit protection within 30 days, Gas Safety, EPC, EICR. India onboarding: KYC, police verification, agreement registration and stamp duty, society NOC.
- **Ledger.** Rent charges are raised every month. Payments are matched to the oldest unpaid month first. Overdue rows show the number of days late in the pill.
- **Reminders.** Gentle, firm and final versions are written from the arrears, ready to copy or send through WhatsApp, and can be logged as sent.
- **Expiry tracking.** Over 60 days is Valid, 31 to 60 is Upcoming, 30 or under is Due soon, and past the date is Expired.

## Iconography

There is no icon set. The only mark is the logo: a `brand` rounded square holding a house in `brand-ink` with an `accent` door. Use words, pills and country tags instead of icons, and no emoji.
