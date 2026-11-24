# Worked examples

Six short scenarios showing how the decision rules in `readiness.md` apply. The buyer is Acme, a fictional company; the suppliers are fictional too. Each shows the package, the key findings, the status, and the rule that sets it.

## 1. Complete package, no issues found → 🟢

**Package:** Northwind MSA (signed, 12 January 2026), amendment 1 (signed, 3 June 2026), SOW 4 (draft for signature), rate card (Schedule 2). Acme's contract policy supplied.

**Findings:** SOW 4 references the MSA as amended, same entities, dates within the MSA's term. Rates match Schedule 2. The MSA meets every documented position in the policy. SOW 4 includes the scope, acceptance criteria and milestones the MSA requires.

**Status:** 🟢 Ready for Legal. Rule: no 🔴 or 🟡 finding, every check done.

```
**Readiness: 🟢 Ready for Legal**
Package complete; no issues found in the material supplied.
**Legal handoff brief:** None identified.
```

## 2. Complete package, liability departure → 🟢, flagged first

**Package:** As in example 1, but the MSA caps the supplier's liability at fees paid in the previous 3 months (MSA, clause 9.2). Acme's policy requires at least 12 months' fees (Contract rules, Liability).

**Findings:** Everything is present and consistent. One departure from policy on liability.

**Status:** 🟢 Ready for Legal. Rule: legal-judgment findings don't change the status. The package is ready for Legal to assess the departure.

```
**Readiness: 🟢 Ready for Legal**
Package complete; one departure from policy for Legal to assess (liability).
**Legal handoff brief:**
1. Liability cap: MSA clause 9.2 "fees paid in the three (3) months preceding the claim"; policy "at least 12 months' fees". Departure from policy.
```

## 3. Unclear pricing decision → 🟡

**Package:** Brightline MSA (signed), order form OF-0042 (draft). The order form offers two options: 150 seats on an annual prepaid fee, or 150 seats billed monthly at a higher rate (section 2). The approved request was for 100 seats.

**Findings:** The order form belongs to the MSA, and the governing terms are clear. Two business questions: which pricing option, and why 150 seats rather than 100.

**Status:** 🟡 Clarification needed. Rule: a business detail needs a decision before Legal can assess the final document.

```
**Readiness: 🟡 Clarification needed**
Pricing option and seat count need a business decision.
**Blockers and clarifications**
- Choose a pricing option (order form, section 2) · Owner: business owner · Next action: confirm the option, then ask the supplier for a single-option order form
- 150 seats against 100 approved · Owner: business owner · Next action: confirm the quantity, or raise a new approval
```

## 4. Missing parent MSA → 🔴

**Package:** SOW 2 and order form OF-0117 from Kestrel Consulting. Both say they're governed by "the Master Services Agreement dated 3 March 2025". No MSA supplied.

**Findings:** The governing terms can't be established. The SOW and the order form can be checked against each other (same parties, consistent fees), but not against the MSA.

**Status:** 🔴 Blocked for routine review. Rule: parent MSA missing when SOWs or order forms are supplied.

```
**Readiness: 🔴 Blocked for routine review**
The MSA dated 3 March 2025, which governs both documents, wasn't supplied.
Not checked: MSA terms, precedence, policy conformity, SOW and order form against the MSA.
**Blockers and clarifications**
- Missing MSA (SOW 2, section 1; OF-0117, header) · Owner: procurement · Next action: find the signed MSA and any amendments in the contract repository, or ask the supplier
```

## 5. No company policy supplied → policy not checked, other checks run

**Package:** Harbor Data MSA (signed), order form OF-0210 (draft). No contract policy, playbook or context file.

**Findings:** The order form belongs to the MSA. It adds a 12-month auto-renewal with 90 days' notice (section 5), which the MSA doesn't have: an additional term for Legal. Everything else is consistent.

**Status:** 🟢 Ready for Legal, with the scope disclosed. Rule: no policy is not a blocker; the status comes from the other findings, and the auto-renewal is a legal-judgment finding.

```
**Readiness: 🟢 Ready for Legal**
Package complete; one additional term for Legal. Policy conformity not checked.
Not checked: policy conformity (no policy supplied).
**Legal handoff brief:**
1. Auto-renewal: MSA silent (clause 3, Term); order form section 5 "renews automatically for successive 12-month periods unless terminated on 90 days' notice". Additional term.
```

## 6. Red package with an urgent legal concern → escalate anyway

**Package:** Two versions of the Vantage MSA (v2 and v3), neither marked final or signed, and SOW 1 (draft). Go-live is next Monday, per the cover note. Acme's policy forbids suppliers training AI models on company data.

**Findings:** The governing version can't be established. SOW 1, section 7, lets the supplier "use Customer Data to train and improve its models". That departs from Acme's policy whichever MSA version governs.

**Status:** 🔴 Blocked for routine review, with the urgent escalation flag. Rule: governing version can't be established → 🔴. The AI data-use clause, with go-live in days, warrants escalation regardless.

```
**Readiness: 🔴 Blocked for routine review**
Two MSA versions (v2, v3) and no way to tell which governs.
**Urgent: escalate to Legal now.** SOW 1, section 7, lets the supplier train its models on Acme data, against Acme's AI policy. Go-live is next Monday.
**Blockers and clarifications**
- Governing MSA version unclear · Owner: procurement · Next action: confirm with the supplier which version was signed, and get the signed copy
```
