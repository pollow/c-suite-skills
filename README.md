# C-Suite

An AI-powered executive team for solo founders. Run Claude Code skills that behave like a CEO, CMO, CPO, COO — and more — so you get real strategic work, not generic advice.

## Quick Start

1. **Clone this repo** into your project or a dedicated workspace.
2. **Run `/c-suite-onboarding`** in Claude Code. It asks ~8 questions about your business and saves a `company-profile.md` that all roles reference.
3. **Run `/ceo`** with a question or objective. The CEO will challenge your thinking, identify gaps, and dispatch specialist roles to do real work.

That's it. You're running a leadership team.

## What You Get

Each role is an **operator**, not an advisor. They do real work — web research, competitive analysis, financial modeling, product scoping, execution planning — and produce actual deliverables saved to `docs/`.

| Skill | Role | What it does |
|-------|------|-------------|
| `/c-suite-onboarding` | — | Guided survey to capture your business context |
| `/ceo` | Chief Executive Officer | Orchestrates roles, challenges assumptions, drives execution |
| `/cmo` | Chief Marketing Officer | Competitor research, positioning, go-to-market strategy |
| `/cpo` | Chief Product Officer | MVP scoping, user stories, feature prioritization |
| `/coo` | Chief Operating Officer | Processes, tool evaluation, operational planning |
| `/board-meeting` | All roles | Status review with prioritized next steps |

More roles (CFO, CTO, VP Sales, VP People) are defined inline in the CEO skill and can be dispatched as sub-agents. Dedicated skill files for these roles can be added using the template in `skills/_role-template/`.

## How It Works

### The Feedback Loop

```
You work on tasks ──→ Mark [x] in HUMAN_AGENDA.md ──→ Run /board-meeting
       ↑                                                        │
       └──────────── Get new prioritized action items ←─────────┘
```

### Key Files

| File | Purpose | Who writes it |
|------|---------|---------------|
| `company-profile.md` | Your business context | Created by `/c-suite-onboarding` |
| `HUMAN_AGENDA.md` | Action items requiring your involvement | C-suite adds items; you update status |
| `JOURNAL.md` | Log of all board meetings and CEO sessions | Written automatically by `/ceo` and `/board-meeting` |
| `docs/` | Deliverables (research, plans, specs) | Created by individual roles |

### HUMAN_AGENDA.md

This is the two-way communication channel between you and the c-suite.

**Updating status:**
- `[ ]` — Open, needs your action
- `[x]` — You completed it
- `[p]` — You're working on it

**Giving feedback:** Add `NOTE:` after any item to communicate back. Examples:
```markdown
- [x] **Customer discovery interviews** NOTE: Visited 8 restaurants. 6/8 said they'd pay $49/mo. Two said they already use MarketMan but hate it.
- [p] **Register domain name** NOTE: narrowed down to 3 options, need help deciding
- [ ] **Request MarketMan demo** NOTE: Their signup requires a business email, I don't have one yet
```

The c-suite reads these notes and adjusts strategy accordingly.

## Example Prompts

**First session:**
```
/ceo I want to build a SaaS tool for [X]. What should I focus on first?
```

**After doing customer discovery:**
```
/board-meeting
```
(Mark your completed items in HUMAN_AGENDA.md first)

**Specific questions:**
```
/cmo Who are our top 5 competitors and where are they weak?
/cpo What should be in the MVP and what should we cut?
/coo Give me a week-by-week execution plan for the next 90 days.
```

## Adding New Roles

See `skills/_role-template/ROLE-TEMPLATE.md` for the template. Create a new directory under `skills/`, add a `SKILL.md`, and the role becomes available.

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) CLI
- Skills must be in the `skills/` directory of your project
