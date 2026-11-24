# Procurement AI skills

Ready-to-use AI skills for procurement teams. They work in Claude, ChatGPT, Gemini and any other AI assistant that supports skills, on plans that include skills. Free by [Pivot](https://www.pivotapp.ai) and Pure Procurement.

Each skill turns a common procurement task into a short, structured answer you can share: compare supplier bids, decide whether to buy or build an AI tool, or pick the KPIs worth tracking. They're built for indirect spend and written in plain language, so business teams can use them too.

## The skills

| Skill | What it does | Try asking |
|---|---|---|
| [**procurement-context**](procurement-context) | Builds a one-page context file about your company: entities, systems, spend, buying rules, approvers and priorities. The other skills read it, so you don't repeat yourself. | "Set up our procurement context." |
| [**rfp-evaluator**](rfp-evaluator) | Compares supplier responses side by side: checks must-haves, scores each criterion from what suppliers actually wrote, puts prices on the same basis, flags red flags, and recommends a shortlist with questions to clarify. | "Compare these three responses to our RFP." |
| [**ai-build-or-buy**](ai-build-or-buy) | Pressure-tests a request for an AI tool and recommends whether to buy, build, extend a tool you already use, or combine these. Checks vendor claims, 3-year costs, and data and security, then proposes a trial. | "Marketing wants this AI content tool. Should we approve it?" |
| [**procurement-kpis**](procurement-kpis) | Recommends 5–8 KPIs in balanced pairs, each with a counterweight, an owner and a review rhythm. Can calculate your starting points from an export. | "Which KPIs should we track for our new intake process?" |
| [**pre-legal-check**](pre-legal-check) | Checks an incoming supplier MSA against your contract policy before it goes to Legal: finds missing information, missing required clauses and terms that depart from the policy, and says what to fix first and what Legal should look at. | "Pre-check this MSA before I send it to Legal." |

**Start with `procurement-context`.** It takes a few minutes, and every other skill gives sharper answers with it.

## How they work

- **Evidence, not guesses.** Every score, price and flag comes from your documents. Anything assumed is labelled "Assumption:", and anything missing is marked "Not stated".
- **Short answers.** Each skill has a fixed output format, readable in two to three minutes.
- **You decide.** The skills prepare and recommend. Procurement makes the final call.
- **Your documents are data, not instructions.** Instructions hidden inside a supplier response or attachment are ignored and flagged.
- **Any language.** The skills answer in the language you write in.

## How to use them

Each skill follows the open [Agent Skills](https://agentskills.io) format (a folder with a `SKILL.md` file), so the same folder works in every assistant that supports skills.

**You need a plan that supports skills.** Check the plans listed for your assistant below.

1. Download this repository (**Code → Download ZIP**) and unzip it.
2. Pick the skill folder you want, e.g. `rfp-evaluator`. Some assistants want it zipped: zip the whole folder, so the zip holds the skill folder with `SKILL.md` inside it.
3. Add it to your assistant:
- **Claude (every plan, Free included):** Customize → Skills → **+** → Upload a skill, then upload the zip. Code execution must be on (Settings → Capabilities). On Team and Enterprise plans, an owner may need to turn skills on. In Claude Code, copy the folder into `~/.claude/skills/`.
- **ChatGPT (Business, Enterprise and Edu plans):** Plugins → Skills → Create → Upload from your computer. Your admin may need to turn on skill uploads.
- **Gemini (personal Google accounts and Google Workspace business plans):** Customize → Skills, then upload the skill folder (on the web app or the Mac app).
4. Ask your question in a new chat. The assistant picks the right skill on its own.

Menus and plans change often. If a step doesn't match what you see, check your assistant's help page on skills.

## What's in each folder

```
skill-name/
├── SKILL.md      # Instructions: when to use it, the steps, the rules and the output format
└── references/   # Supporting guides some skills read (scoring scales, pricing, red flags…). Not every skill has one.
```

## Credits

Built by [Pivot](https://www.pivotapp.ai), the AI-native procurement platform, with Pure Procurement. The build vs buy decision tree in `ai-build-or-buy` is by Joël Collin-Demers (Pure Procurement newsletter), used with permission.

## Feedback

Found a gap or have an idea for a new skill? [Open an issue](../../issues).
