<div align="center">
  <img src="c-suite-skills.png" alt="C-Suite Skills" width="180" />
  <h1>C-Suite Skills</h1>
  <p><strong>An AI-powered executive team for solo founders.</strong></p>
  <p>Ten executive role skills for Claude Code — CEO, CMO, CPO, COO, CFO, CTO, VP Sales, CHRO, and more — so you get real strategic work done, not generic advice.</p>

  <a href="https://skills.sh/pollow/c-suite-skills"><img src="https://img.shields.io/badge/skills.sh-c--suite--skills-blue" alt="skills.sh" /></a>
  <a href="https://github.com/pollow/c-suite-skills/blob/main/LICENSE"><img src="https://img.shields.io/github/license/pollow/c-suite-skills" alt="License" /></a>
</div>

---

## Install

```bash
# Install all skills (works with Claude Code, Cursor, Windsurf, and 16+ AI tools)
npx skills add pollow/c-suite-skills

# Install a single role
npx skills add pollow/c-suite-skills --skill ceo
```

Or via the Claude Code plugin marketplace:
```
/plugin install ceo@c-suite-skills
```

---

## Quick Start

1. **Install** using one of the commands above.
2. **Run `/c-suite-onboarding`** — a guided ~8-question survey that captures your business context into `company-profile.md`. All roles read this file.
3. **Run `/ceo`** with a question or objective. The CEO challenges your thinking, identifies gaps, and dispatches specialist roles to do real work.

```
/ceo I want to build a SaaS for [X]. What should I focus on first?
```

That's it. You're running a leadership team.

---

## Skills

| Skill | Role | What it does |
|-------|------|-------------|
| `/c-suite-onboarding` | Setup | Guided survey to capture your business context |
| `/ceo` | Chief Executive Officer | Orchestrates roles, challenges assumptions, drives execution |
| `/cmo` | Chief Marketing Officer | Competitor research, positioning, go-to-market strategy |
| `/cpo` | Chief Product Officer | MVP scoping, user stories, feature prioritization |
| `/coo` | Chief Operating Officer | Processes, tool evaluation, 90-day execution planning |
| `/cfo` | Chief Financial Officer | Pricing, unit economics, runway, financial modeling |
| `/cto` | Chief Technology Officer | Architecture, tech stack, build-vs-buy decisions |
| `/vp-sales` | VP of Sales | ICP, outreach templates, pipeline strategy |
| `/chro` | Chief People Officer | Hiring plans, org structure, compensation benchmarking |
| `/board-meeting` | All roles | Status review with prioritized next steps |

---

## How It Works

Every role is an **operator**, not an advisor. They do real work — web research, competitive analysis, financial modeling, product scoping — and produce deliverables saved to `docs/`.

### The Feedback Loop

```
You work on tasks ──→ Mark [x] in HUMAN_AGENDA.md ──→ Run /board-meeting
       ↑                                                        │
       └──────────── Get new prioritized action items ←─────────┘
```

### Key Files

| File | Purpose |
|------|---------|
| `company-profile.md` | Your business context — created by `/c-suite-onboarding`, read by all roles |
| `HUMAN_AGENDA.md` | Two-way task list — c-suite adds items, you update status |
| `JOURNAL.md` | Append-only log of board meetings and CEO sessions |
| `docs/` | Role deliverables — research, plans, specs |

### HUMAN_AGENDA.md

This is the communication channel between you and the c-suite. Update item status and add `NOTE:` to give feedback:

```markdown
- [x] **Customer discovery interviews** NOTE: Visited 8 restaurants. 6/8 said they'd pay $49/mo.
- [p] **Register domain name** NOTE: Narrowed to 3 options, need help deciding.
- [ ] **Request competitor demo** NOTE: Their signup requires a business email I don't have yet.
```

The c-suite reads your notes and adjusts strategy accordingly.

---

## Example Prompts

```
# First session
/c-suite-onboarding

# Strategic questions
/ceo I want to build a SaaS tool for [X]. What should I focus on first?
/cmo Who are our top 5 competitors and where are they weakest?
/cpo What should be in the MVP and what should we cut?
/cfo Model out pricing at $49/mo with 100 customers. What's the unit economics?
/cto Should we build this ourselves or use an existing platform?

# Weekly check-in (after marking completed tasks in HUMAN_AGENDA.md)
/board-meeting
```

---

## Adding Roles

See `skills/_role-template/ROLE-TEMPLATE.md`. Create a new directory under `skills/`, add a `SKILL.md` with the required frontmatter, and the role is available immediately.

---

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) or any AI coding tool that supports the [Agent Skills standard](https://agentskills.io)
