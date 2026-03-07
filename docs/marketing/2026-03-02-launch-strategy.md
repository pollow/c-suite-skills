# CMO Launch Strategy — Community Channel Distribution

**Date:** 2026-03-02
**Role:** CMO
**Status:** Active launch window

---

## HN Post Performance Summary

**Post URL:** https://news.ycombinator.com/item?id=47229020
**Post Type:** Show HN

**Note on live data:** Web fetch was unavailable during this session. The founder must check current score/comments directly. Use the framework below to interpret what you see:

| Score Range | Comment Count | Signal | Action |
|-------------|---------------|--------|--------|
| 0–10 pts | < 5 comments | Flat | Post community channels NOW — don't wait for HN to rescue |
| 11–30 pts | 5–15 comments | Decent | Post community channels today to add cross-channel velocity |
| 31–100 pts | 15–50 comments | Good | Ride HN for 12 more hours, then post community channels |
| 100+ pts | 50+ comments | Front page | Focus entirely on HN replies for 24 hrs; community channels after |

**Known context from HUMAN_AGENDA:**
- HN post is confirmed live
- "Ran board-meeting and CMO suggested to make post on Show HN. So I did." — this is the meta-story that is working
- `npx skills add pollow/c-suite-skills` install path works; skills.sh listing is not yet live

---

## Timing Recommendation

**Default: Post community channels TODAY (within 4–6 hours of reading this).**

Rationale:
- HN Show HN posts peak engagement in hours 2–8. If you're past that window, the HN boost is already spent.
- Cross-posting to Discord/Reddit while HN is still warm creates a brief multi-channel moment that signals "this is happening right now."
- The project is in its first 48-hour launch window. Every hour of silence is lost momentum.
- Exception: if HN is actively front-page (100+ points, active comment thread), stay there and handle it. Community posts can wait 12–24 hours in that case.

**If the HN post is flat (under 10 points):** Do not mention HN in community posts. Lead with the story, not the score.

---

## Ready-to-Post: Claude Code Discord

**Target channel:** `#show-and-tell` or `#general` or `#projects`
**Tone:** Conversational, direct, no hype
**Length:** Short. Under 200 words.

---

**DRAFT — Claude Code Discord:**

> **I built a skills pack that gives solo founders an AI c-suite**
>
> It's called c-suite-skills. You get a CEO, CMO, CPO, COO, CFO, CTO, VP Sales, and CHRO — all as Claude Code skills that know your company and work like actual executives.
>
> The meta part: it manages its own growth. I ran `/board-meeting` and the CMO told me to post on HN. So I did.
>
> Install:
> ```
> npx skills add pollow/c-suite-skills
> ```
>
> GitHub: https://github.com/pollow/c-suite-skills
>
> Would love feedback — especially if you're a solo founder who's tried it or has thoughts on the approach.

---

**Usage notes:**
- Post this verbatim. Do not add emojis or exclamation points.
- If there's a thread in show-and-tell, reply directly to any question within 1 hour.
- If someone asks "does this actually work?" — link to the HN thread and/or paste a real output snippet from your board meeting session.

---

## Ready-to-Post: Reddit r/claudeai

**Target subreddit:** r/claudeai (primary), r/ClaudeAI (mirror 24h later if allowed)
**Tone:** Honest, slightly self-aware, concrete
**Length:** Medium. 300–400 words. Reddit rewards substance.
**Post type:** Text post (not link post — more visibility, allows full story)

---

**DRAFT — Reddit r/claudeai:**

**Title:** I built a Claude Code skills pack that gives solo founders an AI c-suite — and it manages its own growth

**Body:**

Solo founder here. I got tired of having no one to pressure-test decisions with, so I built c-suite-skills — a Claude Code skills framework that gives you a full AI executive team.

You get: CEO, CMO, CPO, COO, CFO, CTO, VP Sales, and CHRO. Each one reads your company profile, tracks a shared agenda, and writes deliverables to a `docs/` folder. They don't just answer questions — they identify gaps, write actual documents, and leave action items for you.

**The meta part (this is the part people find funny):**

I ran `/board-meeting` to figure out how to grow the project. The CMO's output said: post on HN, then post in community channels, reply to every comment for 48 hours. So that's what I'm doing right now. The project is literally managing its own distribution.

**Install:**

```
npx skills add pollow/c-suite-skills
```

Then create a `company-profile.md` (just a plain markdown file describing your startup), and run `/c-suite-onboarding` to get started. After that, try `/board-meeting` for a strategic review or `/cmo` for anything marketing.

**GitHub:** https://github.com/pollow/c-suite-skills

**What it's good for:**
- Reality-checking your strategy before committing to it
- Getting a second opinion that isn't just a chatbot saying yes
- Forcing yourself to write down what your company actually is
- Replacing the "talk it out with a co-founder" function when you don't have one

**What it's not:**
- It's not a replacement for real advisors on legal/financial decisions
- It's not magic — the quality scales with how good your company-profile.md is
- It's early stage, open source, and rough in places

Happy to answer questions. If you try it, tell me what broke.

---

**Usage notes:**
- Use this title verbatim. It is direct and front-loads value.
- Post body is already formatted for Reddit markdown.
- Reply to every comment within 6 hours for the first 48h. Even short replies ("good question, here's what I've seen...") keep the thread alive.
- If someone is skeptical: don't argue. Agree with the limitation, then say what it's actually good for.
- If someone asks for a demo: paste your actual board-meeting output (or the CMO output that told you to post here).

---

## 48-Hour Engagement Playbook

### First 6 Hours After Posting

**Goal:** Seed the thread with energy. The algorithm rewards early velocity.

- Reply to every comment, even short ones ("thanks for trying it")
- For skeptics: acknowledge the limitation they raised, then pivot to the use case where it works
- For enthusiasts: ask what they tried, what company profile they used
- Never delete or edit posts — shows confidence
- Don't cross-post to both subreddits on the same day; stagger by 24h

### Hours 6–24: Sustain

- Check every 2–3 hours
- Look for comments that are actually questions disguised as criticism — answer them directly
- If someone posts a screenshot of their own output, engage heavily — they're becoming advocates
- If a comment gets upvoted and you haven't replied, prioritize it

### Hours 24–48: Convert

- Identify 2–3 commenters who seem genuinely interested — reply to them specifically and ask if they'd try it on a real project
- If anyone has tried it and reported friction: acknowledge, say what you'll fix, and tag them when it's done
- Post a brief "update" comment in the Reddit thread if there's been meaningful new development (e.g., a fix you shipped based on their feedback)

### What Not to Do

- Don't spam cross-posts ("also posted in r/solofounder, r/startups, r/SideProject" all at once)
- Don't use engagement bait ("upvote if you agree")
- Don't defend every criticism — let some land; shows confidence
- Don't go silent after 6 hours — threads die when founders stop showing up

### Comment Response Templates (adapt, don't copy verbatim)

**On "is this real/does it actually work?"**
> Yeah, it works — here's the actual output from when I ran /board-meeting: [paste excerpt]. The quality depends on how good your company-profile.md is, but it does produce real deliverables.

**On "this seems like just prompt engineering"**
> That's fair — it is prompt engineering, structured as a skills framework. The value is in the protocol: every role reads your company context, tracks a shared agenda, and builds on previous outputs. You could do this manually, but you won't.

**On "what happens when the AI is wrong?"**
> Same thing that happens when a junior executive is wrong — you push back, it revises. The difference is it's not expensive and it's not offended. I've found it's better at identifying what questions to ask than at giving final answers.

**On "I tried it and X broke"**
> Thanks for reporting this. [If you know the fix: here's what to do / I'll push a fix.] [If you don't: drop an issue on GitHub and I'll look at it this week.]

---

## Notes for Next Session

- skills.sh does not yet list this project — this is a distribution gap. Should be addressed before the next launch push.
- If HN got meaningful comments, review them before community posting — incorporate any language that resonated into the Reddit post title/hook.
- The "I ran /board-meeting and the CMO told me to post here" story is the core hook. It should appear in every post, every reply thread, every description. It is the product demo in one sentence.

---

## 2026-03-06 Update

**Status:** HN 48-hour window has closed. skills.sh listing is live, badge active, install works. Community channel posts were not executed during the HN window — that simultaneous multi-channel moment is permanently missed. However, Discord and Reddit are still viable with adjusted framing.

**Key shift:** Do not use "launch moment" language. The drafts above are stale. The meta-story hook is unchanged and still strong; the framing must shift from "I just launched" to "here's a project I built and here's how it works." The HN thread can now be cited as social proof.

---

### Revised Discord Draft (use this, not the original above)

**Target channel:** `#show-and-tell` or `#general` or `#projects`

> **I built a Claude Code skills pack that gives solo founders an AI c-suite**
>
> It's called c-suite-skills. You get CEO, CMO, CPO, COO, CFO, CTO, VP Sales, and CHRO — all as Claude Code skills that read your company profile and operate like actual executives: they write deliverables, track a shared agenda, and leave action items for you.
>
> The meta part: it manages its own growth. I ran `/board-meeting` and the CMO told me to post on HN. So I did. The HN thread is here if you want to see how it landed: https://news.ycombinator.com/item?id=47229020
>
> Install:
> ```
> npx skills add pollow/c-suite-skills
> ```
>
> GitHub: https://github.com/pollow/c-suite-skills — listed on skills.sh too.
>
> Would love feedback — especially if you're a solo founder who's tried it.

---

### Revised Reddit Draft (use this, stagger 24h after Discord)

**Title:** I built a Claude Code skills pack that gives solo founders an AI c-suite — it told me how to distribute itself

**Body:**

Solo founder here. I got tired of having no one to pressure-test decisions with, so I built c-suite-skills — a Claude Code skills framework that gives you a full AI executive team.

You get: CEO, CMO, CPO, COO, CFO, CTO, VP Sales, and CHRO. Each one reads your company profile, tracks a shared agenda, and writes deliverables to a `docs/` folder. They don't just answer questions — they identify gaps, write actual documents, and leave action items for you.

**The meta part:**

I ran `/board-meeting` to figure out how to grow the project. The CMO's output said: post on HN, then post in community channels, reply to every comment for 48 hours. So that's what I did. The HN thread is here: https://news.ycombinator.com/item?id=47229020

**Install:**

```
npx skills add pollow/c-suite-skills
```

Then run `/c-suite-onboarding` to set up your company profile. After that, try `/board-meeting` for a strategic review or `/cmo` for marketing.

**GitHub:** https://github.com/pollow/c-suite-skills (also listed on skills.sh)

Happy to answer questions. If you try it, tell me what broke.

---

### Execution Order

1. **Post Discord today** — highest-leverage unblocked action, takes under 10 minutes
2. **Post Reddit r/claudeai tomorrow** — 24h stagger; review HN thread comments first and sharpen the title/hook based on what resonated
3. **Do not cross-post to multiple subreddits same day**
