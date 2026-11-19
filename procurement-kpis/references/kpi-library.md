# KPI library (indirect spend)

The KPIs this skill can recommend.

How to read each entry:
- **Use:** Core (recommend by default), Situational (only when the situation calls for it), Monitor (track, no target, not for leadership)
- **Moves:** how soon the number usually responds to a change
- **Data needed:** the fields required to calculate it (used to tell the user what's missing)

---

## Control

### PO before invoice
- **Use:** Core · Outcome, lagging · **Moves:** 1–2 quarters
- **Formula:** invoice spend with a PO dated before the invoice ÷ invoice spend that should have a PO
- **How to measure it:** take invoices for the period, exclude cards, payroll, taxes and other spend that never needs a PO, then check if the PO date is before the invoice date
- **Counterweight:** POs raised after the invoice
- **Data needed:** invoice date, invoice amount, linked PO number, PO date, spend type (to exclude)
- **Watch:** don't aim for 100%. Small buys are often better on a card. Report entities on a different ERP separately.

### POs raised after the invoice
- **Use:** Core (as counterweight) · Driver · **Moves:** 1 quarter
- **Formula:** POs created after their invoice or goods receipt ÷ all POs
- **How to measure it:** compare each PO's creation date with the date of its first invoice
- **Counterweight to:** PO before invoice
- **Data needed:** PO date, first invoice date per PO

### Spend through procurement (spend under management)
- **Use:** Core · Outcome, lagging · **Moves:** 2–4 quarters (check yearly for leadership)
- **Formula:** spend procurement actively managed (sourced, contracted or bought through a procurement request or catalog) ÷ addressable indirect spend
- **How to measure it:** agree with Finance what counts as addressable, then add up spend that went through a request, contract or catalog
- **Counterweight:** on-contract spend, requester satisfaction
- **Data needed:** total indirect spend by supplier, list of spend that went through requests, contracts or catalogs
- **Watch:** easy to overclaim. Only count spend procurement actually influenced.

### On-contract spend
- **Use:** Core · Driver · **Moves:** 2–4 quarters
- **Formula:** spend with contracted suppliers at contract terms ÷ addressable spend
- **How to measure it:** match supplier spend against your contract list; count only suppliers with an active contract
- **Counterweight to:** spend through procurement (stops counting spend that only passed through a form)
- **Data needed:** spend by supplier, contract list with supplier and dates
- **Watch:** needs a contract list. If there isn't one, start there (see contract repository coverage).

### Off-contract spend
- **Use:** Situational, when the goal is framed as "stop buying outside the process" · **Moves:** 2–4 quarters
- **Formula:** spend outside approved suppliers, channels or policy ÷ addressable spend
- **How to measure it:** the mirror of on-contract spend; most useful split by entity or department
- **Note:** recommend this or on-contract spend, not both

---

## Speed and experience

### Request-to-PO time
- **Use:** Core · Driver, leading · **Moves:** weeks
- **Formula:** median days from request submitted to PO sent (starting at submission, not approval, includes approval time, which is usually what requesters complain about)
- **How to measure it:** take the request date and the PO date for each completed request and use the median, not the average
- **Counterweight:** competitive coverage, or requester satisfaction
- **Data needed:** request date, PO date

### Requester satisfaction
- **Use:** Core (often as counterweight) · Outcome · **Moves:** 1–2 quarters
- **Formula:** average score (1–5) or NPS from people who buy through procurement
- **How to measure it:** a short quarterly survey (one score plus one open question), and optionally after big purchases
- **Counterweight to:** adoption, PO before invoice, savings, spend through procurement
- **Data needed:** survey responses
- **Note:** for indirect spend this is also the best quality signal: do the people using what was bought think it does the job?

### Intake or guided buying adoption
- **Use:** Core during a rollout · Driver, leading · **Moves:** weeks
- **Formula:** requests (or spend) through the intake form, catalog or guided buying ÷ all requests (or eligible spend)
- **How to measure it:** count requests by channel (form, email, chat, card) each week
- **Counterweight:** requester satisfaction
- **Data needed:** request channel
- **Watch:** adoption is a means, not an outcome. Use it during a rollout, then move it to monitor.

### Early involvement
- **Use:** Situational: intake rollouts, "procurement hears about it too late" · **Moves:** 2–3 quarters
- **Formula:** new purchases above a threshold where procurement was involved before the supplier was chosen ÷ all new purchases above the threshold
- **How to measure it:** add one question to the request form ("Have you already chosen a supplier?") and count the answers
- **Counterweight:** request-to-PO time
- **Data needed:** request date, supplier-selected flag or quote dates

---

## Value

### Competitive coverage
- **Use:** Core (as counterweight to speed; driver for savings) · **Moves:** 1–2 quarters
- **Formula:** awarded spend above your threshold that had 2+ (or 3+) real bids ÷ awarded spend above the threshold
- **How to measure it:** use your policy's threshold; count quotes per purchase
- **Counterweight to:** request-to-PO time, savings
- **Data needed:** purchase amount, number of quotes or bids
- **Watch:** if the policy is unclear on the threshold, pick one and say so

### Finance-validated savings
- **Use:** Core when savings are the goal · Outcome, lagging · **Moves:** 2–4 quarters
- **Formula:** savings that Finance accepts, against a baseline agreed with Finance (previous price or budget), that lower actual spend
- **How to measure it:** agree the baseline rules with Finance first, then log each saving with its baseline, new price and volume, and get Finance sign-off
- **Counterweight:** savings realisation
- **Data needed:** baseline price, new price, volume, Finance sign-off

### Savings realisation
- **Use:** Core when savings are the goal · Driver · **Moves:** 6–12 months after signing
- **Formula:** savings seen in actual spend ÷ savings in signed deals, same period
- **How to measure it:** compare what was actually spent on the deal with the volumes and prices it was signed at
- **Counterweight to:** finance-validated savings
- **Data needed:** signed savings per deal, actual spend per deal

### Total cost evaluation
- **Use:** Situational: savings goals, big IT or services buys · **Moves:** 1–2 quarters
- **Formula:** big purchases (above a threshold, e.g. €100k) decided on total cost and service, not unit price alone ÷ all big purchases
- **How to measure it:** check whether each big award had a scoring sheet covering total cost (setup, licences, support, exit) and service
- **Counterweight to:** competitive coverage, savings ("cheapest price wins")
- **Data needed:** list of big awards, evaluation method used

### Cost avoidance
- **Use:** Monitor; Situational for big renewals with price increases
- **Formula:** value of price increases prevented, against a written supplier request or index
- **Note:** report it, never set a target on it. It is the easiest number to inflate.

---

## Efficiency and automation

### Strategic time share
- **Use:** Situational: "grow without hiring", automation or AI projects · **Moves:** 1–2 quarters
- **Formula:** share of team time on strategic work (sourcing, negotiation, supplier and stakeholder work) vs admin (chasing approvals, creating POs, answering "how do I buy")
- **How to measure it:** a two-week time log once a quarter, or a monthly estimate per person
- **Counterweight:** requester satisfaction
- **Data needed:** hours by activity

### Automation and AI share
- **Use:** Situational: AI or automation projects · **Moves:** weeks to 1 quarter
- **Formula:** tasks or transactions completed end to end by automation or AI ÷ total, always reported with the error and exception rate
- **How to measure it:** count tasks the automation finished without a person stepping in, and sample them for errors
- **Counterweight:** error and exception rate, first-pass match
- **Data needed:** task log with who completed it, exceptions

### Sourcing cycle time
- **Use:** Situational: teams that run RFPs or tenders · **Moves:** 1–2 quarters
- **Formula:** median days from request to contract award, by type of event
- **Counterweight:** competitive coverage
- **Data needed:** request date, award date, event type

### Touchless invoices
- **Use:** Situational: when accounts payable is part of the change · **Moves:** 1–2 quarters
- **Formula:** invoices processed with no manual step ÷ all invoices
- **Counterweight:** first-pass match
- **Data needed:** invoice processing history
- **Note:** usually owned by AP, not procurement

---

## Monitors (no target, not for leadership)

| KPI | Formula | Why monitor it |
|---|---|---|
| First-pass match | Invoices matching PO (and receipt) at first try ÷ all PO invoices | Catches bad POs and automation that pushes errors to AP. Also the usual cause of late payment. |
| Cost per PO | Purchase-to-pay running cost ÷ number of POs | Context only. Easy to misuse as a benchmark. |
| Spend classification | Spend classified to your categories ÷ total spend | Every spend KPI depends on it |
| Supplier master data | Duplicate suppliers and incomplete records | Wrong supplier data breaks spend and contract KPIs |
| Contract repository coverage | Active spend linked to a stored contract ÷ active spend | Without it, on-contract spend and savings realisation can't be measured |

---

## KPIs users often bring

Keep the user's own KPI if it measures an outcome. Pair it with a counterweight.

| User's KPI | What to do |
|---|---|
| Invoices paid on time | Keep. Formula: invoices paid by the due date ÷ invoices paid. Counterweight: first-pass match (stops checks being skipped to pay faster). Owner: usually AP. Data: due date, paid date. |
| Number of POs, requests or RFPs handled | Activity, not an outcome. Suggest request-to-PO time or competitive coverage instead, and say why. |
| Tool logins or users | A means, not an outcome. Suggest adoption (during rollout only) or requester satisfaction. |
| Number of suppliers (reduction) | Can create single points of failure. Suggest on-contract spend instead. |

---

## Not in this skill

Risk and resilience, sustainability and social impact, supplier delivery and quality (on-time-in-full, defects), procurement ROI, working capital and payment terms, price vs market index, supplier experience and innovation, team capability. If asked, say in one line that they're out of scope for this skill.
