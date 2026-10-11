# Game Design — Glossary & Frameworks

Attributed by author and work. Page numbers are deliberately absent: across this corpus the
majority of page references were unverifiable (print- or lending-restricted sources), so cite
author + work only. `[UNVERIFIED]` marks claims the research could not confirm; `[synthesis]`
marks constructions of this corpus rather than any single source.

---

## Loops

| Term | Meaning | Source |
|---|---|---|
| **Skill atom** | The indivisible unit of play: goal → action → simulation → feedback → updated player model. | Cook, *Chemistry of Game Design* (01) |
| **Loop** | What repeats. A chain of skill atoms. | Cook, *Loops and Arcs* (01) |
| **Arc** | What does **not** repeat — a one-shot tension/release structure that paces loops. | Cook (01) |
| **Grind** | Repetition with no downstream skill atom. | Cook (01) |
| **Reciprocal / figure-8 loop** | Two loops that feed each other; the engine of compounding play. | Cook (01) |
| **Tight vs loose systems** | How much the player can vary a loop before it breaks. Cook's tuning toolkit. | Cook (01) |
| **Loop stack** | Moment → Core → Session → Meta. Retention lives in the seams between them. | [synthesis] of Cook, Sellers, Luton, Koster (02) |
| **Exit state** | The designed state in which a session ends — it should imply the next session. | Luton, via 02 |
| **Return trigger** | What specifically brings a player back. Needs **time + claim + sender**; persistence alone is a property, not a trigger. | Luton, via 02 |
| **Seam failure** | Churn (no meta payoff) · obligation (no satisfying core) · exhaustion (no session frame). | [synthesis] (02) |
| **Pattern mastery** | Fun is the brain's reward for mastering a pattern; boredom is a mastered pattern. The design clock. | Koster (09) |

## Motivation

| Term | Meaning | Source |
|---|---|---|
| **Autonomy · Competence · Relatedness** | The three basic psychological needs. | Deci & Ryan (04) |
| **Need frustration** | A separate pathway from low satisfaction — worse than mere absence. | SDT literature (04) |
| **Overjustification / undermining effect** | Expected tangible rewards for an interesting activity reduce intrinsic motivation. Pooled d ≈ −0.35 to −0.40 on high-interest tasks; both sides of the dispute agree on this cell. | Deci 1999; Cameron 2001 (04) |
| **Informational vs controlling rewards** | Feedback that informs supports autonomy; rewards that control undermine it (Cognitive Evaluation Theory). | SDT (04) |
| **PENS** | Player Experience of Need Satisfaction — SDT's game-specific instrument. Only partially validated. | Ryan, Rigby & Przybylski (04) |
| **Flow** | Challenge–skill balance, clear goals, immediate feedback; the channel between anxiety and boredom. Empirically contested; incompatible with deception. | Csíkszentmihályi (05) |
| **Player's journey** | Discovery → Onboarding → Habit-building → Mastery. | Amy Jo Kim (06) |
| **Social Action Matrix** | Compete · Collaborate · Explore · Express — verbs, not personality buckets. | Amy Jo Kim (06) |
| **Hard / Easy / Serious / People Fun** | The 4 Keys: mastery · curiosity · meaning · sociality. Emotions in play are often *not* fun in the moment. | Lazzaro (07) |
| **8 Kinds of Fun** | Sensation, Fantasy, Narrative, Challenge, Fellowship, Discovery, Expression, Submission. | LeBlanc (03) |
| **Bartle types** | Achievers, Explorers, Socialisers, Killers. Categorical, descriptive, unaudited (n≈30); the canon's most-misused framework. | Bartle (08) |
| **Yee / Quantic Foundry model** | 12 motivations in 6 clusters; dimensional, quantitative, built to be falsified. Yee's data **failed to recover Explorer**. | Yee (08) |
| **Typology audit** | Not "what type is this person" but "whose motivations does this design reward, and who does it starve?" | [synthesis] (08) |

## Aesthetics & design method

| Term | Meaning | Source |
|---|---|---|
| **MDA** | Mechanics → Dynamics → Aesthetics. One-way causality; design backwards from the aesthetic target. A fault *locator*. | Hunicke, LeBlanc, Zubek (03) |
| **Meaningful play** | Discernible + integrated action→outcome. The causal test MDA lacks. | Salen & Zimmerman (03) |
| **Lens** | A named question-set for interrogating a decision. Combinatorial; questions, not rules. | Schell (10) |
| **Lens of Essential Experience** | Start from the experience the player should have, not the game. | Schell (10) |
| **Interest curve** | Hook → rising peaks with valleys → finale; fractal across scales. | Schell (10) |
| **Elemental Tetrad** | Mechanics, story, aesthetics, technology — a *diamond on a visibility gradient*, not a tetrahedron. | Schell (10) |
| **Second-order design problem** | You design the rules; players produce the dynamics. | Salen & Zimmerman (03) |

## Social & party play

| Term | Meaning | Source |
|---|---|---|
| **Jack Principles** | Maintain pacing · create and maintain the **illusion of awareness** · shared control. | Jellyvision (12) |
| **One screen, many phones** | Shared screen as host; personal phones as controllers; room code; no install. | Jackbox (12) |
| **Death as a state, not an exit** | Eliminated players keep voice, presence, and some agency (BotC: one vote). | Blood on the Clocktower (11) |
| **Enumerated discretion** | Judgement = selection from supplied options, never fabrication. The Storyteller's rule, transferable to an AI narrator. | BotC (11) |
| **Confirmed-good problem** | Any mechanic that can certify an honest player collapses a hidden-role game. | BotC (11) |
| **Hidden malfunction** | A player who is silently *wrong* rather than lying — structural unreliability. | BotC (11) |
| **One asymmetry is the game** | Add a second only if it changes the endgame. | The Resistance (13) |
| **Climax last** | Place the decisive moment *after* the apparent resolution (the Assassin). | Avalon/Resistance (13) |
| **Relocated elimination** | Removing elimination only moves it into the social layer. | The Resistance (13) |
| **Play community** | The unit of design is the community that plays, not the game. Authority transfers from rule-maker to room. | De Koven (14) |
| **Game community (failure)** | Drift where the rules decide who is good enough to play. | De Koven (14) |
| **Appropriation** | Players take and remake the game; the physical context is constitutive, not a container. | Sicart (15) |
| **Lusory attitude** | The voluntary acceptance of rules for the sake of the game. A game is the voluntary attempt to overcome **unnecessary obstacles** — the obstacle is the point. | Suits (25) |
| **Magic circle** | The bounded play-space. **Correction:** Huizinga named the *play-ground*; "magic circle" appears once in a list. The concept was formulated by Salen & Zimmerman (2003). | 25 |

## Persistent worlds & live-ops

| Term | Meaning | Source |
|---|---|---|
| **Persistence = run it forever** | A world never resets; the design consequence of that. | Koster (16) |
| **The social fabric is the content** | People, not systems, are what a persistent world is made of. [paraphrase] | Koster (16) |
| **Ownership is the barrier to departure** | Investment makes leaving costly. A lever and an ethical line. | Koster (16) |
| **Never let the world feel empty** | Decide what a lone arrival finds — and what the last session left behind. | Koster (16) |
| **Worlds must change on the real calendar** | If the world is identical after a week away, absence is free. | Koster (16) |
| **Empty-world death spiral** | Population falls → encounters thin → player types decouple → newcomers bounce → repeat. | Koster; 16, 18 |
| **Critical mass Φ** | The minimum viable population. Not a constant — a function of mode, roles, skill spread, time of day. Small games beat it by **synchronisation, not scale**. [preprint source] | 18 |
| **Cold start / atomic network** | The smallest self-sustaining instance; the thing to launch first. | 18 |
| **Content treadmill** | Players consume content faster than it can be produced. Unwinnable; use their stories instead. | 16 |
| **World as database** | History is generated, stored, and then must be *retrieved*. Generation is cheap; curation and retrieval are the work. | Dwarf Fortress (17) |
| **Monuments as retrieval interfaces** | Physical/digital objects that make history legible to people who weren't there. | DF + EVE (17) |
| **Legibility is the binding constraint** | DF suffocates in ~1 GB of history; EVE's is legible only to an elite. | 17 |
| **Turn boundary** | Simultaneously a synchronisation point and a deadline. The only moment that must be shared. | Diplomacy / Neptune's Pride (19) |
| **The between-turn window is the gameplay** | In async games the gap is the game, not the turn. | 19 |
| **Do not mechanise trust** | Unenforceable promises are the point; making betrayal impossible makes the game smaller. | Diplomacy (19) |
| **Presence advantage** | Rewards whoever has the most free time, unless equalised. | Neptune's Pride (19) |

## AI narrative

| Term | Meaning | Source |
|---|---|---|
| **Drama manager** | A system that sequences authored dramatic beats against a tension arc; wakes only at beat boundaries. | Façade (20) |
| **Structure vs surface** | Author the *logic* of drama; generate the *language*. The single most important AI-narrative lesson. | Façade (20) |
| **Re-entry layer** | Gist points · repeat · reestablish · local deflect — how the drama absorbs a late arrival. | Façade (20) |
| **Memory stream** | An append-only prose log; the substrate of a persistent LLM character. | Generative Agents (21) |
| **Retrieval score** | `recency + importance + relevance`; recency decays by last access, importance judged at write time, relevance against a *named* query. | Generative Agents (21) |
| **Reflection** | Triggered when accumulated importance crosses a threshold; synthesises insights that write back into the stream. The cure for amnesia. | Generative Agents (21) |
| **Simulate, don't script** | Model social state; author conditions and pools, not sequences ("quantum authoring"). | Versu / Prom Week (22) |
| **Felt-meaning gap** | Simulated social meaning can still read as arbitrary. LLMs ease authoring burden, not this gap. | 22 |
| **Procedural authorship** | The author writes rules and processes, not fixed text. | Murray (24) |
| **Agency** | "The satisfying power to take meaningful action and see the results of our decisions and choices." | Murray (24) |
| **Altar problem** | Locally plausible, globally incoherent output. | AI Dungeon (23) |
| **Puppeting** | The narrator acts or speaks as the player. The most-cited agency failure. | AI Dungeon (23) |
| **Lenient narrator** | Nothing fails, so nothing has stakes. A narrator needs a rule under the prose. | AI Dungeon (23) |
| **Walls, not Police** | Constrain the shape of the space rather than policing content after the fact. | AI Dungeon (23) |

## Process

| Term | Meaning | Source |
|---|---|---|
| **Playcentric iterative loop** | goals → prototype → playtest → evaluate *against goals* → prioritise → change → retest. | Fullerton (26) |
| **Groups generate, individuals evaluate** | Group playtests surface possibilities; individual forms surface evaluations. Never test a social core alone. | 26 |
| **Watch behaviour, not opinions** | Behaviour > stated preference. Ask opinions individually *before* the group debrief. | 26 |
| **Golden set + replay** | For a non-deterministic narrator: log every call, keep canonical scenarios, replay after each change. | 26 |
| **Blind playtest** | Can the rules teach without the designer present? Board-game practice. | 26 |
