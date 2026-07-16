# Founder Fundraising Outreach

A Claude skill that helps founders write investor outreach that actually gets replies, and reads like a human wrote it.

Cold emails to VCs that don't get deleted. Follow-ups that add real progress instead of nagging. Replies to investor questions that don't fumble valuation or traction. Due diligence prep that surfaces gaps before investors do. Post-meeting recaps within the 24-hour window. Pipeline stall recovery scripts that work without faking competitive tension.

Built for founders raising pre-seed through Series B.

---

## The problem

Most founder cold emails to VCs get deleted in 5 seconds. The reason isn't the company. It's the email.

Four patterns kill them:

1. **Generic personalization.** "I admire your portfolio" tells the partner you mass-mailed.
2. **Vague traction.** "Strong growth" reads as "no growth."
3. **No specific ask.** "Let me know if you're interested" gets ignored.
4. **Reads as AI.** In 2026 investors filter for generated text and stop reading the second they catch it. Paul Graham said publicly he stops reading founder emails the moment he recognizes AI, because it feels like being lied to. Several funds have asked founders outright to stop sending AI-written pitches. The best email in the world still fails if the reader clocks it as generated.

Most fundraising advice is too high-level to fix any of this. Templates produce emails that read templated. Coaches charge thousands per session. AI tools cheerfully invent investor podcasts that don't exist and burn the founder's reputation.

This skill is built around what actually works at the seed and Series A level, drawn from public examples of cold emails that got founders funded (Mapistry, Box, the playbooks Jason Lemkin and Mark Suster have published) and the structural patterns of how real fundraises run.

---

## What it does

Eight modes, all routed from the same shared inputs:

1. **Cold email** — first-touch outreach, calibrated to recipient (institutional partner vs. operator angel vs. solo angel)
2. **Follow-up sequence** — full 3-message chain with timing rules, plus optional re-engagement
3. **Reply to investor inquiries** — deck requests, traction questions, valuation deflection, round status, polite pass, adversarial pushback
4. **Due diligence prep** — 5 Ts framework, gap-flagging, complete data room checklist
5. **Review and rewrite** — diagnose what's wrong with a draft and fix it, with explanations so the founder learns the pattern
6. **Mass outreach** — parameterized template with three research tiers (A: 20+ min bespoke, B: 10 min, C: 5 min)
7. **Post-meeting recap** — high-leverage 24-hour recap, calibrated to how the meeting actually went
8. **Pipeline stall recovery** — Script A (soft re-engage) and Script B (force a decision, only with real verifiable pressure)

---

## What makes it different

**Built to never read as AI.** This is the v0.10 headline. The skill treats sounding human as the top priority, above every other rule. It researches like a machine and writes like a founder typing between meetings: short, one proof point, a plain ask, uneven rhythm, no performance. It ships with a seven-layer field guide to the tells (words, phrases, constructions, punctuation, rhythm, theme, and the meta-tells that survive word-scrubbing) in `references/anti-ai-tells.md`, and runs a scrub pass on every draft before you see it. The reason this leads the list is the fourth failure pattern above. A perfect email still dies if the reader thinks a bot wrote it.

**The fabrication rule.** The skill never invents investor content (posts, podcasts, theses, portfolio companies) or founder facts (background, commits, customers, metrics). When information is missing, it surfaces a visible placeholder instead of guessing. This protects founders from sending emails referencing essays the investor never wrote.

**Voice calibration by recipient.** A cold email to Sarah Tavel at Bessemer should not read identical to a cold email to James Currier at NFX. The skill flexes between institutional, operator-angel, and solo-angel voice. Three archetypes, three tones, drawn from how those investors actually read.

**Refuses to fake competitive tension.** When a founder wants to use Script B (force-a-decision) without real pressure (no committed term sheet, no anchored close date), the skill refuses to draft it and explains why. Faked urgency is verifiable in two phone calls; real urgency closes rounds.

**Self-audits every draft.** Before showing output to the founder, the skill runs five checks: fabrication, word count, subject line quality, tone-flex (lines that condescend to the investor), and specificity (claims that need to be backed). If anything fails, it fixes it or surfaces it.

---

## Before / after

A real example of what the skill produces, given a 261-word draft a founder pasted in.

**Before (the founder's draft):**

> Subject: Disrupting the future of work with AI
>
> I hope this message finds you well. I'm David Park, founder and CEO of Helix, a revolutionary AI platform that's transforming how legal professionals work. Our world-class team consists of myself (formerly an engineer at Google, with deep expertise in machine learning) and my co-founder Anjali, who brings best-in-class product chops from her time at Asana. We're building a holistic, end-to-end ecosystem that seamlessly leverages cutting-edge AI to supercharge the entire legal research workflow [...continues for 261 words...]

**After (the skill's rewrite):**

> Subject: AI legal research for mid-market firms, $48K MRR
>
> Hi John,
>
> >>> PERSONALIZATION HOOK: read John's recent post on vertical AI. Pull one specific phrase and replace this line. Skill won't invent one. <
>
> Helix is AI legal research for mid-market law firms (50-300 attorneys). Not big-law, not solos. The legal data, workflow, and buying motion at that firm size are not what most legal-tech is built for.
>
> Where we are:
> - $48K MRR, 14 paying firms, 91% retention
> - Two AmLaw 200 firms in active pilot
>
> Team: I'm ex-Google ML engineer, my co-founder Anjali is ex-Asana product.
>
> Raising $2M seed, $700K soft-circled from legal-tech angels.
>
> 25 minutes next week?
>
> >>> CALENDLY: paste your link <
>
> Deck: docsend.com/view/helix-deck
>
> David Park

75 words instead of 261. Zero buzzwords instead of 12+. Specific traction instead of vague "interest." A real ask instead of "looking forward to hearing back."

The skill explains every change in a "why this works" section so the founder learns the pattern, not just gets one email.

---

## Install

The skill is packaged as a single `.skill` file you can install in Claude.

1. Download [`founder-fundraising-outreach.skill`](./founder-fundraising-outreach.skill) from this repo
2. In Claude, go to Settings → Capabilities → Skills
3. Click "Install skill" and select the downloaded file
4. The skill triggers automatically when you mention raising, pitching investors, sending decks, getting passed on, post-meeting recaps, investor going silent, or paste an investor email asking for a reply

You can also install it in Claude Code, or browse the source files directly in this repo if you want to read what the skill does before installing.

---

## How to use it

Just talk to Claude naturally. The skill handles the rest.

Examples that trigger it:

- "Help me write a cold email to Sarah Tavel at Bessemer"
- "Investor went silent for two weeks, what do I send"
- "VC asked for our data room, what do I send back"
- "Just had a meeting with Foundation, help me send the recap"
- "Improve this fundraising email" (paste your draft)
- "Mass outreach for our seed round, 40 investors"
- "Make this sound human" (paste any draft)
- "Does this sound like AI"

As of v0.10 the skill also fires on general email tasks, not just fundraising. If you paste any message and ask to rewrite it so it reads human, or to check whether it sounds AI-generated, it will handle that too.

The skill will ask for the inputs it needs (company one-liner, traction, target investor, etc.) and run a pre-flight check before drafting so you know whether your email is structurally strong, medium, or thin given the inputs.

---

## Status

**v0.10.0, in pilot with founders.**

This release makes sounding human the skill's top job. New in v0.10:

- A prime directive that puts never reading as AI above every other rule, with the 2026 evidence behind it
- A new `references/anti-ai-tells.md` field guide: a seven-layer tell catalog plus a scrub procedure the skill runs on every draft
- A tightened, reorganized SKILL and an expanded style guide
- Broader triggering, so the skill now also helps with general email and de-AI-ing any draft, not only fundraising

It's still stress-tested for fabrication, voice calibration, and edge cases (medium-thin inputs, adversarial replies, fake-pressure refusal). It's better than what most founders currently use. It's not perfect.

Real-world feedback is what gets it to v1.0. If you use it and something feels off, please [open an Issue](../../issues). Bug reports are more useful than compliments.

---

## Contributing

If you have a fundraising scenario the skill doesn't handle well, or a real-world pattern (a reply that worked, a follow-up that closed a meeting), open an Issue with the example. The skill improves with real-world signal, not theoretical polish.

---

## License

MIT. Use it, modify it, share it. Built for founders, free forever.

---

## Built by

[Evalyze](https://github.com/evalyze-ai). More tools for founders coming.
