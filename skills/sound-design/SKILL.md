---
name: sound-design
description: >
  Sound design — audio for screen, venues and interactive systems. Covers the mix (levels, EQ,
  compression, ducking, frequency separation, the low end), loudness standards and delivery
  targets, phone-speaker translation, sound-to-picture relationships (diegetic/non-diegetic,
  added value, synchresis, the acousmêtre), the sound-design process (spotting, sound maps,
  foley, effect layering, ambience), music for image, game and state-driven audio, venue
  acoustics and installed sound, music programming and DJ set structure, voice casting and
  direction for TTS, narration theory, conversational latency and turn-taking, and generative
  audio with its licensing risks. Use when mixing a video where music fights the voice, choosing
  levels or loudness targets, designing sound for a scene, building a sound effect, casting or
  directing a voice, designing an unseen narrator or AI host, tuning venue audio, programming
  music for a space, or assessing generative-audio rights.
---

# Sound Design

A working reference for designing, mixing and delivering audio — weighted toward **the mix**,
**sound-to-picture**, **voice**, and **the room**, because those are where this portfolio's work
actually lives and where generic audio advice fails.

**Start with §0.** It is the fix for the most common failure in short-form work — music fighting
the voice — and it contains the one quantified mixing rule in the canon.

---

## When to load this skill

- **Mixing** anything voice-led: music too loud under dialogue, effects too hot, levels wrong
- Choosing **loudness targets** or preparing a file for a platform or broadcast
- Deciding **what a sound should be doing** to the picture, not just what it should sound like
- **Planning sound for a piece** from the script or brief
- **Building a sound effect** from layers
- **Casting or directing a voice** — human or synthetic — including an unseen narrator
- Designing a **venue's sound**: acoustics, isolation, PA, music programming, volume policy
- Designing audio that must **respond to state** (a game, an installation, an interactive system)
- Tuning a **voice AI**: latency, turn-taking, interruption
- Assessing whether **generative audio** is safe to ship

Don't load it for: audio DSP/plugin engineering, codec or streaming implementation, licensing
negotiation, or music composition theory for its own sake.

---

## 0. The mix — start here

### The attention budget (Murch's Law of Two-and-a-half)

**At any moment an audience tracks roughly 2.5 simultaneous sound layers** before they congeal
into one indistinguishable mass. Three is the crossing point. Spread the layers across the
Encoded→Embodied spectrum and the ceiling roughly doubles to five. (02)

Two consequences that resolve most mix complaints:

1. **It is usually a budget problem, not a fader problem.** "The music is too loud and the SFX
   are too loud" normally means too many layers competing, not that the wrong things are loud.
2. **Mix by dropping, not by adding.** Decide what to remove *before* deciding how loud to make
   it. Murch calls this the shell game: continuous, deliberate sacrifice.

### The ordered mix checklist

For a 60–120 s voice-led video with music and effects. Order matters. (04)

1. **Calibrate monitoring** — mix at a known reference level; keep the master under −6 dBFS.
2. **Clean and level the voice alone** — in solo, no music.
3. **Voice chain:** high-pass ~80 Hz → cut mud/boxiness → compress 2:1–4:1, 5–20 ms attack,
   50–150 ms release → presence +1–3 dB at 2–4 kHz → de-ess. **No reverb** (it costs
   intelligibility in short-form).
4. **Anchor the voice's loudness alone** — everything else is built relative to it.
5. **Add music 15–20 dB under the voice** (24–31 dB if narration is continuous).
6. **Carve a midrange pocket** for the voice — roughly 3 dB around 2–4 kHz.
7. **Duck the music** (numbers below) rather than relying on the static level.
8. **Manually override on key lines** — automated ducking is a floor, not the final answer.
9. **Effects ~10 dB under the voice**, short, and off-centre in the field.
10. **Pan:** voice centred (mono, and keep everything under ~100–150 Hz mono).
11. **Low end:** add a saturated **harmonic copy** an octave up (150–200 Hz+) — the sub will not
    survive a phone speaker.
12. **Mono check** — collapse to mono and confirm nothing disappears.
13. **Phone check** — play it through an actual handset, quietly. Every word must land.
14. **Loudness-normalise last**, ≤ −1 dBTP, with only 1–2 dB of limiting.
15. **Re-listen** at the calibrated level.

### The numbers

| What | Value | Status |
|---|---|---|
| Duck music under voice | **6–10 dB**, ratio 4:1, attack 1–10 ms, **release 200–400 ms** | practitioner convention |
| Music bed under voice | 15–20 dB (24–31 dB under continuous narration) | practitioner convention |
| Voice high-pass | ~80 Hz | practitioner convention |
| Voice compression | 2:1–4:1, 5–20 ms attack, 50–150 ms release | practitioner convention |
| Sidechain high-pass | ~120 Hz (stop bass pumping the duck) | practitioner convention |
| Harmonic copy for small speakers | an octave up, **150–200 Hz+** | psychoacoustic |
| EBU R128 (European broadcast) | **−23 LUFS**, −1 dBTP | EBU R128 |
| ATSC A/85 (US broadcast, CALM Act) | **−24 LKFS** ±2, −2 dBTP | ATSC A/85 |
| Netflix | −27 LKFS ±2 dialog-gated, −2 dBTP | Netflix (self-conflicting across its own pages) |
| Spotify / YouTube / Amazon / Tidal | ~**−14 LUFS** | platform docs (changeable; YouTube publishes nothing) |
| Apple Music / Apple Podcasts | −16 | platform docs |

**Fix true peak first, then integrated loudness.** A true-peak overshoot distorts the loudness
reading and drives codec distortion downstream.

**Two rules that never change:** the measurement stack (ITU-R BS.1770) is stable; the platform
targets are not. Re-check them. And **no standard covers music-vs-voice balance** — that part is
your judgement, which is why the checklist exists.

---

## 1. Decision trees

### 1.1 Mix anything voice-led

Follow §0. Then diagnose:

- **Voice hard to hear at some words only** → masking, not level. Cut the competing band, don't
  raise the voice.
- **Music sounds right alone, wrong together** → duck it and carve the midrange pocket.
- **Fine on headphones, thin on a phone** → the low end has no harmonic support (§0 step 11).
- **Boomy on a laptop, thin on a phone** → you have real sub-bass that nothing reproduces; the
  mix is relying on content the listener cannot hear.
- **Everything fights at once** → count the layers. You are over the 2½ budget.

### 1.2 Plan sound for a piece from the script or brief

*Sources: 07 Sonnenschein, 08 Thom.*

1. **Read the script (or watch the cut) for sound specifically** — uninterrupted, at playback
   pace, pencil in hand.
2. **Mark four categories:** explicit sounds · environments · emotional clue words · transitions.
3. **Find the bipolarities** — the opposing emotional poles the piece moves between. Those become
   the sound map's curves.
4. **Draw the sound map:** a timeline with one curve per bipolarity, in different colours.
5. **Decide what each sound is *for*** — atmosphere, information, emotion, punctuation — rather
   than what it *is*.
6. **Cut.** Cross out everything that duplicates what the picture already says (see §1.4).
7. **Design it in early.** Thom's finding: sound's real problem is not making good sounds, it is
   being allowed to influence the other crafts before they foreclose the options. Get it into the
   room while mistakes are still cheap.

### 1.3 Build a sound effect

*Source: 10 foley & effect construction.*

1. **Decide the category:** *foley* (a body present, performed in sync), *hard effect* (a placed
   library element), *designed effect* (no real referent — must be invented), *ambience*
   (the continuous bed that glues cuts).
2. **Ask what it must *do*** — read on a phone, sell weight, feel like a place, land a joke.
3. **Build it in four layers**, sharing one attack/sustain/decay shape:
   - **sub** — the weight you feel
   - **body** — the midrange that identifies the thing
   - **detail** — the high-frequency specifics that sell it
   - **tail** — the decay/reverb that places it in a room
4. **Stop when it reads.** More layers buy nothing past the 2½ budget.
5. **Render the impression, not the reality** — the real sound is often the wrong sound. (01)
6. **Place it off-centre** and below the voice.

### 1.4 Write or judge narration

*Source: 20 narration theory, 09 Chion.*

1. **Ask what the narration *adds*** that the image cannot show. If the answer is "nothing," cut
   it — "say cow, see cow" is the failure.
2. **Rank the options: relay > anchorage > duplication.** Relay adds new information; anchorage
   pins down genuine ambiguity; duplication repeats the picture.
3. **Decide the narrator's position** on the two load-bearing axes: *can it be wrong?* and *does
   it have a locatable body?*
4. **Remember authority is manufactured** — granted in proportion to how far the voice is
   detached from a body. **Reliability is the only lever that converts an authority into a
   character.**
5. **If the narrator is unseen, treat it as an acousmêtre** (§1.5).

### 1.5 Design an unseen voice (the acousmêtre)

*Source: 09 Chion, The Voice in Cinema.*

1. **Give it a frame.** Chion's acousmêtre needs a locus — a screen, a speaker, a radio, a
   television. Without a frame it is just a disembodied voice, not a character.
2. **Establish it as continuous enough to be a character** — recurring, consistent, with a
   consistent relationship to the room.
3. **Use the four powers deliberately:** ubiquity, panopticism (it sees everywhere),
   omniscience, omnipotence. **Conceal their limits** — the power comes from what is not known.
4. **Know the cost of embodiment: de-acousmatisation destroys it.** "When the acousmêtre shows
   himself, the incarnation of his voice brings about his death." A reveal is a spend, once.
5. **The one documented exception is HAL** — a *machine* locus amplifies rather than dissipates
   the power. Partial or non-human embodiment preserves it; **a full human face destroys it.**
6. **Choose the voice's register:** an exterior authority voice (it addresses you) versus an
   I-voice (it identifies with you). They do different work.

### 1.6 Cast and direct a voice — including a synthetic one

*Sources: 18 TTS casting, 19 latency, 20 narration.*

1. **Cast by function, not by pleasantness.** Is this voice a narrator, an authority, a comic, a
   companion? Write a short character brief, then audition a slate of 6–12 candidates —
   including ones that are wrong on purpose and ones with the "wrong" accent.
2. **Audition with an identical script, on the real playback chain** (the actual phone, the
   actual PA), scored blind on whether it performs the function.
3. **Listen on a second day.** Voice preference is unstable.
4. **Test for spread:** run the same line five times and see how much it drifts. Cast for the
   range you need, not the sample.
5. **Direct through the text first** — punctuation, line breaks, an emphasised word do more than
   any slider. Then tags/instructions. Then settings.
6. **Freeze the identity knobs** (voice similarity/consistency) and move only the performance
   knobs. **Change one variable per retry.**
7. **Normalise the text before it reaches the model.** Numbers, dates, times, phone numbers,
   URLs, units, `St.`, roman numerals, and homographs are where raw text misreads — and it fails
   hardest on proper nouns.
8. **Watch the uncanny valley as a *mismatch* problem**, not a realism problem. Inconsistency and
   context-mismatch trigger it; more realism does not fix it.

### 1.7 Tune a voice conversation

*Source: 19 latency & turn-taking.*

1. **Target time-to-first-audio, not total response time.** Listeners consume speech as it
   plays, so TTFA governs the felt latency. Stream so the pipeline costs ~the slowest stage
   rather than the sum.
2. **Know the human baseline:** turn-taking has a **modal gap of 0 ms, mean +208 ms**
   (Stivers et al., PNAS 2009). Any perceptible delay is read as hesitation, not as network.
   (The familiar "200–300 ms threshold" is a composite, not a study finding.)
3. **Tune endpointing in both directions.** Too aggressive cuts the user off mid-sentence and
   destroys trust; too conservative produces robotic pauses.
4. **Allow barge-in.** Interruptibility is a trust behaviour.
5. **Add the human furniture** — backchannels and brief acknowledgements do latency-hiding work
   as well as rapport work. A voice with none of them sounds like a kiosk.
6. **Budget per stage and instrument it.** Measure; do not infer.
7. **In noise, expect this to be much harder.** A bar is a multi-speaker, reverberant
   environment — a different problem from one-to-one.

### 1.8 Fix a room's sound

*Source: 15 room acoustics & installed sound.*

1. **Separate the two problems before spending anything.** **Treatment** changes how the room
   sounds *inside*. **Isolation** changes how loud it is *outside* (the neighbours upstairs).
   They are different money. **"Absorbing isn't blocking."**
2. **Classify the transmission:** airborne or **structure-borne** (flanking). Get this wrong and
   everything downstream is wasted.
3. **Control the source first:** turn it down, move the sub out of the corner, off the shared
   wall, decouple it from the floor. This is nearly free and often sufficient.
4. **Seal penetrations** — a 1-inch hole costs roughly 10 STC.
5. **Decouple the structure** — resilient channels and separated leaves, not shared studs.
6. **Add mass** — useful but rapidly diminishing (on the order of ~6 dB).
7. **Treat the room for how it sounds**, not for the complaint.
8. **Do not buy foam, egg cartons, blankets or thin panels for a neighbour complaint.** They do
   nothing below ~2 kHz.
9. **Check the sound limiter early.** It cuts power after *sustained* level, so the whole night
   must be arranged underneath it — with the voice as the loudest sustained element, not the
   kick drum.

### 1.9 Programme music for a space

*Sources: 16 venue programming, 17 DJ set structure.*

1. **Programme by daypart and purpose, not by playlist.** Four buckets: daytime (background),
   threshold (signals the switch), peak (carries the room), close (shapes the exit). Each is a
   *purpose*, not a genre.
2. **Keep one shared "spine"** of familiar tracks that appears in every daypart — that is what
   makes the room sound like itself across a week.
3. **Programme an energy curve, not a track list.** Warm-up → build → peak → close. Energy
   carries the arc; **tempo does not** (median published BPM is flat at 126 across a set).
4. **Respect the phrase.** Music is built in 8/16/32-bar phrases; put transitions on boundaries.
5. **Move tempo gently:** ~±3% is comfortable, ~±6% is the practical limit of a pitch fader;
   beyond that, cut or filter instead of blending.
6. **Do not over-trust harmonic mixing.** It is real but weak — **78% of professional transitions
   are not in key.**
7. **Never stack competing vocals** — one voice at a time in a room.
8. **Set volume from room state, not the clock.** Use the far-table conversation test: if they
   have to raise their voices, it is too loud. Move in ≤3 dB steps, re-check after 15 minutes,
   and give one named person ownership per shift.
9. **Do not justify music spend with the tempo→spend myth.** Tempo→arousal is supported;
   tempo→spend is not (a 2024 meta-analysis reports a global null). Sell music on atmosphere,
   dwell and identity, which are defensible.

### 1.10 Design audio that responds to state

*Sources: 13 adaptive audio, 12 Collins, 14 Phillips.*

1. **Decide who controls order, timing, duration and occurrence.** In linear media you do; in an
   interactive system the player/system does. Every other decision follows.
2. **Classify the trigger:** *adaptive* (driven by state) versus *interactive* (driven by direct
   input).
3. **Prefer vertical layering for a first build** — adding and removing layers of one composition
   has no seam to hide. Horizontal re-sequencing needs transition craft.
4. **If you go horizontal, compose the transition.** Options in rising order of cost: cut ·
   crossfade (the criticised default) · segue · stinger (an in-key event phrase) · a bridge
   segment written as a joint · branching.
5. **Design against loop fatigue.** The same asset will be heard hundreds of times. Mitigations:
   write randomness into the composition, use variation pools, make the base layer minimal so
   layering does the work, align to phrases, and use **silence** deliberately.
6. **Treat music as a vocabulary of states, not a narrative arc.** A fixed build/climax/resolve
   loops badly and cannot be recombined — the classic crossover mistake.
7. **Minimum viable adaptive audio:** one composition in three stems, two or three states, fades
   rather than crossfades, one bar-aligned loop, one in-key stinger, and four buses
   (Music / SFX / Voice / Master) with a music duck whenever voice plays.

### 1.11 Decide whether generative audio is safe to ship

*Source: 22 generative audio production. **This is not legal advice.***

1. **Use it where it is strong:** temp/scratch cues, beds, ambience, drones, risers, one-shot
   effects, era pastiche, and cheap ideation.
2. **Do not use it where it is weak:** long-form structure, phrase-level sync, anything that must
   be reproduced identically, consistent vocals, or **stems you need to edit** — some generators
   regenerate stems rather than slicing the mix, so a generated track is effectively indivisible.
3. **Impose coherence yourself.** You will not get the same sound twice; consistency must come
   from your own processing and mix chain.
4. **Separate the two legal questions:** what the platform's terms of service permit, and what
   copyright actually attaches. They are not the same, and terms of service ≠ copyright.
5. **Know the current position:** prompt-only authorship has been held unprotectable
   (*Thaler v. Perlmutter*, D.C. Cir. 2025). Several major-label settlements landed in Oct–Nov
   2025; further suits were pending as of the research date. Some platforms' terms now restrict
   or ban downloads. **This landscape moves monthly — re-check it.**
6. **Do not build a brand's core identity on generated audio.** Use it for texture; own your
   identity with something you can protect.
7. **Run the risk checklist before shipping:** terms tier and revision date · commercial-use
   mechanism · download terms · copyright position · uniqueness · training provenance ·
   watermarking · destination platform's rules · disclosure obligations · voice consent ·
   client IP assignment · insurance · reversibility · and a records trail.

---

## 2. Failure-mode catalogue

Use as a pre-mortem.

**Mix failures** — over the 2½ attention budget (02) · music masking the voice instead of being
ducked (04) · voice drowned by continuous narration-level music · reverb on a short-form voice ·
sub-bass with no harmonic support, inaudible on a phone (05) · mixing by adding rather than
dropping (02) · loudness-normalising as a substitute for balance (03) · fixing the wrong failure
(raising the voice instead of cutting the mask).

**Sound-to-picture failures** — duplicating what the picture already says (20) · an acousmêtre
given a face and thereby killed (09) · a narrator with no defined position, therefore no
character · sound designed too late to change anything upstream (08) · unplanned sound, chosen
from a library rather than derived from the piece (07).

**Process failures** — a single effect used where a body's presence is needed (10) · an effect
with no `tail`, so it sits outside the room · ambience missing, so cuts are audible · too many
layers, so nothing reads.

**Venue failures** — spending on treatment to fix an isolation complaint (15) · foam where mass
and decoupling were needed · the limiter tripping at peak, forcing the mix to be re-arranged
after the fact · one playlist for all dayparts (16) · programming for tempo and ignoring energy
(17) · no named owner for volume, so it drifts upward all night (16).

**Voice failures** — a synthetic voice selected rather than cast (18) · identity knobs moved
alongside performance knobs, so the voice drifts · raw text misread (numbers, dates, homographs) ·
perceptible latency at the start of speech (19) · endpointing that cuts the user off · a voice
with no backchannels, reading as a kiosk · uncanny-valley triggered by inconsistency, and then
"fixed" by adding realism.

**Generative failures** — un-editable output used where editability was needed (22) · assuming
terms of service equal copyright · style drift across a project · building brand identity on
output that cannot be owned · shipping without a licensing risk review.

---

## 3. When to break the default

| Tension | Default | Break it when |
|---|---|---|
| **Fidelity vs impression** (01, 10) | Record and reproduce the real sound | The real sound reads wrong — render the impression the audience expects |
| **Audibility** (11) | Music should be felt, not heard | Short-form and venues need music *heard* as identity; inaudibility is a cinema convention |
| **Structure vs emergence** (08, 07) | Plan sound from the script | Discovery beats intention — the right sound is often found in the edit |
| **Fewer layers vs more** (02, 04) | Respect the 2½ budget | A dense, deliberate wash is the intention — then make it one *thing*, not five |
| **Latency vs naturalness** (19) | Respond as fast as possible | Speaking before the thought is complete reads as interruption — a short pause beats a wrong sentence |
| **Synthetic vs performed voice** (18, 09) | TTS is castable and directable | Presence and body are the point — then no synthesis substitutes for a performance |
| **Generated vs authored** (22, 14) | Fast, cheap texture | It must be owned, defended, repeated or edited — then it must be made |

---

## 4. Applying it to the four live fronts

**1. Marketing/social video — the active pain.** Run §0's checklist. The complaint ("music
louder than the voice, effects too loud") is a layer-budget problem as much as a level problem:
drop something before turning something down. Deliver at the platform target, check on an actual
phone, and licence the music **before** locking the edit — temp music biases the cut. (04, 03,
05, 06)

**2. Live venue.** Separate treatment from isolation and spend on the right one. Bass is
structure-borne: control the source, decouple, and seal penetrations before buying anything.
Programme four dayparts plus a shared spine, set volume by room state with one owner per shift,
and do not justify the spend with the tempo→spend myth. (15, 16, 17)

**3. The voice host.** The Host is an **acousmêtre**: keep it framed in the
television and never give it a full human face — that is de-acousmatisation, and it destroys the
power; partial machine embodiment preserves it (HAL). Its authority is manufactured by detachment
from a body, and **reliability is the only lever that turns it into a character**. Give it
narration discipline (relay, don't duplicate) and conversational discipline (TTFA, endpointing,
barge-in). (09, 20, 19, 18)

**4. Voice AI agents.** Cast, then direct. Write performance into the text,
freeze identity knobs, change one thing per retry. Measure time-to-first-audio, not total
response time, and expect the bar to be far harder than a one-to-one call. (18, 19)

---

## 5. Reference files

- **`references/glossary.md`** — the concepts and vocabulary by domain, attributed to source.
  Load when you need to reason about *why*, or to name a technique properly.
- **`references/sources.md`** — the 22 sources, what each owns, and the honest caveats —
  including which findings are `UNVERIFIED`, which "numbers" are convention rather than
  standard, and the two genuine gaps in the literature.

**Corpus (not included in this repo):** the full research corpus — 25 reports, ~1.3 MB —
with `SYNTHESIS-NOTES.md` holding the evidence trail and the domain matrix.
