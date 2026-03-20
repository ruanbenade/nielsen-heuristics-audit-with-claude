# Nielsen Heuristics UI Audit — Claude Skill

A free Claude skill for evaluating digital user interfaces against Jakob Nielsen's 10 Usability Heuristics. Upload a screenshot and receive a structured, prioritised usability audit report.

---

## What it does

The skill runs a structured evaluation across all 10 heuristics, producing a consistent audit report that includes:

- A severity rating for each heuristic (0 = no issue → 4 = critical)
- Specific observations tied to visible UI elements
- Concrete, actionable recommendations
- A prioritised summary of the top issues to fix

Reports follow a fixed structure, making audits comparable across different screens, designs, and iterations.

---

## What it does not do

This skill evaluates **static screenshots only**. Three heuristics cannot be fully assessed from a single image and are flagged accordingly rather than guessed at:

- **H7 — Flexibility and efficiency of use** (requires observing user flows and interaction patterns)
- **H9 — Help users recognise, diagnose, and recover from errors** (only assessable if an error state is visible)
- **H10 — Help and documentation** (only assessable if help features are visible on screen)

For these, the report notes "Not assessable from static image" and recommends review through user testing or separate error state audits.

---

## How to install

1. Download `nielsen-heuristics-audit.zip`
2. Open [Claude.ai](https://claude.ai) and go to **Settings → Capabilities**
3. Ensure **Code execution and file creation** is enabled
4. Go to **Customize → Skills**
5. Click **"+"** → **"Upload a skill"** and upload the ZIP file

> Requires a free, Pro, Max, Team, or Enterprise Claude account.

---

## How to use

Once installed, start a new conversation, attach a screenshot of any digital UI, and use any of these prompts:

- "Audit this UI"
- "Review this screen for usability issues"
- "Run a heuristic evaluation on this design"
- "What usability problems can you see here?"
- "Check this interface against Nielsen's heuristics"

Claude will automatically invoke the skill when a screenshot is shared alongside a usability-related request.

### Multiple screenshots

You can share more than one screenshot in a single request. The skill will audit each screen individually and then add a cross-screen consistency note flagging any discrepancies between screens — relevant to H4 (Consistency and Standards).

---

## What's inside the ZIP

```
nielsen-heuristics-audit/
├── SKILL.md              — Main instructions and report template
└── references/
    └── heuristics.md     — Detailed guidance and common violation patterns per heuristic
```

The full `SKILL.md` is readable above. It contains all instructions Claude follows when the skill is active — no hidden logic, no external calls, no data collection.

---

## Limitations

- **Static images only** — the skill cannot evaluate interactions, animations, transitions, or flows
- **Works in claude.ai and Claude Desktop** — image analysis does not work in browser-based artifacts or apps that call the Anthropic API directly via fetch (CORS restriction)
- **Expert evaluation, not user testing** — this skill applies heuristic analysis, which surfaces likely usability problems but does not replace testing with real users

---

## License

This skill is released under the MIT license.

---

## Attribution

Based on Jakob Nielsen's 10 Usability Heuristics, originally published by Nielsen Norman Group. This skill is an independent implementation and is not affiliated with or endorsed by Nielsen Norman Group.

---

## About

Created as an example of how Claude Skills can be used to apply established UX frameworks in a structured, repeatable way. Contributions and improvements welcome.
