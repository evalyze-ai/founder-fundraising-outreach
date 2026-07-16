# Anti-AI Tells: The Field Guide

Why this file exists: the people founders email are actively filtering for AI-written text, and they delete on detection. This file is the complete catalog of what gives AI writing away, with the evidence behind each tell, and the scrub procedure. Read it before the first draft in any conversation. The short enforcement rules live in SKILL.md's Human-voice system; this is the deep reference.

## The evidence (why this is not paranoia)

- Paul Graham, May 2026, on X: founders now email him in a "hard-hitting journalistic style" that he knows is AI "because no founder ever wrote this way before." He stops reading on detection: "It feels like being lied to." He flagged "delve" as a tell back in 2024.
- 1517 Fund (January 2026): AI-written founder emails are "generic, sanitized, and soulless," and the fund can no longer assess founder competence through them, so they skip to the next email.
- Will Richardson, Startup Daily (June 2026): the one cold email that caught his attention "wasn't polished, rather subtly self-deprecating but undeniably honest."
- Bynder consumer study: 52% of readers stop reading the moment they suspect a text is AI-generated. Klaviyo: only 13% fully trust AI-generated brand content.
- Ohio State (Bingjie Liu): recipients rate AI-generated personal messages more negatively because the sender outsourced the effort. People now run an unconscious Turing test on what they read.
- BetterUp Labs (Sept 2025): about half of recipients rate senders of AI-generic "workslop" as less capable and less reliable; 42% as less trustworthy.
- LinkedIn (May 2026, VP of Product Laura Lorenzetti): official classifiers now cap the reach of generic AI content, and LinkedIn publicly named the "it's not X, it's Y" construction as a detection signal.
- Barracuda (2025): 51% of spam email is now AI-generated, and AI spam is MORE formal and grammatically perfect than human spam. Flawless formality itself now pattern-matches to machine.
- Kobak et al., Science Advances (2025): analysis of 15M+ abstracts found 379 "excess vocabulary" words whose frequency spiked after ChatGPT's release; at least 13.5% of 2024 abstracts were LLM-processed. The word lists below are grounded in this and in Wikipedia's "Signs of AI writing" project, the most exhaustive field guide (built from thousands of confirmed AI submissions).
- 2026 detection consensus (EyeSift, SkillsLLM's avoid-ai-writing, Woodpecker's assistant tests): detection is now CLUSTER-based. Structural regularity (metronomic rhythm, outline-perfect flow) outweighs vocabulary; single tells prove nothing, co-occurring tells convict. Woodpecker's 2026 finding: inboxes are saturated with emails whose structure is "too clean" (perfect intro, pain point, value prop, CTA), and the flow itself is the tell even when the words are customized.
- Voice-drift research (2025-2026, summarized widely on LinkedIn): AI has standardized writing toward a bland "LinkedIn-average" style, and stylistic variation across the population has measurably dropped since ChatGPT's release. Writers are now deliberately roughening their prose in response, which created the second-order tells in Layer 7.
- Length and links, field data: Instantly's 2026 benchmark and Woodpecker's 20M-email dataset both put peak cold-email reply rates under 80 words with a single CTA. Deliverability guides (Mailpool 2026, Woodpecker, Overloop) converge on zero links and zero attachments in a first touch, and investor-outreach data shows asking permission to send the deck outperforms dropping it. Short, linkless, one-fact emails are simultaneously the highest-converting and the least machine-looking. That is not a coincidence: length, links, and metric-stacking are all machine signatures.

## The three detection layers

1. **Humans pattern-matching.** The layer that matters most. The penalty is binary: once flagged, the content stops mattering and trust collapses.
2. **Platform classifiers.** LinkedIn's slop classifier is live. Email providers do not run an explicit AI flag, but generic mass patterns die through engagement-based filtering anyway, and links/attachments in cold sends feed the spam scorers directly.
3. **Detector software** (GPTZero, Originality, Copyleaks, etc.). They score perplexity (word predictability), burstiness (sentence-length variance), and classifier fingerprints. They are unreliable: documented false-positive rates above 60% for non-native writers, and they have flagged the US Constitution. Some recipients run them anyway. The same writing that beats the human layer (specific, varied, real) scores human here too, as a side effect.

The one fix for all three layers: research like a machine, write like a founder on their phone. Specificity raises perplexity. Casual uneven rhythm raises burstiness. Both are what real founders sound like anyway.

---

## Layer 1: Words (era-tiered blacklist)

LLM vocabulary shifts by model generation. Delve peaked 2023 to mid-2024, then collapsed. Newer models lean on emphasizing, enhance, highlighting, showcasing. Scrubbing only the famous words fights the last war; the full list and the constructions below matter more.

| Tier | Words |
|---|---|
| Classics (2023-2024 era, still radioactive) | delve, tapestry, landscape (abstract), realm, beacon, symphony, journey/roadmap (figurative), testament, "stands as a testament", garner, bolster, intricate, meticulous |
| Current wave (2025+) | emphasizing, enhance, highlighting, showcasing, fostering, "align with", elevate |
| 2026 LinkedIn-average abstractions | impact (bare noun), alignment, insights, momentum (figurative), efficiency (bare), scalability, and the hollow intensifiers: genuine, meaningful, truly, "real impact" |
| Fake-precision adjectives | pivotal, crucial, robust, vibrant, multifaceted, comprehensive, unwavering, seamless, holistic, dynamic, cutting-edge, future-ready, transformative, revolutionary |
| Marketing verbs | leverage, harness, unlock, unleash, ignite, empower, foster, showcase, underscore, highlight, streamline, optimize, navigate (figurative), embark, uncover, demystify, supercharge, turbocharge |
| Quantity inflation | myriad, plethora, "diverse array", "a wealth of", countless |
| Sentence-starter adverbs | Additionally, Moreover, Furthermore, Notably, Ultimately, "In conclusion", "In essence", and any "Let's + verb" ("Let's explore", "Let's break this down") |
| Stock fillers | "valuable insights", "ever-evolving", "fast-paced", "in today's digital age", "at its core", "in the heart of", nestled, "game-changer", "best-in-class", "world-class", "mission-critical", "key" (as adjective) |

Replacement principle: concrete noun or active verb, in the simplest available word. Not "leverage our platform to optimize workflows" but "cut your close time from 9 days to 2." Simple wording is itself a human signal: use, help, buy, run, build. If a smart 12 year old would stumble on a word, swap it.

## Layer 2: Phrases (email-specific)

**Openers, delete on sight:**
- "I hope this email finds you well" / "I hope you're doing well"
- "I wanted to reach out" / "I'm reaching out because"
- "My name is X and I'm the founder/CEO of Y"
- "In today's fast-paced world" / "in the ever-evolving landscape of [industry]"
- "As a [busy investor / business owner], you know..."
- "I came across your profile/company"
- "I know you're busy, so I'll keep this brief" (announcing brevity instead of being brief)

**Hooks and pivots (the cheesy transitions):**
- "Let's dive in" and any "diving into"
- "Here's the thing:" / "But here's the kicker:" / "That's only half the story"
- "Why does this matter?" / "Real talk:" / "Here's the truth" / "Let that sink in"
- "Picture this..." / "Imagine a world where..."
- "And honestly? That's rare." (quoted verbatim in 2026 community threads as a new top tell)

**Body:**
- "pick your brain" / "hop on a quick call" / "no pressure at all" / "feel free to"
- Hollow empathy: "I know how challenging fundraising can be"
- "This email aims to..." (the "aims to" tell)
- "It is important to note/consider..."
- Presumptive triggers: "Since you're scaling your team..." / "As you look to expand..." (confident claims about the recipient's situation with no citable source; a named 2026 AI-SDR fingerprint)

**Follow-up leads (all banned):**
- "Following up" / "Just following up on my last email"
- "Circling back" / "Bumping this to the top of your inbox"
- "Just checking in" / "Gentle reminder"
- Approved replacements: lead with the new fact itself, or "One thing I left out last time:", "Quick update:", "putting [Company] back on your radar"

**Closers:**
- "Looking forward to hearing from you at your earliest convenience"
- "Let me know if you have any questions or concerns"
- "Don't hesitate to reach out" / "Thanks in advance"
- Chatbot leakage: "I hope this helps", "Certainly!", "Would you like me to..."

**Emoji:** none in professional outreach. The rocket, checkmark, and fire (and emoji in headlines generally) are documented 2026 AI-copy fingerprints across every major model.

## Layer 3: Constructions (the deep tells; these survive word-scrubbing)

**1. Negative parallelism.** "It's not X, it's Y." "Not just X, but Y." "This isn't about the deck. It's about the list." LinkedIn named this as an explicit detection signal in May 2026. Wikipedia documents it at length. The number one community-cited tell of the post-em-dash era.
Fix: take the position directly. "The list is what matters here."

**2. Fragment stacks and slogan cadence.** "Short. Isolated. Trying to feel reflective." The "No X. No Y. Just Z." shape ("No hardware. No fees. Just growth."). And the negation-contrast fragment: "It's pre-seed. But not like other pre-seed." 2026 detection guidance (SkillsLLM) calls metronomic rhythm the single highest-weighted structural signal: when every line lands like a slogan with near-identical length and the same 2-3 word punch pattern, the email reads like copy-deck output no matter how casual the words are. Humans drop ONE fragment for emphasis; real fast typing produces run-ons and comma splices, not ad copy.
Fix: maximum one fragment per email, never stacked, never as a recurring rhythm. Break parallel lines on purpose.

**3. Rule of three.** Triple adjectives, triple phrases, three parallel bullets of identical shape. Wikipedia: LLMs use it to make superficial analysis look comprehensive.
Fix: use two, or four, or one strong one. Break the symmetry on purpose.

**4. Question? Answer.** "The result? More meetings booked." "The takeaway? Speed wins." A rhetorical question immediately answered.
Fix: state the point. "Meetings doubled."

**5. Copulative avoidance.** "serves as," "stands as," "marks a," "represents," "boasts," "features," "offers" where is/has belongs. Documented: a 10%+ drop in is/are usage in 2023 academic writing, with no prior trend.
Fix: "Quill is the ops layer." "The platform has four modules."

**6. Participial tails.** Sentence + ", highlighting our commitment to..." / ", ensuring seamless onboarding" / ", positioning us as..." Superficial -ing analysis bolted onto sentence ends.
Fix: cut the tail. If the claim matters, give it its own sentence with its own evidence.

**7. Elegant variation.** Synonym-cycling driven by repetition penalties: the company, the firm, the organization, the venture, all in one email. Humans repeat words.
Fix: repeat the word.

**8. Hedging and fake balance.** "It's worth noting that," "While X is true, it's also worth considering Y," "It could be argued," "Generally speaking." RLHF safety language; reads as fear of being wrong.
Fix: take the position or cut the sentence.

**9. Vague attribution.** "Experts argue," "industry reports suggest," "observers have noted," "many founders struggle with."
Fix: name the source or drop the claim.

**10. Numbered frameworks in emails.** "Here are 3 ways..." "We see 4 key challenges..." Claude-era models in particular default to framework packaging. In a blog post it's a style; in a 60-word cold email it reads consultative and machine-made.
Fix: make the one point that matters. The other two go in the call.

**11. Presumptive triggers.** Overconfident statements about the recipient's specific situation without a verifiable source ("Since you're scaling your sales team..."). A documented AI-SDR fingerprint: the model invents a plausible pain to pivot from.
Fix: only reference recipient facts you can cite (their post, their investment, their public statement). Otherwise open with your own identity or fact.

**12. The template meta-structure.** Subject with wordplay, one-line role hook, one smooth pain sentence, benefit bullets, low-friction CTA. Woodpecker's 2026 tests: this flow is now recognized on sight even with fully customized vocabulary, because the joins are too smooth and the sequence too complete.
Fix: don't run a persuasion arc. State who you are, what the thing is, one fact, one question. Four blocks, blank lines between, no connective tissue.

**13. Stacked metric strings.** "$40K MRR, 35% MoM, 11 customers, 92% retention." Four facts compressed into fourteen words is machine efficiency, not human recall. Real founders under time pressure give you the one number they're proud of.
Fix: one proof point per email, carrying at most a number or two inside it. Rotate the rest across follow-ups.

## Layer 4: Punctuation

- **Em dash:** still the loudest single mark. LLMs use them where humans use commas, parentheses, or colons, in a formulaic punched-up way. Newer models suppress them (GPT-5.1 era), so absence proves nothing, but presence still trips the alarm. Banned.
- **Semicolon:** now AI-associated too (documented through 2025-2026; multiple writers report clients asking them removed). In a cold email a semicolon was always overdressed; now it's overdressed and suspicious. Banned in output.
- **En dash as a sentence break:** getting caught in the same net. Fine inside ranges ($250-500K, Tue-Thu). Banned as a break.
- **Optional compound hyphens:** not a documented detector signal (style guides still endorse them, AP defends them), but a REGISTER signal with real evidence behind it: fast informal human typing routinely drops them, and perfect compound-modifier hyphenation everywhere reads as edited prose. Write "early stage fund," "first time founder," "real time data" in email prose. Keep hyphens in ranges, fixed tokens (B2B, 510(k)), and anywhere dropping one creates a genuine misread. An email with zero dashes of any kind reads dashed-off, which is the target.
- **Colon-label cadence:** "The challenge: ... The solution: ... The result: ..." and "Bold Header: explanatory sentence" bullets. AI almost always formats lists this way. Banned. In cold emails, no colons at all, body or subject; the colon is list-machinery a phone-typer never reaches for.
- **Perfect formal punctuation in a casual register:** Binghamton research (Klin et al., Computers in Human Behavior): text replies ending in a period read as less sincere, and punctuation in casual channels conveys negativity and stiffness. AI defaults to formal-perfect punctuation everywhere; that mismatch is the tell. Underpunctuate on purpose: roughly one comma per sentence or fewer, an occasional comma splice ("We launched in March, revenue doubled since"), clauses left unbuttoned.
- **Curly quotes and apostrophes:** a chatbot copy-paste artifact, flagged by Wikipedia editors along with odd Unicode bullets. Straight quotes only.
- **Exclamation points:** one can read warm and human (Klin's follow-up found exclamation marks read as MORE sincere in casual messages). Stacked, or in a cold first touch, they read as AI enthusiasm. Max one, warm contexts only.

## Layer 5: Rhythm and structure

- **Low burstiness, the umbrella tell.** AI text is uniform in sentence length and complexity. Humans mix a long three-clause sentence with a short one, then a fragment. Detectors score this; readers feel it without naming it. SkillsLLM's 2026 guidance weights metronomic pacing above every vocabulary signal.
- **The rectangle paragraph.** Three sentences, all 15-20 words, every paragraph the same size. A visual grid.
- **Listicle uniformity.** Every bullet the same length and shape, each opening with a bolded label.
- **Register mismatch.** Four structured paragraphs answering a one-line email. A 2-line investor email gets a 2-line reply.
- **Markdown artifacts** (asterisks, ###) pasted into email, headers in a 60-word message.
- **The hard-hitting journalistic style.** Graham's tell: dramatic declaratives, sales-page staccato, newsletter cadence. Founders write hurried and plain, not like Morning Brew.
- **Length itself.** A 150-word first touch signals a writer with unlimited time, which no founder has. The 2026 reply-rate data and the human-read both point the same way: under 80 words.

## Layer 6: Content and theme

- **Could-be-sent-to-anyone genericity.** No numbers, names, dates, or details only this sender could know about this recipient. The single biggest thing investors say they screen for.
- **Over-personalization, the opposite failure.** Three researched personal details in one short email reads like enrichment-tool output (because it usually is) and can tip into creepy ("saw you went to Michigan and love hiking"). One recipient-specific detail, one line, then move on. Thesis fit does more work than personal flattery.
- **Empty significance and hollow empathy.** "A pivotal moment," "part of a broader movement," "I know how hard fundraising is."
- **Polished but unowned.** Grammatically perfect, totally forgettable. No scars, no opinion, no contrarian detail, nothing risked.
- **Comprehensiveness theater.** Covering every angle evenly instead of going deep on the one thing that matters.
- **Claims that outrun facts.** Regulatory, legal, and certification words ("cleared," "approved," "patented," "HIPAA compliant") stated one notch stronger than reality. Sophisticated investors verify these in minutes, and the correction email costs more credibility than the modest claim ever would have earned.

## Layer 7: Meta-tells (the second-order generation)

- **Humanizer syntax salad.** Paraphrasing tools that beat detectors create a new tell: correct grammar with bizarre word swaps ("paramountly significant"). Never use or recommend humanizer tools.
- **Fake typos.** A tool that adds typos for you exists and is publicly mocked by VCs. Manufactured imperfection is a tell and a trust killer. Real casual is fine; deliberate errors never.
- **Costume casualness.** By mid-2026, "lowercase, minimal punctuation, typed on phone" is a selectable tone in AI outreach tools and a widely shared prompt pattern. The result: forced-casual style is now itself scanned for. The giveaways are perfectly consistent lowercase (no natural slips), comma splices that are still rhythmically smooth, and casual styling wrapped around generic content. Casualness only reads human when it sits on top of real specifics and uneven rhythm. Light punctuation yes, gimmick styling no, and never all-lowercase as a costume.
- **"I wrote this myself, not AI" disclaimers.** Saying it raises the question.
- **Template convergence.** When one tool produces one recognizable skeleton at scale, the skeleton becomes the tell. This is why this skill rotates structures, rotates proof points across batches, and retired its own fixed traction block.

---

## The scrub procedure (run as review check 8)

1. Scan for blacklist words, including the 2026 LinkedIn-average abstractions and hollow intensifiers. Target: zero.
2. Scan for banned phrases (openers, hooks, follow-up leads, closers, presumptive triggers, emoji). Target: zero.
3. Scan for the thirteen constructions. Target: zero hits, with the single allowed fragment as the only exception.
4. Punctuation pass: no em dashes, no semicolons, no en-dash breaks, no colons in cold emails, no colon-label cadence, no bold-label bullets, straight quotes, max one exclamation (warm only), optional compound hyphens dropped, at least one clause left unbuttoned.
5. Rhythm pass: at least one sentence under 7 words and one over 18; no three consecutive sentences of similar length; paragraphs uneven; max one fragment; no bullets in cold emails under 80 words.
6. Content pass: exactly one proof point, at most one recipient-specific detail, no stacked metrics, no claim stronger than the founder's own wording. Could any sentence appear in anyone else's email? Rewrite it until it could only be this founder's.
7. Mechanics pass (cold first touch): zero links, zero attachments, zero calendar links, subject under 55 chars with no colons or dashes, body 40-70 words.
8. The three gates:
   - **Pub test:** would the founder say this sentence out loud to a friend over a beer?
   - **Phone test:** does the whole thing read like a busy person typed it between meetings, knowing their numbers cold?
   - **Graham test:** if Paul Graham received this, does anything smell machine-made?

Fail any step, fix before the founder sees the draft.

## What NOT to do (worth repeating)

- No humanizer tools. No fake typos. No costume casualness. No "written by a human" disclaimers. No chasing detector scores; the target is the human reader, and writing only this founder could have written beats the software as a side effect.
- Casual is not sloppy. Errors still hurt (research shows mobile framing softens the penalty, it doesn't erase it). Casual means contractions, plain simple words, light punctuation, dropped optional hyphens, uneven rhythm, brevity.

## Maintenance note

This catalog decays. Vocabulary tells shift with each model generation (delve already faded; the LinkedIn-average abstractions are the current wave). Constructions and rhythm tells are more durable than words, and the 2026 shift to cluster-based detection means no single scrubbed item saves a draft whose structure is machine-shaped. When in doubt, the doctrine holds even as the lists age: short, specific, real, owned, and slightly uneven beats polished, generic, and symmetric, in every era.
