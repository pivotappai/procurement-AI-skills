# Email to the supplier (🔴 only)

When the light is red, write an email the user can copy, review and send to the supplier. The skill never sends it.

## What goes in

- **Only the red items:** missing information, missing documents, missing required clauses, and broken non-negotiable rules.
- **For each item:** where it is in the MSA (clause or section), what the MSA says or that it's missing, what the company needs, and a clear ask.
- **Leave out** yellow items. They're for Legal to decide and negotiate.

## What stays out

- **No legal wording.** Ask the supplier to amend the clause to meet the requirement; don't draft the clause.
- **No internal information:** approval thresholds, budgets, who approves, internal deadlines, or anything from the context file beyond the requirement itself.
- **No judgment of the supplier:** no "unacceptable", "non-compliant" or "risky". State the requirement neutrally.
- **No invented facts:** names, dates or deadlines the user didn't give stay as [placeholders].

## Template

Write it in the user's language, unless they ask for the supplier's language.

```
Subject: [Supplier] MSA: changes needed before our review

Hi [Name],

Thanks for sending the Master Services Agreement dated [date]. Before it goes to our legal team, we need a few changes and some missing information:

1. [Topic] (clause [x]): [what the MSA says, or "this is missing"]. [What we need, from the policy, in plain words]. Could you [update the clause / add it / send it]?
2. [...]

Could you send an updated version [by (date)]? Once we have it, we'll move on to our legal review.

Thanks,
[Your name]
```

## Writing each item

| Issue type | Example item |
|---|---|
| **Missing info** | "Parties (preamble): the agreement names Acme Group. Please issue it to Acme SAS, the entity buying and paying." |
| **Missing document** | "Data processing (clause 12): the agreement refers to a DPA that wasn't attached. Could you send it?" |
| **Terms at a link** | "Terms (clause 2.1): the agreement includes terms at a web address. Could you attach them, or confirm they don't apply?" |
| **Missing clause** | "Confidentiality: the agreement has no confidentiality clause. We need a mutual confidentiality clause. Could you add one?" |
| **Breaks a must-have** | "Renewal (clause 11.2): the agreement renews automatically for 12 months. We can't accept automatic renewal for this agreement. Could you change it to renewal by written agreement?" |
| **Breaks a must-have (data)** | "AI and data use (clause 8.4): the agreement lets you use our data to improve your models. We need our data excluded from model training. Could you update the clause?" |

Keep it short: one line of context, the numbered items, one closing line. Five items at most; if there are more, group the small ones.
