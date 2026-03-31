# doerr-bot

A Claude skill that turns Claude into John Doerr — the OKR coach who brought structured goal-setting to Google, Intel, the Gates Foundation, and hundreds of other organizations.

Grounded entirely in Doerr's book *Measure What Matters*. Coaches in his actual voice: direct, story-driven, and relentlessly focused on outcomes over activities.

---

## What it does

**Four coaching modes:**

| Mode | What it does | When to use it |
|------|-------------|----------------|
| **Review** | Evaluates existing OKRs against Doerr's litmus tests, identifies traps, delivers concrete rewrites | "Are these good OKRs?" |
| **Build** | Interactive coaching conversation from priorities to finished OKRs, including cascading across teams | "Help me set goals for next quarter" |
| **Grade** | End-of-quarter scoring with honest assessment and learning-focused reflection | "Let's grade our Q2 OKRs" |
| **CFRs** | Coaches Conversations, Feedback, and Recognition — the companion system that keeps OKRs alive | "How do we run weekly check-ins?" |

**What it delivers:**

Every session ends with tangible artifacts, not just advice:
- Formatted OKR document (Word)
- OKR tracking spreadsheet with dashboard, weekly check-in logs, and grading sections
- North Star Metrics doc (when long-term targets surface)
- Multi-quarter Roadmap (when vision milestones surface)
- Cascade map (when coaching across multiple teams)

## Install

### Claude.ai (personal)

1. Download [`doerr-bot.skill`](https://github.com/buildwithtandem/doerr-bot/releases/latest/download/doerr-bot.skill) from the latest release
2. Go to **Settings → Customize → Skills**
3. Click **Add Skill** and upload the file

### Claude.ai (organization-wide)

1. Download [`doerr-bot.skill`](https://github.com/buildwithtandem/doerr-bot/releases/latest/download/doerr-bot.skill) from the latest release
2. Go to **Settings → Organization → Skills**
3. Upload — it will appear for all users automatically

### Claude Code

```bash
git clone https://github.com/buildwithtandem/doerr-bot.git
cp -r doerr-bot/doerr-bot ~/.claude/skills/doerr-bot
```

### Manual install from source

```bash
git clone https://github.com/buildwithtandem/doerr-bot.git
cd doerr-bot
zip -r doerr-bot.skill doerr-bot/
# Upload doerr-bot.skill to Claude via Settings → Customize → Skills
```

## What triggers it

The skill activates automatically when you mention OKRs, objectives and key results, goal setting, quarterly planning, annual planning, Doerr, or *Measure What Matters*. It also triggers on phrases like "help me set goals," "what should our priorities be," or "are these good OKRs."

## What's inside

```
doerr-bot/
├── SKILL.md                              # Core coaching instructions + Doerr's voice
├── references/
│   ├── doerr-methodology.md              # Complete OKR system: definitions, superpowers,
│   │                                     # traps, litmus tests, scoring, cascading, CFRs
│   ├── doerr-stories.md                  # 10 coaching anecdotes from Doerr's career
│   │                                     # (YouTube, Chrome, Intel, Gates Foundation, etc.)
│   ├── examples-and-patterns.md          # 6 before/after OKR rewrites + stage-specific
│   │                                     # trap patterns by company maturity
│   └── cfr-coaching.md                   # Weekly check-in format, feedback principles,
│                                         # recognition framework, monthly review structure
└── scripts/
    └── generate_tracker.py               # Generates OKR tracking spreadsheet from JSON
```

## Examples

**Review mode** — share your OKRs and get honest feedback:

> Here are our Q3 OKRs, can you review them?
>
> Objective: Increase revenue  
> KR1: Close 10 new deals  
> KR2: Launch new pricing page  
> KR3: Hire 2 sales reps

The skill will diagnose the specific traps (vague objective, activity-based KRs, no committed/aspirational distinction) and deliver a concrete rewrite.

**Build mode** — start from scratch:

> We're a 15-person biotech startup with 2 paying customers and 3 pilots. Help us figure out our Q3 priorities.

The skill will coach you through priority discovery, challenge you to pick 3–5 things that actually matter, draft objectives and measurable key results, classify committed vs. aspirational, and stress-test the whole set.

**Grade mode** — end-of-quarter reflection:

> Here are our Q2 OKRs and what actually happened. Help us score them.

The skill will walk through each KR with a 0.0–1.0 score, apply the right standard (1.0 for committed, 0.7 for aspirational), and drive a learning conversation.

## Methodology

Everything in the skill is grounded in John Doerr's *Measure What Matters*. Key principles:

- **3–5 objectives per cycle.** Less is more. If everything is a priority, nothing is.
- **Key results must be measurable.** "It's not a key result unless it has a number."
- **Outcomes, not activities.** If your KR uses words like "consult," "analyze," or "participate," it's a task, not a result.
- **Committed vs. aspirational.** Committed OKRs target 1.0 — you rearrange resources to deliver. Aspirational OKRs target 0.7 — you're reaching for something bold.
- **Pair quantity with quality.** Every speed target needs a quality counterpart. The Ford Pinto lesson: hitting every metric while ignoring what wasn't measured.
- **The sufficiency test.** If you score 1.0 on all KRs, is the objective definitely achieved? If not, rework the KRs.

## Contributing

Issues and PRs welcome. If you've used the skill and found a pattern it doesn't handle well, or a coaching moment that could be sharper, open an issue.

## License

MIT

## Credits

Methodology from *Measure What Matters* by John Doerr (Portfolio/Penguin, 2018). This skill is not affiliated with or endorsed by John Doerr or Kleiner Perkins.
