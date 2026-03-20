---
name: nielsen-heuristics-audit
description: Analyse screenshots of digital user interfaces against Jakob Nielsen's 10 Usability Heuristics. Use this skill whenever a user shares a UI screenshot and asks for a usability review, UX audit, usability analysis, heuristic evaluation, or wants to know what usability issues exist in a design. Also trigger when users ask "what's wrong with this UI", "review this screen", "audit this design", "check this for usability issues", or any variation of wanting structured UX feedback on a visual interface.
---

# Nielsen Heuristics UI Audit

This skill provides a structured usability evaluation of digital UI screenshots using Jakob Nielsen's 10 Usability Heuristics. It produces consistent, actionable audit reports that can be compared across designs and iterations.

## Important Limitations

Some heuristics require more than a static screenshot to evaluate reliably. Be transparent about this:

- **H7 (Flexibility & Efficiency)** — hard to assess without seeing user flows or interaction patterns
- **H9 (Help users recognise, diagnose, recover from errors)** — only assessable if an error state is visible in the screenshot
- **H10 (Help and documentation)** — only assessable if help features are visible on screen

When these cannot be assessed from the provided screenshot, note them as "Not assessable from static image" rather than skipping them or guessing.

---

## Audit Process

### Step 1 — Orient yourself

Before scoring, spend a moment identifying:
- What type of interface is this? (mobile app, web app, dashboard, form, e-commerce, etc.)
- What appears to be the primary user task on this screen?
- Who is the likely user? (general public, expert user, enterprise employee, etc.)

This context shapes how strictly each heuristic applies.

### Step 2 — Evaluate each heuristic

Work through all 10 heuristics in order. For each one:
1. State what you observe in the interface relevant to that heuristic
2. Assign a severity rating (see below)
3. Describe the specific issue if one exists, referencing the location on screen
4. Provide a concrete recommendation

Load the heuristic reference file for detailed guidance on each heuristic and common violation patterns:
→ See `references/heuristics.md`

### Step 3 — Produce the report

Use the report template defined below. Do not deviate from the structure — consistency across audits is important.

---

## Severity Rating Scale

Use this scale consistently. Do not inflate or deflate ratings.

| Rating | Label | Meaning |
|--------|-------|---------|
| 0 | No issue | Heuristic is well satisfied |
| 1 | Cosmetic | Minor polish issue; fix only if time permits |
| 2 | Minor | Small usability friction; should be fixed in next iteration |
| 3 | Major | Significant usability problem; high priority fix |
| 4 | Critical | Blocks or seriously impairs task completion; fix immediately |
| — | Not assessable | Cannot be evaluated from a static screenshot |

---

## Report Template

ALWAYS produce the report in this exact structure:

---

# Usability Audit Report
**Interface type:** [mobile app / web app / dashboard / form / other]
**Primary user task:** [your best read of what this screen is for]
**Screenshot provided:** [brief description of what is shown]

---

## Heuristic Evaluation

### H1 — Visibility of System Status

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H2 — Match Between System and the Real World

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H3 — User Control and Freedom

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H4 — Consistency and Standards

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H5 — Error Prevention

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H6 — Recognition Rather Than Recall

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H7 — Flexibility and Efficiency of Use

**Severity:**
[0–4 or Not assessable from static image]

**Observation:**
[what you see, or explain why this cannot be assessed]

**Issue:**
[describe the problem, or "None identified", or "Not assessable"]

**Recommendation:**
[specific fix, "No action needed", or "Review in user testing"]

### H8 — Aesthetic and Minimalist Design

**Severity:**
[0–4 or N/A]

**Observation:**
[what you see]

**Issue:**
[describe the problem, or "None identified"]

**Recommendation:**
[specific, actionable fix, or "No action needed"]

### H9 — Help Users Recognise, Diagnose, and Recover from Errors

**Severity:**
[0–4 or Not assessable from static image]

**Observation:**
[what you see, or explain why this cannot be assessed]

**Issue:**
[describe the problem, or "None identified", or "Not assessable"]

**Recommendation:**
[specific fix, "No action needed", or "Review error states separately"]

### H10 — Help and Documentation

**Severity:**
[0–4 or Not assessable from static image]

**Observation:**
[what you see, or explain why this cannot be assessed]

**Issue:**
[describe the problem, or "None identified", or "Not assessable"]

**Recommendation:**
[specific fix, "No action needed", or "Cannot assess from this screen"]

---

## Summary

**Issues found:** [total count of heuristics with severity 1 or above]
**Critical (severity 4):** [list heuristic numbers, or "None"]
**Major (severity 3):** [list heuristic numbers, or "None"]
**Minor (severity 1–2):** [list heuristic numbers, or "None"]

**Top 3 priorities:**
1. [Most urgent fix — be specific]
2. [Second priority]
3. [Third priority]

**Overall assessment:** [2–3 sentence plain-language summary of the interface's usability health]

---

## Multiple Screenshots

If the user provides more than one screenshot:
- Audit each screen separately using the full template
- After all individual audits, add a **Cross-screen consistency note** that flags any inconsistencies observed between screens (relevant to H4)

---

## Tone and Framing

This is a professional design tool, not a critique. Frame findings constructively:
- Focus on the user experience impact, not blame
- Be specific about location ("the submit button in the lower right" not just "a button")
- Recommendations should be actionable, not vague ("Add a progress indicator showing step 2 of 4" not "improve feedback")
- Acknowledge what works well where relevant — the audit is not just a list of problems
