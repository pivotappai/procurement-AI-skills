# Worked examples

Six short examples showing how the rules in `traffic-light.md` apply. The buyer is Acme, a fictional company; the suppliers are fictional too. Acme's Contract rules (in `procurement-context.md`) say:

- Liability: supplier cap of at least 12 months' fees (preferred)
- Auto-renewal: none above €50k (must-have)
- DPA: required whenever the supplier processes personal data (must-have)
- AI and data use: no training on Acme data (must-have)
- Governing law: French law, Paris courts (preferred)

## 1. Everything matches → 🟢

**MSA:** Northwind Analytics MSA, €40k a year. Complete, DPA attached, every key term matches the policy.

**Light:** 🟢 Send to Legal. Rule: no gap and no departure.

```
**🟢 Send to Legal**
Complete, and every key term matches your contract rules.
**Note for Legal:** Checked parties, term, renewal, payment, liability, data protection, AI use and governing law against Acme's Contract rules. No issues found.
```

## 2. Liability below the preferred cap → 🟡

**MSA:** As in example 1, but the cap is 3 months' fees (clause 9.2).

**Light:** 🟡 Send to Legal, with flags. Rule: the liability rule is preferred, so the departure is Legal's call, not the supplier's homework.

```
**🟡 Send to Legal, with flags**
Complete; one term departs from a preferred position (liability).
**Brief for Legal:**
1. Liability: MSA clause 9.2 "fees paid in the three (3) months preceding the claim"; policy: at least 12 months' fees (preferred). Departs from policy.
```

## 3. Missing DPA and auto-renewal → 🔴, with the email

**MSA:** Harbor Data MSA, €84k a year, for a service handling employee data. Clause 12 refers to a DPA "available on request", not attached. Clause 11.2 renews automatically for 12 months. Clause 18 sets English law.

**Light:** 🔴 Don't send yet. Rule: a missing document and a broken must-have. The governing law departure is yellow, so it goes to Legal, not into the email.

```
**🔴 Don't send yet**
The DPA is missing, and the MSA renews automatically above €50k.

**Email to the supplier** (review before sending)
Subject: Harbor Data MSA: changes needed before our review

Hi [Name],

Thanks for sending the Master Services Agreement dated [date]. Before it goes to our legal team, we need a few changes and some missing information:

1. Data processing (clause 12): the agreement refers to a data processing agreement that wasn't attached. Could you send it?
2. Renewal (clause 11.2): the agreement renews automatically for 12 months. We can't accept automatic renewal for this agreement. Could you change it to renewal by written agreement?

Could you send an updated version? Once we have it, we'll move on to our legal review.

Thanks,
[Your name]

**For Legal, once the supplier has replied:**
1. Governing law: MSA clause 18 "English law"; policy: French law, Paris courts (preferred). Departs from policy.
```

## 4. Policy doesn't mark non-negotiable rules → 🟡

**MSA:** Kestrel Consulting MSA with automatic renewal (clause 7). The company's contract policy says "we avoid auto-renewal" but doesn't mark any rule as must-have.

**Light:** 🟡 Send to Legal, with flags. Rule: unmarked rules count as preferred, so only gaps can make it red.

```
**🟡 Send to Legal, with flags**
Complete; auto-renewal departs from your policy.
Your policy doesn't mark which rules are non-negotiable, so departures are flagged for Legal rather than sent back to the supplier.
```

## 5. No policy supplied → partial check

**MSA:** Brightline MSA. The user says to go ahead without a policy. The MSA names "Acme Group" instead of the buying entity.

**Light:** 🔴 Don't send yet, from the gaps only. Rule: without a policy, only missing items can be checked, and 🟢 isn't possible.

```
**Brightline MSA: partial check (no company policy)**
**🔴 Don't send yet**
The buying entity is wrong. Key terms weren't checked against a policy: attach your contract policy or procurement context for a full check.
```

## 6. Must-have broken and go-live is close → 🔴 with an urgent flag

**MSA:** Vantage MSA. Clause 8.4 lets the supplier "use Customer Data to train and improve its models". The user mentions go-live is next Monday.

**Light:** 🔴 Don't send yet, plus the urgent flag. Rule: a broken must-have makes it red; the AI data-use issue with go-live days away also warrants telling Legal straight away.

```
**🔴 Don't send yet**
The MSA lets the supplier train models on Acme data, which your policy doesn't allow.
**Urgent: tell Legal now.** Clause 8.4 allows model training on Acme data, and go-live is next Monday.
```
