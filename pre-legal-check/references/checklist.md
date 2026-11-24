# Checklist

Four parts: the package and its versions, how the documents relate, the MSA against the company's policy, and related documents against each other.

## Part 1: Inventory, completeness and versions

Record each document in the **Review scope** table.

| Check | What to record | Watch for |
|---|---|---|
| **Type** | MSA, amendment, SOW, order form, schedule, DPA, rate card, other | A document titled "Agreement" that's really an order form, or the reverse |
| **Date and version** | Date on the document, version number, "final" or "draft" marks | No date; several versions with the same title |
| **Signed or draft** | Signature blocks completed, or an e-signature certificate | Blank signature blocks; one party signed only. If unclear, write "Unclear" |
| **Parties** | Full legal names of both parties | A brand name instead of a legal name; a different entity from the other documents |
| **Referenced documents** | Every document, schedule or link mentioned | "As set out in Schedule 3" with no Schedule 3; terms at a URL; "DPA available on request" |
| **Amendment history** | Each amendment, its number and date, and what it changes | Amendment 2 supplied but not amendment 1; an amendment that refers to an MSA version not supplied |

**Missing documents.** For each missing document, say who refers to it (document and clause) and what can't be checked without it.

**Never assume** a document is signed, current or approved. Don't take a cover email's word for it either: the document itself is the evidence.

## Part 2: Relationships and governing terms

### Does each SOW or order form belong to this MSA?

| Check | Look in | Watch for |
|---|---|---|
| **MSA referenced** | Opening, definitions, "this SOW is governed by…" | No MSA named; a different MSA; an older version; "the supplier's standard terms" |
| **Same parties and entities** | Party blocks, signature blocks | A different supplier entity, or a different company entity from the MSA |
| **Dates** | Start and end dates; the MSA's term and survival clauses | Work starting before the MSA, or running past its end. Before flagging, check whether the MSA lets existing SOWs continue after it ends |

### Separate engagements

Several SOWs under one MSA are usually separate engagements. Differences between them (rates, teams, deliverables, dates) are not conflicts. Only compare documents that cover the same engagement, such as a SOW and its change order, or an order form and its renewal.

### Governing terms

1. Find the precedence clause, usually in the MSA, sometimes in the SOW or order form.
2. Note which document says it prevails: in general, or only for named clauses.
3. Check each amendment: which clauses it replaces, and whether later documents refer to the amended version.
4. If two documents both say they prevail, or the precedence clause is missing, write "Unclear" and flag it for Legal. Don't decide which is enforceable.

## Part 3: The MSA against the company's policy

Only run this part if the user supplied a contract policy, legal playbook or `procurement-context.md` with Contract rules. Otherwise, write in the scope: "Not checked: policy conformity (no policy supplied)."

For each provision, compare the MSA with the policy:

- The policy requires it and the MSA doesn't have it: **missing required provision**
- The MSA says something different from a documented position: **departure from policy**
- The policy has no position: don't flag it as a departure. List it for Legal only if it's unusual or high-risk, labelled "Not covered by the policy"

Only treat something as required if the policy says so. Don't add requirements, and don't use "market standard" as a substitute.

| Provision | What the policy usually sets |
|---|---|
| **Contract length and renewal** | Maximum term; whether auto-renewal is allowed; longest notice |
| **Payment and price increases** | Standard payment terms; cap on increases |
| **Liability** | Minimum cap on the supplier's liability; what's excluded from the cap |
| **Indemnities** | Which claims the supplier must cover |
| **Termination** | Right to exit; notice; fees on exit |
| **Intellectual property** | Who owns deliverables and company data |
| **Confidentiality** | Mutual; how long it lasts |
| **Data protection and location** | When a DPA is required; where data may be stored |
| **Security** | Required certifications |
| **AI and data use** | Whether the supplier may use company data to train models |
| **Governing law** | Accepted law and courts |
| **Sector rules** | Clauses the sector requires, e.g. DORA for critical ICT suppliers in EU financial services |

## Part 4: Related documents against each other

Compare each SOW or order form with its MSA, as amended. Classify each difference:

- **Contradiction:** says something different from the MSA (e.g. Net 15 against Net 45)
- **Express override:** says it replaces an MSA term ("notwithstanding the MSA…")
- **Additional term:** something the MSA doesn't cover (e.g. a new fee or an auto-renewal)

| Topic | Watch for in the SOW or order form |
|---|---|
| **Payment** | Shorter payment terms; payment in advance; invoicing before acceptance |
| **Fees and rates** | Rates above the rate card; new fees (set-up, travel, rush); a different currency |
| **Price increases** | A higher cap than the MSA's, or increases the MSA doesn't allow |
| **Renewal** | Auto-renewal the MSA doesn't have; longer notice |
| **Termination** | No termination for convenience; termination fees |
| **Liability** | A lower cap for this engagement; new exclusions |
| **Indemnities** | Indemnities removed or narrowed |
| **Intellectual property** | Supplier keeps ownership of deliverables |
| **Confidentiality** | Shorter or one-way |
| **Data protection** | New personal data processing not covered by the DPA; new sub-processors or locations |
| **Acceptance and change control** | Deemed acceptance after a few days; changes the supplier can make alone |
| **Subcontracting and staff** | Subcontractors without consent |
| **Governing law** | A different law or court |

### Project details are not conflicts

Scope, deliverables, milestones, named staff, locations, quantities and dates are what a SOW is for. Don't flag them as differences from the MSA unless they change a governing term (for example, a "milestone" that triggers payment in advance when the MSA says payment in arrears).

A SOW doesn't need to repeat the MSA. If it's silent on a topic, the MSA applies.

### Required SOW content

If the MSA or the policy lists what every SOW must include (scope, acceptance criteria, rates, milestones, term, signatures), check each item and flag what's missing. Only check what's actually listed.

### Contract issues or business questions?

| It's a contract issue when… | It's a business question when… |
|---|---|
| A document changes a governing term (liability, IP, payment terms, data) | The commercial content needs a decision or explanation (which pricing option, why the quantity differs from the request, which entity pays) |
| Goes to: **Legal handoff brief** | Goes to: **Blockers and clarifications**, owner: business owner or procurement |

## How to write a finding

One row per finding, with both sources and the passages side by side: "Payment: MSA clause 6.1 'payable within 45 days'; Order form section 3 'payable within 15 days'. Contradiction. MSA clause 2.3 says the MSA prevails."
