# OKR Examples and Stage-Specific Patterns

This file has two sections: before/after rewrites showing common mistakes and fixes, and stage-specific trap patterns so you can diagnose issues faster based on company context.

## Table of Contents
1. [Before/After Examples](#examples)
2. [Stage-Specific Patterns](#patterns)

---

## Before/After Examples {#examples}

Use these to show people what good looks like. When you spot a problem, say "let me show you what I mean" and walk them through a rewrite.

### Example 1: Hardware Startup (Pre-Revenue)

**Before:**
```
OBJECTIVE: Build and deploy our product
  KR1: Ship v1.0 of hardware by end of quarter
  KR2: Onboard 3 beta testers
  KR3: Gather feedback and iterate
```

**What's wrong:** The objective is an activity ("build and deploy"), not an outcome. KR1 is a milestone, not a measure of success. KR3 is hopelessly vague — "gather feedback" isn't a result. You could hit all three and still have a product nobody wants.

**After:**
```
OBJECTIVE: Prove our hardware solves a real problem for real customers
Type: Committed
  KR1: 3 beta units deployed and processing live data at customer
       sites by August 31
  KR2: Each beta customer reports ≥30% improvement on their
       primary pain point (defined per customer) within 30 days
       of deployment
  KR3: Gross unit economics documented from beta deployments —
       actual BOM, install cost, and customer willingness-to-pay
       validated through signed LOIs or contracts
```

**Why this is better:** The objective is about proof, not shipping. KR1 requires live deployment, not just manufacturing. KR2 measures the actual customer outcome. KR3 connects to business viability. You cannot score 1.0 on all three without genuinely proving the product works.

---

### Example 2: SaaS Company (Series B, Scaling)

**Before:**
```
OBJECTIVE: Grow revenue
  KR1: Increase MRR from $500K to $700K
  KR2: Close 20 new customers
  KR3: Reduce churn to below 5%
```

**What's wrong:** "Grow revenue" is so generic it could be anyone's objective at any company. The KRs are all reasonable metrics but there's no quality pairing — nothing about customer satisfaction, product quality, or whether the growth is sustainable. This is a Ford Pinto OKR.

**After:**
```
OBJECTIVE: Build a revenue engine that scales without breaking
Type: Committed
  KR1: Net new MRR grows from $500K to $700K by September 30
  KR2: Logo churn stays below 3% while net revenue retention
       exceeds 110% (expansion from existing customers)
  KR3: Average onboarding time for new customers decreases from
       6 weeks to 4 weeks without reducing NPS below 45
```

**Why this is better:** The objective says WHY growth matters — it has to be sustainable. KR1 is the quantity target. KR2 pairs growth with retention — and specifies BOTH logo churn and net revenue retention, catching the case where you keep customers but they shrink. KR3 pairs speed with quality — faster onboarding, but not at the expense of customer satisfaction.

---

### Example 3: Nonprofit / Mission-Driven Organization

**Before:**
```
OBJECTIVE: Increase our impact in underserved communities
  KR1: Launch programs in 3 new cities
  KR2: Serve 500 new beneficiaries
  KR3: Publish impact report by end of quarter
```

**What's wrong:** "Increase our impact" is a mission statement, not an objective. KR1 is a launch (activity), not an impact. KR2 measures reach, not results. KR3 is a publishing task. You could serve 500 people badly in 3 cities and publish a glossy report about it.

**After:**
```
OBJECTIVE: Prove our workforce training program produces
           measurable employment outcomes in new markets
Type: Aspirational
  KR1: 500 participants complete the full training program across
       3 new city cohorts by December 31
  KR2: ≥60% of program completers are employed in their field
       of training within 90 days of graduation
  KR3: Cost per employed graduate documented and ≤$3,000
       (validating scalability of the model beyond pilot cities)
```

**Why this is better:** The objective is about proof of outcomes, not just activity. KR1 measures completion, not enrollment (people who drop out don't count). KR2 measures actual employment — the real impact. KR3 pairs impact with economics — does this work at a cost that can scale?

---

### Example 4: Individual Contributor (Engineering Lead)

**Before:**
```
OBJECTIVE: Improve platform reliability
  KR1: Fix the top 10 bugs from the backlog
  KR2: Improve test coverage to 80%
  KR3: Complete infrastructure migration
```

**What's wrong:** Every KR is a task. Fixing bugs, writing tests, and completing a migration are things you DO — they're not outcomes. You could fix 10 bugs and have 50 new ones. You could hit 80% test coverage with meaningless tests.

**After:**
```
OBJECTIVE: Make the platform reliable enough that customers
           stop complaining about downtime
Type: Committed
  KR1: Platform uptime reaches 99.9% (measured weekly) by end
       of quarter, up from current 99.2%
  KR2: P0/P1 customer-reported incidents decrease from 8/month
       to ≤2/month
  KR3: Mean time to recovery (MTTR) for production incidents
       drops from 4 hours to under 45 minutes
```

**Why this is better:** The objective is framed around the customer experience, not internal work. Every KR is a measurable outcome — uptime, incident count, recovery time. The engineer might still fix bugs, improve tests, and do migrations, but those are HOW they achieve these results, not the results themselves.

---

### Example 5: Executive / CEO

**Before:**
```
OBJECTIVE: Lead the company through a strong quarter
  KR1: Hit revenue target
  KR2: Keep the team happy
  KR3: Maintain good relationships with board and investors
```

**What's wrong:** This is a description of the CEO's job, not an OKR. Every KR is vague — what revenue target? How do you measure happy? What constitutes "good" relationships? This is the classic business-as-usual trap.

**After:**
```
OBJECTIVE: Position the company for Series B by proving
           repeatable growth with healthy unit economics
Type: Committed
  KR1: ARR grows from $2M to $3.2M with ≥90% of new revenue
       from repeatable sales motion (not founder-led deals)
  KR2: Gross margin reaches 72% (up from 65%) by reducing
       professional services mix in new contracts
  KR3: Series B lead investor identified and in active
       diligence by end of quarter

OBJECTIVE: Build the leadership team that can scale beyond
           founder-mode
Type: Aspirational
  KR1: VP Sales hired and has independently closed ≥2 deals
       by end of quarter
  KR2: VP Engineering hired and owns the Q4 technical roadmap
  KR3: CEO time on direct selling decreases from 60% to <25%
       without revenue growth stalling
```

**Why this is better:** Two objectives instead of one vague one. Each is specific about what "strong quarter" actually means for this company at this stage. The committed OKR is about proving the business model. The aspirational OKR is about the founder transitioning from doing everything to building a team. KR3 on the aspirational OKR is the most important key result here — it pairs the hiring KRs with a quality check (did hiring actually free the CEO, or are they still selling?).

---

### Example 6: Department (Marketing)

**Before:**
```
OBJECTIVE: Increase brand awareness
  KR1: Post 3x/week on social media
  KR2: Publish 8 blog posts
  KR3: Attend 2 conferences
  KR4: Redesign the website
```

**What's wrong:** Every single KR is an activity. Posting, publishing, attending, redesigning — these are things you do. They say nothing about what changes as a result. You could post three times a week to zero engagement. You could attend conferences and generate zero pipeline.

**After:**
```
OBJECTIVE: Marketing generates measurable pipeline, not just
           content
Type: Committed
  KR1: Marketing-sourced qualified leads grow from 30/month
       to 80/month by end of quarter
  KR2: Conference presence at [Event X] generates ≥25
       qualified leads with follow-up completed within 14 days
  KR3: Website conversion rate (visitor → demo request)
       improves from 1.2% to 2.5%
```

**Why this is better:** Three outcome-based KRs instead of four activity-based ones. The team can still post on social media, write blogs, and redesign the website — but only if those activities move the numbers that actually matter.

---

## Stage-Specific Patterns {#patterns}

### Pre-Revenue / Early Stage (0–10 employees)

**The #1 trap:** Confusing milestones with objectives. "Ship v1.0" and "close first customer" are milestones on a project plan — they belong on a Gantt chart, not an OKR. The objective should be about what the milestone PROVES.

**What to watch for:**
- Every OKR is really a task list in disguise
- Objectives are about building things rather than proving things
- No distinction between committed and aspirational (everything feels committed because survival is at stake)
- Zero financial or unit economics measurement because "it's too early"

**Coaching posture:** Be encouraging but firm on outcome framing. These founders are builders — they think in terms of what they'll create, not what they'll prove. Redirect every "build X" to "prove Y by building X." Even pre-revenue companies can measure something: LOIs, waitlist signups, design partners, pilot commitments.

---

### Post-Seed / Growth Stage (10–50 employees)

**The #1 trap:** Too many priorities. The company has found something that works and now wants to do everything: new features, new markets, new hires, partnerships, conferences. Everyone is stretched thin and the OKRs reflect it — seven or eight objectives, none getting real focus.

**What to watch for:**
- More than 5 objectives per quarter
- OKRs that are really just a department-by-department task list
- No cross-functional OKRs (sales, product, and engineering each have their own world)
- The CEO's OKRs are indistinguishable from the company's OKRs

**Coaching posture:** Push hard on ruthless prioritization. "You've got eight priorities. Which three would you bet the company on?" This is where the "what are you going to STOP doing?" question is most powerful. Also push for the CEO to have personal OKRs distinct from the company's.

---

### Scaling / Series B+ (50–200 employees)

**The #1 trap:** Business-as-usual OKRs. The company has real processes now, and the OKRs start to describe what the team was already going to do anyway. "Maintain 99.9% uptime" and "Hit quarterly revenue target" are not OKRs — they're operating metrics.

**What to watch for:**
- OKRs that wouldn't surprise anyone (no real choices being made)
- Heavy cascading that turns OKRs into a bureaucratic exercise
- KRs that are all internal-facing (no customer or market outcomes)
- No aspirational OKRs — everything is committed because the culture has become risk-averse
- Alignment problems between departments that nobody wants to surface

**Coaching posture:** Challenge them to identify what they're choosing to do DIFFERENTLY this quarter. "If you deleted these OKRs entirely, would the team do anything differently tomorrow? If not, these aren't OKRs." Push for at least one aspirational goal. Surface cross-functional dependencies explicitly.

---

### Enterprise / Large Organization (200+ employees)

**The #1 trap:** OKRs as compliance theater. The process exists, everyone fills out the template, but nobody actually uses them to make decisions. OKRs become backward-looking documentation of work already planned, not forward-looking commitments that drive behavior.

**What to watch for:**
- OKRs written after the quarter starts (post-hoc rationalization)
- No visible connection between individual OKRs and company-level strategy
- Scoring is perfunctory — everything gets 0.7 because that's "good enough"
- No one can name the company's top 3 objectives from memory
- CFRs (conversations, feedback, recognition) are completely disconnected from OKRs

**Coaching posture:** Focus on transparency and honest grading. "If everyone scores 0.7 every quarter, you're either sandbagging or not paying attention." Push for fewer company-level OKRs with stronger cascading discipline, and insist that the CEO presents OKRs to the whole company quarterly (as Google does). Connect OKRs to CFRs — the goal-setting system only works if it's embedded in ongoing conversations.

---

### Nonprofit / Mission-Driven

**The #1 trap:** Confusing the mission with the objective. "End poverty" is a mission. "Reduce food insecurity by 20% in our three pilot counties" is an objective. Nonprofits often write OKRs that sound inspiring but are unmeasurable because they conflate aspiration with accountability.

**What to watch for:**
- Objectives that could be anyone's mission statement
- KRs measured in activities (programs launched, people served) rather than outcomes (lives changed, problems solved)
- No cost-effectiveness KRs (impact per dollar is the nonprofit equivalent of unit economics)
- Reluctance to set numerical targets because "our work can't be reduced to numbers"

**Coaching posture:** Use the Gates Foundation example extensively. Bill Gates is emphatic: "A mission is directional. An objective has a set of concrete steps." Push for at least one outcome-based KR per objective (not just output-based). And pair impact KRs with cost-effectiveness KRs — good intentions don't scale without sustainable economics.
