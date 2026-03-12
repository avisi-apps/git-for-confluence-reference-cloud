# GFC Demo 2026 — Asset Flow Guide

This is the order to show the assets and what to say at each moment.  
All files live in `avisi-apps/git-for-confluence-reference-cloud`.

---

## 1. README.md — The instant "aha"

**When:** Opening demo moment (Q5 in the script — "show us how you'd embed something")

**What to do:**  
Paste the raw GitHub URL into a Confluence page live. It renders immediately.

**What to say:**  
> "Paste a URL, see the content. No configuration. No sync schedule. It's reading directly from the repo right now."

**Why it works:**  
Zero setup visible to the audience. Markdown with tables renders cleanly. Non-technical people in the room immediately get it.

---

## 2. CHANGELOG.md — The sync moment

**When:** Q3 in the script — "walk me through why stale docs are painful"

**What to do:**  
Show the Confluence page with CHANGELOG embedded. Then open the GitHub file, change the version number or add a line to `[2.4.0]`. Commit. Reload the Confluence page.

**What to say:**  
> "I just pushed a change. No manual update, no copy-paste. The page reflects what's in the repo right now."

**Why it works:**  
This is the single most memorable moment in the demo. The audience sees the sync happen live. It makes the "stale docs" argument real.

---

## 3. system-overview.mmd — Diagrams as code

**When:** Q7 in the script — "can you show what diagram support looks like"

**What to do:**  
Show the Mermaid file in GitHub (plain text). Then show it rendered in Confluence — the full component diagram with color-coded layers.

**What to say:**  
> "This is a text file in Git. Developers update it in their normal workflow. Confluence renders it as a diagram automatically. No Lucidchart, no manual export."

**Why it works:**  
The gap between "text file" and "visual diagram" is striking. Directly answers the Lucidchart comparison question audiences always ask.

---

## 4. deploy-flow.puml — Sequence diagram, different format

**When:** Immediately after system-overview, still in the diagrams section

**What to do:**  
Show the `.puml` file, then its Confluence rendering — the full deployment sequence from git push to production.

**What to say:**  
> "Same principle, different format. PlantUML, Mermaid, they all render. The diagram lives next to the code it describes."

**Why it works:**  
Shows format breadth without a long explanation. Two diagrams back to back makes the point.

---

## 5. api.yaml — The closer for technical audiences

**When:** Q12 in the script — "how does OpenAPI rendering play out in practice"

**What to do:**  
Show the raw YAML in GitHub. Then show it in Confluence — endpoints listed, parameters formatted, response schemas readable.

**What to say:**  
> "Your API spec is already in the repo. Embed it here. Product, support, and sales can read the same docs your developers maintain. Nobody duplicates work."

**Why it works:**  
Non-technical people seeing formatted API docs is always striking. Makes the "single source of truth" claim tangible.

---

## 6. compliance/security-policy.md — The surprise use case

**When:** Q11 in the script — "a use case that surprised you"

**What to do:**  
Show the security policy rendered in Confluence. Point to the version number and last-updated date at the top. Mention it's traceable to a Git commit.

**What to say:**  
> "A team keeps all their security policies in Git — version controlled, auditable. When auditors ask for documentation, everything traces back to a specific commit. We didn't build this for that. They just found it."

**Why it works:**  
It's unexpected. Compliance and audit trails resonate strongly with the enterprise and aerospace/defense segment in your audience. Ends the demo on a use case that expands the imagination.

---

## Total runtime estimate

| Asset | Time |
|---|---|
| README embed live | ~2 min |
| CHANGELOG sync moment | ~3 min |
| system-overview + deploy-flow | ~3 min |
| api.yaml | ~2 min |
| security-policy | ~2 min |
| **Total** | **~12 min** |
