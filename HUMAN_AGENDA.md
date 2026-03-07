# Human Agenda

> Items requiring human action. C-suite roles add items here; the human updates status.
>
> **Status markers:**
> - `[ ]` — Open, needs human action
> - `[x]` — Completed by human
> - `[p]` — Work in progress by human
>
> **Feedback:** Add `NOTE: ` after any item to communicate back to the c-suite.
> This can be challenges, pushback, context, or questions.

### HIGH PRIORITY

- [x] **Post "Show HN" on Hacker News** — The README manifesto tone is ready for HN. The hook ("fire your executives, hire these instead") and the self-referential angle (c-suite managing its own growth via c-suite skills) is the kind of meta-story HN rewards. Post as a "Show HN" not a link post. Include the install command and a real 1-paragraph example of output. Do this before any further development — distribution first. [Added by Board, 2026-03-02]
  - NOTE: https://news.ycombinator.com/item?id=47229020

- [ ] **Share in Claude Code community channels** — Post in the Claude Code Discord and/or Reddit (r/claudeai, r/ClaudeAI) with the same story: "I built a skills pack that gives solo founders an AI c-suite. It manages its own growth now." Link to GitHub. Reply to every comment personally for the first 48 hours. [Added by Board, 2026-03-02]
  - NOTE: Ready-to-paste drafts (Discord + Reddit) written to `docs/marketing/2026-03-02-launch-strategy.md`. Also includes 48-hour engagement playbook with pre-written responses for common pushback.
  - NOTE: [Board, 2026-03-06] HN window has closed. Original drafts are stale — use the REVISED drafts in the "2026-03-06 Update" section of the same file. Post Discord today, Reddit tomorrow (24h stagger). The meta-story hook still lands; only the framing changes from "launch" to "here's what I built."

- [x] **Fix the skills.sh badge in README** — The README has a badge linking to `https://skills.sh/pollow/c-suite-skills` which 404s because the project isn't listed. HN traffic is live right now and every badge click damages credibility. Immediate options: (1) go to skills.sh and submit the project — check for a web form or PR-based registry; (2) if submission takes more than 10 minutes to figure out, remove the badge and replace it with a GitHub stars badge instead. Step-by-step checklist at `docs/operations/2026-03-02-launch-ops.md`. [Added by Board, 2026-03-03]
  - NOTE: skills.sh listing is live, badge is active.

- [x] **Archive or remove the stale `docs/` content** — All current files in `docs/` (90-day plan, MVP scope, competitive analysis) are from a previous company profile (restaurant food waste tracking SaaS). Anyone who clones the repo will see these and be confused. Either delete them or move to `docs/examples/` with a clear note that they're sample outputs. Resolve before public launch. [Added by Board, 2026-03-02]

### MEDIUM PRIORITY

- [ ] **Post dev.to article** — Draft is ready at `docs/marketing/2026-03-07-devto-article.md`. Copy-paste and publish under your name on dev.to or Hashnode. HN didn't convert (2 points); this article creates durable organic reach independent of any launch window. [Escalated by Board, 2026-03-07]

- [ ] **Identify the 30-day revenue project** — Your 3-month objective is "run it for another project to grow to profit." Name that project now, even roughly. It anchors everything: which skills to improve, what edge cases to handle, what the POC needs to prove. You don't need to start it this week, but you need a target. [Added by Board, 2026-03-02]

- [ ] **Check GitHub star count and HN thread outcome** — The c-suite has no visibility into how the HN post actually performed (points, comments, front-page duration) or the current star count. Pull these numbers and add a NOTE below this item. This data feeds the next board meeting and determines whether the current distribution strategy needs adjustment. [Added by COO, 2026-03-06]
  - NOTE: [CMO, 2026-03-07] C-suite checked via WebFetch. HN post scored 2 points, no visible comments, no front-page duration. GitHub at 2 stars, 0 forks. HN did not convert. Mark this [x] — data is in hand. Distribution strategy must shift.

- [ ] **Post the launch write-up to dev.to or Hashnode** — CMO can draft the article ("How I used an AI c-suite to plan my own project's launch"); you post it under your own name. This drives ongoing organic search traffic long after HN fades and establishes the project's story as a reference piece. [Added by COO, 2026-03-06]
  - NOTE: [CMO, 2026-03-07] Draft written to `docs/marketing/2026-03-07-devto-article.md`. Ready to post under your name. Title: "I used an AI c-suite to plan my project's launch — here's what it actually produced."

- [x] **Run c-suite on itself for one real decision and document the output** — Pick a real business question about growing this project (e.g., `/cmo Who should we target first: solo technical founders or non-technical founders?`). Run it. Save the output to `docs/examples/`. Use this as the primary demo artifact in all launch posts. The product sells itself best when people see actual output, not just feature lists. [Added by Board, 2026-03-02]
  - NOTE: ran board-meeting and CMO suggested to make post on Show HN.

### LOW PRIORITY

- [x] **Check the `npx skills add` install path** — The README assumes `npx skills add pollow/c-suite-skills` works and is how Claude Code users discover skills. Verify this is live, works end-to-end, and matches how the skills.sh ecosystem actually distributes. If there's friction in the install, fix it before launch or the README's strong first impression dies on the second step. [Added by Board, 2026-03-02]
  - NOTE: worked, but skills.sh does not have this project.
