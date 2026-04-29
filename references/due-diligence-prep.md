# Due Diligence Prep

Everything a founder needs to handle DD smoothly. The 5 Ts framework, the most common DD questions and how to answer them, what goes in the data room, and the red flags founders should surface proactively.

## Table of contents

1. The 5 Ts framework
2. Common DD questions by category
3. Data room checklist
4. Red flags to surface before you're asked
5. Output format for DD prep

---

## 1. The 5 Ts framework

Every DD question maps to one of five buckets. Mapping the question helps the founder see the shape of the inquiry, not just answer in isolation.

### T1: Team

Who's building this and why are they uniquely qualified? Investors are buying the people first, the idea second.

What investors actually probe:
- Founder backgrounds and prior wins/losses
- Domain expertise relevant to this market
- Co-founder dynamics (who decides what, what's the tie-breaking process, equity split)
- Key hires already in seat
- Hiring gaps and the plan to fill them
- Advisor quality and engagement
- References from former colleagues, employees, or co-founders

### T2: Tech / Product

What's actually built, what's defensible, and what could a competitor copy.

What investors actually probe:
- What's in production today vs. roadmap
- Architecture (in plain language, not jargon)
- IP: patents, trade secrets, proprietary data
- Security posture (SOC 2 status, encryption, data residency)
- Tech debt and engineering velocity
- Vendor lock-in or single-points-of-failure (e.g., 100% of inference on one model API)
- Defensibility moat: data, network effects, integrations, switching costs

### T3: Traction

The hard numbers. This is where vague language kills you.

What investors actually probe:
- Revenue (MRR, ARR, GMV)
- Growth rate (MoM, YoY)
- Net Revenue Retention (NRR) and gross retention
- Cohort behavior (do later cohorts behave better, worse, or same as earlier ones)
- Pipeline (qualified leads, weighted pipeline value, conversion rates by stage)
- Unit economics (CAC, LTV, payback period, gross margin)
- Sales velocity (cycle length, win rate, ACV)
- Customer concentration (revenue from top 1, top 5, top 10)
- Logos: who, how big, when signed, what they pay

### T4: TAM (and market dynamics)

Why this market, why now, and how big it really is.

What investors actually probe:
- Bottom-up TAM (don't show $100B with no math; build it from your ICP × ACP × penetration)
- Why now: what changed in tech, regulation, behavior, or cost structure
- Competition: who else is in this space, why you'll win, how you're differentiated
- Market timing: is this market emerging, growing, mature, or declining
- Adjacent markets you could expand into post-Series A
- The path from current customer base to a $100M ARR company

### T5: Terms

The mechanical structure of the round and the cap table.

What investors actually probe:
- How much you're raising and what for (use of funds)
- Pre-money / post-money / discount on a SAFE
- Round structure: priced equity, SAFE, convertible note
- Existing cap table, including options pool
- Prior round terms (any preferences, MFNs, anti-dilution clauses)
- Lead status: do you have one, do you need one
- Other investors in or expected
- Target close date
- What founder ownership looks like post-round

---

## 2. Common DD questions and how to answer them

For each question: the right shape of the answer, what to avoid, and a template line.

### "What's your customer acquisition strategy and CAC?"

**Right shape:** Channels in priority order, with current CAC and trend. If CAC is high or unknown, say so honestly.

**Avoid:** "Word of mouth" as a primary channel without numbers. Vague "multi-channel approach."

**Template:**
> Three channels working today: outbound to specific titles ($X CAC), inbound from content ($Y CAC, ~30% of pipeline), partner referrals ($Z CAC but limited volume). Blended CAC is [$W], payback [N] months. We're not yet running paid acquisition, planning to test in Q2 once we have 12 months of cohort data to underwrite spend.

### "What's your retention look like?"

**Right shape:** Gross retention, net retention, and cohort behavior over time.

**Avoid:** "Retention is great" without numbers. Citing only your best cohort.

**Template:**
> Logo retention is [X]% at 12 months across all cohorts. NRR is [Y]% driven by seat expansion and tier upgrades. Earliest cohort (12 months in) is at [Z]% NRR. Most recent cohort (3 months in) is tracking [W]%, similar shape to the early cohorts. Churned customers are concentrated in [segment], we tightened ICP after we saw the pattern.

### "What's your moat?"

**Right shape:** Honest. Most early-stage companies don't have a deep moat yet, they have an early lead. Say what you have and what you're building toward.

**Avoid:** Calling something a moat when it's not (e.g., "our team" is not a moat).

**Template:**
> Three things compounding: [1] proprietary data on [X], we now have 18 months of [type of data] across [N] customers; [2] integrations with [system A, B, C], each takes 6+ months for a competitor to replicate; [3] switching costs increase with usage because [reason]. None of these are moats yet, they're early advantages. The real moat we're building is [specific thing], and we'll know it's working when [observable signal].

### "Who are your competitors and how do you win?"

**Right shape:** Map the field honestly. Pick 2–3 real competitors. State how you're different and why your differentiation matters to your ICP.

**Avoid:** "We have no competitors." "We're 10x better." Naming companies that aren't actually in your space.

**Template:**
> Three categories of competition: [Incumbent A] (legacy, what they're missing: X), [Startup B] (similar stage, what we do better: Y), and the status quo of "build it in-house with [Z]." Where we win: we're built specifically for [ICP], the others are general-purpose. Our wedge is [specific use case], and once we land we expand into [adjacent use cases]. Lost deals so far: [N], reasons: [honest list].

### "What are the biggest risks you see in the business?"

**Right shape:** Name 2–3 real risks before they ask. This earns trust fast.

**Avoid:** "Execution risk" as a non-answer. Pretending there are no risks.

**Template:**
> Three things I lose sleep over: [1] dependency on [vendor / API / partner], if they change pricing or shut us out, here's our hedge: [hedge]; [2] sales cycle length in [segment] is hard to forecast, our model assumes [X] months and we've seen [Y]; [3] we're a single-product company today, the path to second product needs to start in [timeframe] and we're not yet sure what wins.

### "What's your hiring plan?"

**Right shape:** Specific roles, in order, with timeline and rationale.

**Avoid:** "We'll hire engineers and salespeople." Vague headcount targets.

**Template:**
> Next four hires in order: (1) Head of Sales, target Q1, ex-[type of company] who's done 0-to-$5M, JD posted; (2) Senior Eng for our [system] team, replacing the consulting work we're doing now; (3) Customer Success lead, Q2 once we cross [N] customers; (4) Founding designer, Q2. Plan post-round headcount: 14 (currently 8). We'll burn ~[$X]K/month at full strength.

### "Why should we invest in this round versus wait for your Series A?"

See `references/email-templates.md`, Scenario: "Why now? Why not wait until your Series A?"

### "What's your sales cycle and ACV?"

**Right shape:** Median, with variance. Top deal, bottom deal, what causes the variance.

**Template:**
> Median cycle: [N] days from first call to signed contract. Range: [low] to [high]. ACV median is [$X], range [$Y] to [$Z]. The variance is mostly driven by [factor: deal size, security review, procurement complexity]. We've shortened the cycle from [old] to [new] by [specific change].

### "How are you thinking about pricing?"

**Right shape:** What you charge, why, what you've tested.

**Template:**
> Charging [pricing model: per seat / usage-based / per integration / etc.] at [$X]. Tested two other models in the first 6 months ([model A] and [model B]), this one had the best willingness-to-pay signal. Largest customer pays [$Y]/year, smallest pays [$Z]/year. We're underpriced relative to [comp] by ~30%, and we'll re-test pricing once we hit [milestone].

### "Walk me through your model."

**Right shape:** Lead with the assumptions, not the numbers. The numbers fall out of the assumptions.

**Avoid:** Hockey-stick projections without underwriting them. Round numbers ($100M ARR by year 3 with no math).

**Template:**
> Three drivers in the model: [1] new customer acquisition (current rate: [N]/month, model assumes [N+x]/month by Q4 driven by [hire/channel]); [2] ACV expansion (current: [$X], model assumes [$Y] driven by [feature/tier]); [3] retention (current: [%], held constant in the model). Result: [$M] ARR by end of Year 2. Sensitivity: if customer acquisition lags by 30%, we land at [$M-Z]. Comfortable showing every assumption on a call.

### "What's your fundraising history?"

**Right shape:** Every round, every check, on whichever instrument.

**Template:**
> Pre-seed: [$X] on a SAFE at [$Y] cap, closed [date]. Investors: [list]. Currently raising [$X2] seed at [target structure]. No bridge rounds, no down rounds, no off-cycle SAFEs.

---

## 3. Data room checklist

Standard contents for a seed or Series A data room. Adapt for sector. Use a tool like DocSend, Visible, Notion (with view-only sharing), Google Drive (with named-access only), or a dedicated data room product.

### Essentials (every data room)

- [ ] Pitch deck (current version)
- [ ] One-pager / executive summary
- [ ] Cap table (current state)
- [ ] Cap table (pro-forma post-round)
- [ ] Financial statements (P&L, balance sheet, cash position)
- [ ] Forward financial model (3-year, monthly)
- [ ] Use of funds summary
- [ ] Founder bios + LinkedIn links
- [ ] Org chart and current headcount
- [ ] Hiring plan (next 12 months, by role)

### Customers and revenue

- [ ] Customer list with ARR per customer
- [ ] Customer concentration analysis (top 1, top 5, top 10 by revenue)
- [ ] Cohort retention chart (12 months minimum if available)
- [ ] Churn analysis (which customers churned and why)
- [ ] 3–5 customer references (with permission)
- [ ] Sample customer contracts (with sensitive parts redacted if needed)

### Pipeline

- [ ] Active pipeline by stage with weighted value
- [ ] Sales cycle metrics (median, range, win rate)
- [ ] Top 10 in-flight deals with status

### Product / Tech

- [ ] Product roadmap (next 12 months)
- [ ] Architecture overview (1-pager, plain language)
- [ ] Security posture summary (SOC 2 status, encryption, data handling)
- [ ] Demo environment access or recorded demo

### Legal

- [ ] Certificate of Incorporation
- [ ] Founder IP assignment agreements
- [ ] Employee IP assignment agreements (every employee, every contractor)
- [ ] Stock plan documents (option pool, vesting schedule)
- [ ] Prior round legal documents (SAFEs, convertible notes, term sheets)
- [ ] Key commercial contracts (top customers, big vendors)
- [ ] Any pending or threatened litigation summary (or a clear statement that there is none)

### Optional but useful

- [ ] Press hits / mentions
- [ ] Awards or recognitions
- [ ] Customer case studies
- [ ] Founder thought-leadership (blog posts, podcast appearances)
- [ ] Advisor list with bios

---

## 4. Red flags to surface before you're asked

Investors trust founders who name their own weaknesses. The list below covers the things every founder should be ready to address proactively, especially in the first DD call.

### Customer concentration

If one customer is more than 25–30% of revenue, name it. Have a plan: how you're diversifying, expected timeline, what's in the pipeline.

> "Our top customer is 35% of ARR. We signed two more in the same segment last quarter, by Q2 the top customer should be under 25%."

### Co-founder churn

If a co-founder left, address it directly. Why they left, where they went, how the equity was handled.

> "[Co-founder name] left in [month]. Mismatched on speed, parted on good terms. Their equity was repurchased per our vesting schedule. Have a written agreement on file, available in the data room."

### Thin retention data

If retention data is too short to be conclusive, say so.

> "We only have 8 months of retention data on our largest cohort. Logo retention is 100% on that cohort, but it's early to claim great retention. Will have 12-month data by end of Q1."

### Dependency risks

If your business depends on one API, one model provider, one channel, one customer, one regulator, name it.

> "Today 90% of our inference is via OpenAI. We've validated Anthropic and Google as backup, latency parity within 15%, and would switch in two weeks if we needed to."

### Burn rate

Don't hide burn. If you're burning faster than the average for your stage, explain why and what your runway looks like.

> "We're burning [$X]/month, runway through [date] at current pace. Most of the burn is engineering, eng-led product is the strategy. Could cut burn to [$Y] in 30 days if needed."

### Competitive pressure

If a well-funded competitor just raised a big round, don't pretend it doesn't matter.

> "[Competitor] raised [$X] in October. They're going broad, we're going deep on [niche]. Our last 4 wins were all from prospects who evaluated both, won on [reason]."

### Compliance gaps

If you don't have SOC 2, GDPR processes, HIPAA BAAs, or whatever your sector requires, name it.

> "SOC 2 Type 1 is in progress, auditor engaged with [firm], target completion [date]. We don't currently have it, which has cost us deals in the [segment]. Closing the gap is part of the use of funds."

### Founder gaps

If neither founder is a domain expert, or if neither has done sales, or if there's a clear missing skill on the team, address it.

> "Neither of us has run enterprise sales before. We hired [name] as Head of Sales in [month] specifically for that. He ran $0–10M at [past company]. References available."

---

## 5. Output format for DD prep

When generating DD prep output, structure it like this:

```
# DD Response Prep - [Investor / Firm]

## At the top: send-back strategy
[One paragraph: how to send this back to the investor. Which questions to lead with, which to flag a gap on, what's still coming, what timing.]

## The questions, mapped and answered

### Q1: [Original question text from investor]
**T category:** [Team / Tech / Traction / TAM / Terms]
**Draft answer:**
[The actual answer the founder will send. Real numbers, no placeholders unless you've flagged them.]
**Gaps to flag:**
- [If anything is missing or weak, name it here. Tell the founder how to address it honestly.]

### Q2: ...
[Same shape]

## Data room status

**Ready to share:**
- [List]

**In progress / not yet ready:**
- [List, with timeline]

**Will not be in this round:**
- [E.g., we won't share full customer names without permission]

## Top 3 red flags to surface proactively
1. [Flag] - [the line to use]
2. [Flag] - [the line to use]
3. [Flag] - [the line to use]
```

This gives the founder a complete package they can use to respond to the investor and prep for the call that follows.
