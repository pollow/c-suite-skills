# I used an AI c-suite to plan my project's launch — here's what it actually produced

*Cross-posted from personal experience building [c-suite-skills](https://github.com/pollow/c-suite-skills)*

---

Here's the meta-story: I ran `/board-meeting` on my own open source project. The AI CMO told me to post on Hacker News. So I did.

That's not a pitch. That's what actually happened.

---

## What is c-suite-skills?

It's a Claude Code skills pack that gives a solo founder a full executive team — CEO, CMO, CPO, COO, CFO, CTO, VP Sales, and CHRO — that lives in a git repo and costs nothing per seat.

You install it once:

```bash
npx skills add pollow/c-suite-skills
```

Then you talk to it like a real exec team. You ask `/cmo` to do competitive research. You ask `/cfo` to model your pricing. You ask `/cpo` to scope the MVP. You run `/board-meeting` when you need a weekly sync that tells you where things stand and what to do next.

The difference from a regular ChatGPT conversation: these aren't one-shot answers. Each role reads your `company-profile.md`, checks what's already been done, scans existing docs, and writes its deliverables to a `docs/` folder it maintains across sessions. It's agentic. It builds up a body of work over time.

---

## What a board meeting actually looks like

Here's what happened when I ran `/board-meeting` on this project.

The session read my company profile (project: c-suite-skills, goal: hit 1k GitHub stars). It scanned the existing `docs/` folder — competitive analysis, a 90-day growth plan, positioning docs already written in prior sessions. Then it produced:

- A current-state summary: skills.sh listing was live, README was solid, but no distribution had happened yet
- A gap analysis: no HN post, no dev.to article, no community channel posts
- A prioritized action list written to `HUMAN_AGENDA.md`

The top item? "Post a Show HN. Distribution first. Do this before any further development."

It drafted the post text. It told me what to include (the install command, a real output example, the meta-angle). I read it, agreed it was correct, and posted.

That's the workflow. The AI identifies the gap. It does the work. It hands off the human-only steps with a clear brief.

---

## The things it's actually good at

**Research that would take you hours.** The CMO skill will do competitive positioning, write a full launch strategy with channel-by-channel drafts, and anticipate the objections you'll face. It took 20 minutes to produce a launch doc I would have spent a day writing.

**Structured thinking under pressure.** Solo founders default to building when they're stressed. Having a `/ceo` that forces you to answer "what's the actual strategic question here" before touching code is genuinely useful.

**Deliverables in files, not chat.** Everything goes to `docs/`. You accumulate a real archive of decisions, not a scroll of conversations you'll never find again.

**Agenda management.** `HUMAN_AGENDA.md` is a living task list the AI maintains and you action. It's a simple mechanism but it changes the dynamic — you're reviewing AI-generated priorities rather than trying to remember what you decided last week.

---

## The honest limitations

**It doesn't know what it doesn't know about your market.** The output quality is proportional to how well you've written your `company-profile.md`. A vague profile produces generic advice. A sharp profile produces sharp advice.

**It won't make the hard human calls.** Which co-founder do you drop? Is this pivot real or are you avoiding the hard thing? It can frame the question well. It won't decide for you.

**It requires Claude Code.** This isn't a web app with a signup form. You need Claude Code installed and a valid Anthropic subscription. That's a real install friction that limits the audience.

**Early-stage project.** The skills are good but not perfect. Some roles are more developed than others. The COO and CMO have the most miles on them; the CFO and CHRO are functional but less battle-tested.

---

## Who it's for

Solo technical founders who are good at building and bad at the business side. People who know they need to think about positioning, pricing, and go-to-market — but keep deferring it because there's no one to do it with.

If you have a co-founder who covers business strategy, you probably don't need this. If you're building alone and your "business planning" is a Notion doc you opened twice, this might actually change how you work.

---

## Try it

```bash
npx skills add pollow/c-suite-skills
```

GitHub: [https://github.com/pollow/c-suite-skills](https://github.com/pollow/c-suite-skills)

Start with `/c-suite-onboarding` to write your company profile, then run `/board-meeting`. The first session will tell you your biggest gap. Whether you act on it is still up to you.

---

*Word count: ~750 words*
