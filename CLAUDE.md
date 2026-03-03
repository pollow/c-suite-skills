# C-Suite Skills

This project provides skills that act as a company's executive leadership team for a solo founder.

## Key Files

- **`company-profile.md`** — Business context. All roles read this on load. If it does not exist, invoke `/c-suite-onboarding` before doing anything else.
- **`HUMAN_AGENDA.md`** — Two-way task list between the c-suite and the human founder.
- **`JOURNAL.md`** — Append-only log of board meetings and CEO sessions.
- **`docs/`** — Role deliverables (research, plans, specs).

## Available Skills

| Skill | Purpose |
|-------|---------|
| `/c-suite-onboarding` | First-time setup or update company profile |
| `/ceo` | Strategic decisions, cross-functional questions, gap identification |
| `/cmo` | Market research, competitor analysis, positioning, go-to-market |
| `/cpo` | MVP scoping, feature prioritization, user stories |
| `/coo` | Operational processes, tool evaluation, execution planning |
| `/cfo` | Financial modeling, pricing, unit economics, runway |
| `/cto` | Technology choices, architecture, build-vs-buy decisions |
| `/vp-sales` | Sales process, outreach, pipeline, ICP |
| `/chro` | Hiring, org structure, compensation, onboarding |
| `/board-meeting` | Status review, progress check, prioritized next steps |

## HUMAN_AGENDA.md Protocol

**Status markers (set by the human):**
- `[ ]` — Open, needs human action
- `[x]` — Completed by human
- `[p]` — Work in progress by human
- `NOTE:` after any item — feedback from the human (challenges, pushback, context, questions)

**On load (all roles):**
- Read `company-profile.md` — internalize the business context.
- Read `HUMAN_AGENDA.md`.
- Treat `[x]` items with `NOTE:` as new inputs — act on them.
- Treat `[p]` items with `NOTE:` as potential plan adjustments.
- Track `[ ]` items as pending.

**When writing:**
- Append to `HUMAN_AGENDA.md` under the appropriate priority section when a task requires human action (authentication, physical meetings, payments, social media posting).
- Format: `- [ ] **Task description** — Context and why it's needed. Reference any artifacts prepared. [Added by ROLE, DATE]`
- Never remove or modify existing items. Only add new `[ ]` items.

## Journal Logging

After completing any `/ceo` or `/board-meeting` session, append a structured summary to `JOURNAL.md`. Append only — never overwrite previous entries.

If `JOURNAL.md` does not exist, create it with:

```markdown
# Journal

> Chronological log of board meetings and CEO sessions. Newest entries at the bottom.
> This file is append-only. Do not edit or delete previous entries.
```

**Entry format:**

```markdown
---

## [Session Type] — [DATE]

### Context
[What triggered this session]

### Actions Taken
- [Roles dispatched, decisions made]

### Outcomes
- [Deliverables produced (with file paths)]
- [Items added to HUMAN_AGENDA.md]

### Strategic Notes
- [Key insights, trade-offs, or open questions]
```
