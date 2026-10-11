---
name: game-design
description: >
  Game design — design and audit game loops, player motivation, social/party play, persistent
  worlds, and AI-driven narrative. Covers the loop stack (moment/core/session/meta), the return
  trigger, motivation frameworks (Self-Determination Theory, MDA, the 8 Kinds of Fun, flow,
  player typologies), social deduction and hidden-role design, in-room party-game architecture
  (one screen + many phones), live-ops cadence and the critical-mass problem, generated history
  and legibility, asynchronous/turn-based cadence, drama-manager and LLM-narrator design
  (structure vs surface, memory architecture, enumerated discretion), and playtesting method.
  Synthesized from 26 foundational sources. Use when designing or critiquing a game loop,
  deciding what makes a game fun or worth returning to, designing social/party/hidden-role play,
  planning a persistent world or live-ops cadence, designing an AI narrator or NPC memory,
  choosing a reward economy, or planning a playtest.
---

# Game Design

A working reference for designing games — weighted toward **the loop, motivation, social play,
persistent worlds, and AI-driven narrative** because those are the hard parts of the live
project this skill was built for — an LLM-narrated party game in development — and the parts
that general game-design advice handles worst.

**Before anything else, read §0.** It contains the finding that most design conversations need
and that most vocabulary lacks: retention is a property of the *seams between loops*, not of the
best loop.

---

## When to load this skill

- Designing or auditing a **game loop** — "what is the loop?", "why does this feel like a grind?"
- Deciding **what makes a game worth playing / returning to**
- Designing **social, party, or hidden-role** play for a room of real people
- Designing a **persistent world** — what survives between sessions, and what brings people back
- Planning **live-ops cadence**, events, or a between-session window
- Designing an **AI narrator, dungeon master, or NPC** — drama management, memory, discretion
- Designing a **reward economy** or progression
- **Onboarding** new players into an already-running game
- Planning a **playtest**

Don't load it for: art/asset production, engine or networking implementation, monetisation
modelling, or marketing. This is about the design of play, not its production.

---

## 0. The loop stack — read this first

*The central finding of the corpus, and a synthesis (not a single citation — label it as such).*

**Retention is a property of the seams between loops, not of the best loop.** (02)

```
MOMENT   ~sub-5s      the skill atom: what ONE interaction teaches
  └ CORE   sec–min    one pass must be independently satisfying and repeatable
      └ SESSION  min–2h   a framed container with a DESIGNED EXIT STATE
          └ META  days–months   everything that survives the session
```

### The three canonical seam failures

| Failure | Shape | Symptom |
|---|---|---|
| **Churn** | a loop with no meta payoff | Play is fun in the moment; nobody returns |
| **Obligation** | a meta loop with no satisfying core | People log in out of duty; play feels like work |
| **Exhaustion** | a core loop with no session frame | Binge then burnout; no designed stopping point |

### The two tests to apply to any design

1. **Cook's test:** *What repeats, and what does one pass teach?* If pass N+1 teaches nothing
   new and unlocks no higher skill atom, it is a **grind** — repetition with no downstream atom. (01)
2. **The seam test:** *What does one session bank outward into the meta loop?* If the answer is
   "nothing," you have churn regardless of how good the session is. (02)

### The return trigger

A trigger needs **time + claim + sender**. "Persistence" is a *property*, not a trigger. (02)

- An **appointment** (a scheduled session) carries hours, not weeks.
- A **social commitment addressed to a person, by name** is the load-bearing trigger for a
  low-frequency game.
- Back it with a **between-cycle action window** and a **non-punitive** consequence ladder.
  Invisible decay and withering read as punishment and convert a game into an obligation.
- **Ownership is the barrier to departure** (16) — the more of themselves players have put in,
  the harder it is to leave. This is a lever and an ethical line.

### Koster's clock

**Fun is the reward for mastering a pattern; boredom is a mastered pattern.** (09) Every loop has
a mastery horizon. When players reach it you must **add depth or retire the loop** — there is no
third option that is not grind.

---

## 1. Decision trees

### 1.1 Design or audit a core loop

1. **Name the verb.** What does the player *do*, in one verb, per pass? (09)
2. **Write the skill atom:** goal → action → simulation → feedback → updated model. (01)
3. **Ask Cook's test** (§0). State one concrete thing pass 1 teaches and pass 5 teaches.
4. **Check independent satisfaction:** is one pass satisfying alone, or only as part of a chain?
5. **Locate the loop in the stack** (§0) and name its neighbours. A core loop with no session
   frame will exhaust; without a meta payoff it will churn.
6. **Set the mastery horizon.** How many passes until the pattern is exhausted? What is added
   at that point?
7. **Check the reward shape against SDT** (§1.2). Rewards that feel controlling crowd out
   intrinsic motivation.

### 1.2 Design motivation (needs audit)

*Sources: 04 SDT, 07 Lazzaro, 08 Yee, 06 Kim, 05 Flow.*

1. **For each beat, name the need it serves:** autonomy / competence / relatedness. (04)
2. **Then ask the harder question: is any need being *frustrated*?** Satisfaction and
   frustration are separate pathways, not two ends of one scale. Frustration is worse than
   mere absence.
3. **Check the reward shape.** Expected tangible rewards for an already-interesting activity
   reliably *reduce* intrinsic motivation (pooled d ≈ −0.35 to −0.40 on high-interest tasks;
   both camps in the dispute agree on this cell). Prefer informational feedback over controlling
   rewards. (04)
4. **Run Lazzaro's diagnostic:** which of Hard / Easy / Serious / People Fun is each beat
   delivering — and which am I starving? The commonest failure is **Hard Fun only**. (07)
5. **Run the typology audit, not a labelling game:** whose motivations does this design reward,
   and who does it starve? (08) Use Yee/Quantic Foundry's dimensions (empirically derived) over
   Bartle's categories (descriptive, unaudited, n≈30, most-misused framework in the canon).
6. **Do not over-index on flow.** Its challenge–skill channel is weak-to-moderate empirically,
   and its "loss of self-consciousness" is *incompatible with deception* — which is the point of
   social deduction. Anxiety is a flow failure state and simultaneously a design product in
   hidden-role games. (05)
7. **Beware daily-cadence assumptions.** Habit-loop frameworks assume daily play. At weekly or
   fortnightly cadence their mechanics break — design the *appointment*, not the habit. (06)

### 1.3 Design the meta loop and return trigger (persistent games)

*Sources: 02, 16, 17, 18, 19.*

1. **Decide what survives the session.** Not "everything" — name the specific durable objects:
   state, standing, relationships, recorded events, possessions, debts.
2. **Design the exit state.** Every session should end in a state that *implies* the next one
   (a cliffhanger, an unresolved claim, a scheduled reveal). (02)
3. **Build the trigger.** Named, personal, time-bound (§0). Make it a *claim* on the player, not
   a notification.
4. **Make the world change on the real calendar** (16). If the world is identical after a week
   away, absence is free and the meta loop has no gravity.
5. **Never let the world feel empty** (16). Decide what a lone player finds when they arrive —
   and what the last session left behind for them. This is the single most-cited persistence rule.
6. **Feed the generator and build the memory.** You need both (17): something that makes history
   (events, conflict, stakes) and a system that *records and retrieves* it.
7. **Curation is the real work** (17). Generation is cheap. History that cannot be surfaced
   legibly may as well not exist — Dwarf Fortress produces ~1 GB of world history that its own
   interface cannot reveal; EVE's history is legible only to an elite. Budget effort for retrieval.
8. **Protect the population** (§1.4 in reference: critical mass). Critical mass is not a fixed
   number — it depends on mode, roles, skill spread and time of day. Small games beat it by
   **synchronisation, not scale**.

### 1.4 Design a social/party game for a room

*Sources: 12 Jackbox, 11 BotC, 13 Resistance, 14 De Koven, 15 Sicart.*

1. **Design the information split first**, not the theme. Who knows what, when, and how
   trustworthily? One asymmetry is usually the whole game. (13)
2. **Satisfy the Jack Principles:** maintain pacing (one task, limited choices, meaningful
   choices only, always know what to do, move on without stragglers); **create and maintain the
   illusion of awareness** (respond to actions, inactions, sequences, users' time and space);
   **shared control** (you author the choice-space, the player picks the path). (12)
3. **Remove friction to zero.** One shared screen + personal phones; no install; a room code;
   one action per beat; reading time budgeted. Friction kills a bar game. (12)
4. **Keep the context constitutive.** The room is part of the game, not a container for it
   (15). Use the space, the neighbours, the noise, the drink.
5. **Handle elimination** (§1.6).
6. **Give every player a public act.** Games where the quiet can hide are games where the quiet
   stop playing. (13)
7. **Put the climax last.** The best hidden-role games place the decisive moment *after* the
   "obvious" resolution, so the win can be inverted at the last second. (13)
8. **Design the spectating seat**, and expect a rolling entry — people arrive late in a bar.
   The re-entry layer must exist (see §1.7, Façade's deflect/reestablish pattern).
9. **Let the room own the game.** De Koven: authority must transfer from the rule-maker to the
   room, and the failure mode is drift into a *game community* where the rules decide who is
   good enough to play. *Change the game, not the people.* (14)

### 1.5 Design hidden roles and information

*Sources: 13, 11.*

1. **One asymmetry is the game.** Add a second only if it changes the endgame. (13)
2. **Decide the knowledge topology:** who knows whom; who knows what about the state; what is
   *knowable* versus merely *claimed*.
3. **Attack the "confirmed good" problem.** Any mechanic that can certify an honest player
   collapses the game. (11) Countermeasures found in the wild: false registration, hidden
   malfunction (a player who is *silently* wrong rather than lying), either/or information,
   assassination, alignment change.
4. **Make unreliability structural, not just deceptive.** "Whose inputs are unreliable" is a
   richer design space than "who is lying." (11)
5. **Forces commitment.** A rejection clock or a mandatory public act prevents endless hedging. (13)
6. **Resolve evidence parsimoniously** — e.g. "at least one of these N is X" — so information is
   real but never conclusive. (13)

### 1.6 Handle elimination and downtime

*Sources: 11 BotC, 13.*

1. **Death should be a state, not an exit.** The dead keep a voice, some agency (in Blood on the
   Clocktower, one vote for the remainder of the game), and social presence. (11)
2. **Check what elimination actually does** even when you remove it: Resistance has no
   elimination but *relocates* it socially — an outed traitor is cooperated with no more. (13)
3. **Design the downtime beat.** What is an eliminated or waiting player *doing*? In a bar: it
   should still be buying drinks and still be involved. (11, 18)

### 1.7 Design an AI narrator (drama manager + memory + discretion)

*Sources: 20 Façade, 21 Generative Agents, 22 Versu, 23 AI Dungeon, 24 Murray, 11 BotC.*

1. **Separate structure from surface — the single most important lesson.** Author the *logic*
   of the drama (state, beat selection, tension arc); generate the *language*. Structure decides
   what happens next; language decides how it sounds. (20)
2. **Give the narrator a drama manager:** discrete beats, one active at a time, sequenced
   against a designed tension arc, with the manager waking only at beat boundaries. (20)
3. **Give it a constrained role and, ideally, a fixed obsession.** A narrator with no defined
   job will manage the game, resolve tension early, and lose pacing. (20, 23)
4. **Enumerate its discretion.** The sharpest transferable rule in the corpus comes from Blood
   on the Clocktower's Storyteller: judgement is a **selection from supplied options, never
   fabrication.** An AI narrator may *choose* among licensed effects; it must not invent world
   state. (11)
5. **Build the memory architecture.** (21)
   - **STREAM** — an append-only prose log of everything that happened (observations, plans,
     reflections).
   - **RETRIEVE** — score each record by `recency + importance + relevance`; take the top k.
     Recency decays exponentially by *last access*; importance is judged at write time; relevance
     is against a *named* query, not the whole context.
   - **REFLECT** — when accumulated importance crosses a threshold, synthesise higher-level
     insights and write them back into the stream. This is what prevents amnesia.
6. **Never narrate the player's own action.** Puppeting is the most-cited agency failure. (23)
7. **Give the narrator a way to say no** — a rule underneath the prose. A narrator that cannot
   refuse has no stakes. (23)
8. **Model social state rather than scripted branches** where NPCs act (22): author *conditions
   and pools*, not sequences. Know the limit — simulated social meaning can still read as
   arbitrary; LLMs ease authoring burden but not the felt-meaning gap.
9. **Design the re-entry layer** for players who arrive late or missed a beat: gist points,
   repeat, reestablish, local deflect. (20)
10. **Decide moderation and privacy before launch.** The AI is reading what people say in a
    public room. This is a design constraint, not a policy afterthought — the AI Dungeon crisis
    was a categorisation failure, not a strictness failure: social-media moderation applied to
    private text, with no policy architecture decided in advance. **Walls, not Police.** (23)

### 1.8 Design the between-session window

*Sources: 19, 18, 02.*

1. **Recognise that the window is the gameplay.** In asynchronous social games the turn is not
   the game; the gap between turns is. (19)
2. **The turn boundary is two things at once** — the only moment that must be shared
   (synchronisation) and a deadline (commitment). (19)
3. **Turn length is the biggest dial you have** over presence, paranoia and story. Long turns
   create anticipation and story; they also tax real life and reproduce 2am-pressure failure
   modes. (19)
4. **Do not mechanise trust.** Unenforceable promises are the point — making betrayal
   impossible makes the game smaller. (19)
5. **Design the stall path.** What happens when someone misses a turn: no-move → civil disorder
   → substitution. (19)
6. **Do the narrative work at the boundary.** The reveal is the beat; the window is the setup. (19)
7. **Equalise presence advantage**, or the game rewards whoever has the most free time. (19)

### 1.9 Onboard a new player into a running world

*Sources: 06, 20, 17, 16.*

1. **Separate the journey stages** (06): Discovery → Onboarding → Habit-building → Mastery.
   What does each stage require *here*?
2. **Assume they arrive mid-story.** Provide a legible summary of the world *and* a private,
   personal hook — not a wiki. (17)
3. **Give them one public act early**, so they exist in the social graph before they need to
   have standing. (13)
4. **Do not gate on the history.** History should reward attention, not be a prerequisite. (17)
5. **Design the first-session exit state** to be as strong as a regular's. (02)

### 1.10 Playtest a social game

*Sources: 26, 03.*

1. **Playtesting is the instrument of the iterative loop**, not a feedback session:
   goals → prototype → playtest → evaluate *against goals* → prioritise → change → retest. (26)
2. **Never test a social game's core alone.** Groups *generate*; individuals *evaluate*. Do
   both, in that order. (26)
3. **Friends are a biased sample.** Include strangers. (26)
4. **Watch behaviour, not opinions.** Ask for opinions only in individual forms *before* the
   group debrief, and weight behaviour over both. (26)
5. **Do not teach, lead, or defend the game.** If you have to explain it, the design failed. (26)
6. **Test in the real room**, at the real time of day, with the real distractions. (26)
7. **Test the eliminated/waiting seat** specifically. (26)
8. **Set one question and three moments to watch before you start.** Everything else is noise. (26)
9. **For a non-deterministic (LLM) component:** log every model call, build a **golden set** of
   canonical scenarios, and **replay** them after every change. You cannot regression-test a
   narrator by memory. (26)
10. **Change one thing between tests.** Trust waves of evidence, not one table's evening. (26)

---

## 2. Failure-mode catalogue

The corpus's collected ways games die. Use as a pre-mortem.

**Loop failures** — grind (repetition with no downstream learning) (01) · pattern exhausted
(09) · core with no session frame → exhaustion (02) · session with no meta payoff → churn (02) ·
meta with no satisfying core → obligation (02) · reward crowding-out of intrinsic motivation (04) ·
Hard-Fun-only (07).

**Social/party failures** — onboarding friction (12) · the quiet player has nothing to do (13) ·
elimination removes a paying customer (11) · an outed traitor is socially dead (13) · the room
can't absorb late arrivals (20) · the group drifts into a *game community* that polices who is
good enough (14) · the game fights the venue instead of using it (15).

**Persistent-world failures** — the empty world: population falls → encounters thin → player
types decouple → newcomers bounce → population falls (16) · dead air between events (18) ·
the content treadmill (players consume faster than you produce) (16) · power creep (18) ·
server culture decays before the server dies (18) · cold start and the self-fulfilling "dead game" (18) ·
history generation without retrieval (17) · punishment-by-decay (02).

**AI-narrative failures** — the altar problem: locally plausible, globally incoherent (23) ·
context amnesia (23, 21) · repetition / loop collapse (23) · the lenient narrator (nothing fails) (23) ·
cannot say no (no rule under the prose) (23) · puppeting the player (23) · prose adjudication
with no cost (23) · generative moderation misfires (23) · policy retrofitted post-launch (23) ·
unbounded token cost (23) · combinatorial state explosion in simulated social worlds (22) ·
simulation that reads as arbitrary rather than meaningful (22).

---

## 3. When to break the default

Present the branch; do not split the difference by accident. (Full reasoning in
`references/glossary.md`.)

| Tension | Default | Break it when |
|---|---|---|
| **Flow vs deception** (05) | Keep players in the challenge–skill channel | In social deduction, anxiety *is* the product; self-monitoring is required |
| **Simulate vs script** (22) | Simulate social state; author conditions | Emergence reads as arbitrary; fall back to authored beats within a simulated frame |
| **Structure vs improvisation** (20, 11) | Drama manager sequences beats | The narrator improvises — but only within **enumerated** grants |
| **Rule-maker vs room** (14) | The designer owns the rules | The play community owns the game; let them bend it, or they leave |
| **Cadence vs pressure** (19) | Turn deadlines force commitment | Long deadlines tax real life; equalise presence before lengthening turns |
| **History vs legibility** (17) | More recorded history = a richer world | Volume destroys meaning; curation is the actual work |
| **Scale vs sync** (18) | Grow the population to survive | Small games beat critical mass by co-ordinating, not growing |
| **Reward vs motivation** (04) | Extrinsic rewards drive engagement | They crowd out intrinsic motivation on interesting tasks — prefer ceremony and standing |

---

## 4. Applying it: a live case

A live LLM-narrated social party game, run in-person at a bar in Tbilisi. The design doc's session
loop is well specified; the corpus's contribution is mostly at the *other three levels*.

| Open question | Recommendation from the corpus |
|---|---|
| **§23 — the fundamental reason to play** | It is a **social game with an audience and a memory**. Relatedness (04) + the play community (14) + People Fun (07) + pattern novelty (09). "The world remembers you" is a meta-loop *promise*; it needs a mechanism, not a slogan. |
| **The missing meta loop** | Add the **trigger** (a named, personal re-entry artifact between sessions, doubling as the remote/traveller hook) and the **seam** (each session banks one recorded world event that returns later as a consequence). Non-punitive ladder: absence must never wither the player. (02) |
| **§25 — reward economy** | SDT argues against extrinsic points. Use **standing over points**: titles, scars, KIA marks, monuments. Ceremony is the delivery mechanism. (04, 17) |
| **§26 — the Host** | It is a **drama manager** (20) + a **memory architecture** (21) + **enumerated discretion** (11). The Host may select from supplied effects; it must never fabricate world state. Give it a defined role and an obsession. |
| **§27 — legibility** | Generation is cheap; **curation is the work**. Monuments as retrieval interfaces. The absent player must still be *inside* the play community, not reading a log. (17, 14) |
| **§8 — elimination** | Death is a state, not an exit: the dead keep a voice and one vote. (11) |
| **§22 — Session #1 theme** | One asymmetry is the game; put the climax last. (13) |
| **Between sessions** | Make the fortnight the longest turn; the session is the *reveal* beat; design the stall path; do not mechanise trust. (19) |
| **Moderation & privacy** | **Launch-blocking.** The AI reads what people say in a public room. Decide the policy architecture before launch. Walls, not Police. (23) |
| **Session #0 (≈8 players)** | 8 sits at the *comfortable floor* of critical mass. Use the playtest method (§1.10); log every model call for replay. (18, 26) |
| **Scale-out / other cities** | Small worlds are communities, not populations. Multi-tenant worlds are still small at the point of play. Synchronise before you scale. (16, 18) |
| **Novelty / positioning** | The four-way intersection (live + in-room + group + AI host + persistent player memory) is **unclaimed in the world**, verified 2026-10-10 — but its components are each taken. Never lead with "world's first"; lead with **memory and legibility**, which is the defensible differentiator. See `references/sources.md`. |

---

## 5. Reference files

- **`references/glossary.md`** — the framework and principle glossary by domain, attributed to
  source. Load when you need to reason about *why*, or to cite a framework by name.
- **`references/sources.md`** — the 26 sources, what each owns, and the honest caveats
  (including which findings are `UNVERIFIED` and which are synthesis rather than citation).
  Also carries the **prior-art verification** of this corpus's named gap: the LLM-narrated live
group game is absent from the literature *and* unclaimed as a product, but its components are
  each shipping. Read it before making any novelty or "first" claim.

**Corpus (not included in this repo):** the full research corpus — 32 reports, ~1.5 MB —
with `CANON.md` (the ratified source list) and `SYNTHESIS-NOTES.md` (the evidence trail and the
domain-ownership matrix). Files `27a`–`27c` are the prior-art scans.
