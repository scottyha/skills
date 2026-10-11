# Sound Design — Glossary & Concepts

Attributed by author and work. Page numbers are deliberately absent: most of these sources are
print- or lending-restricted, and page references were largely unverifiable across this corpus.
`[UNVERIFIED]` marks claims the research could not confirm; `[convention]` marks practitioner
rule of thumb rather than standard or measurement; `[synthesis]` marks a construction of this
corpus rather than any single source.

---

## The mix

| Term | Meaning | Source |
|---|---|---|
| **Law of Two-and-a-half** | At any moment an audience tracks ~2.5 simultaneous sound layers from one region of the spectrum before they congeal; three is the crossing point. Spread across the spectrum, ~5. | Murch, *Dense Clarity — Clear Density* (02) |
| **Encoded ↔ Embodied spectrum** | Sounds that carry meaning by convention vs sounds that affect us physically. Layers of different kinds interfere less. | Murch (02) |
| **Clarity vs Density** | The mixer's job is clarity (what is understood); the designer's job is density (what is present). Managing the tension is the craft. | Murch (02) [synthesis of phrasing] |
| **The shell game** | Continuous, deliberate sacrifice — something is always being dropped so that something else can be heard. | Murch (02) |
| **Conceptual resonance** | A sound should resonate with the meaning of the moment, not merely match the picture. | Murch (02) |
| **Rendered vs reproduced sound** | Sound must *render* the impression the audience expects, not reproduce the real sound. | Chion (01) |
| **Ducking / sidechain** | Attenuating music automatically when the voice plays. 6–10 dB, 4:1, release 200–400 ms. | 04 [convention] |
| **Midrange pocket** | Carving space in the music around 2–4 kHz so the voice reads. | 04 [convention] |
| **Harmonic copy** | Duplicating/synthesising a bass element an octave up (150–200 Hz+) so the low end is perceived on small speakers. | 05 (missing fundamental, Terhardt) |
| **Missing fundamental** | The brain reconstructs a low pitch from its harmonics — the mechanism that makes the harmonic copy work. | 05 |
| **True peak (dBTP)** | Inter-sample peak; fix it before chasing integrated loudness. | 03 |
| **Integrated / short-term / momentary loudness** | The gated whole-programme measure vs rolling windows. Delivery targets use integrated. | 03 |

## Loudness & delivery

| Term | Meaning | Source |
|---|---|---|
| **ITU-R BS.1770** | The loudness measurement algorithm itself (gated, K-weighted). Stable; not a target. | ITU (03) |
| **EBU R128** | −23 LUFS, −1 dBTP (European broadcast). | EBU (03) |
| **ATSC A/85 / CALM Act** | −24 LKFS ±2, −2 dBTP (US broadcast; mandated). | ATSC, 47 CFR §76.607 (03) |
| **LUFS vs LKFS** | Effectively the same unit; the difference is naming, not measurement. | 03 |
| **Platform normalisation** | Platforms turn loud masters *down*; mastering louder therefore buys nothing. ~−14 LUFS typical. | 03 (changeable) |
| **Dialog-gated loudness** | Measuring loudness only across dialogue — used by Netflix. | Netflix (03) |

## Sound to picture

| Term | Meaning | Source |
|---|---|---|
| **Added value** | Sound enriches an image so thoroughly that the meaning seems already to be in the image. | Chion (01) |
| **Synchresis** | The involuntary perceptual weld of a sound to an image, even an arbitrary pairing. The basis of all sound design. | Chion (01) |
| **Vococentrism** | Cinema privileges the voice above all other sound. | Chion (01) |
| **Three listening modes** | Causal (what made it), semantic (what code it is), reduced (its qualities as sound). | Chion (01) |
| **Acousmêtre** | The unseen voice-character; holds ubiquity, panopticism, omniscience, omnipotence. | Chion, *The Voice in Cinema* (09) |
| **De-acousmatisation** | Attaching the unseen voice to a body — which destroys the power. "When the acousmêtre shows himself, the incarnation of his voice brings about his death." | Chion (09) |
| **Empathetic / anempathetic sound** | Music that matches the scene's feeling vs music that indifferently continues through it. | Chion (01) |
| **Audiovisual scene** | Sound's power to temporalis an image — making us anticipate or recall. | Chion (01) |
| **Inaudibility** | Classical film music is *designed* to be felt but not consciously heard; subordination to dialogue is a constructed effect, not an absence. | Gorbman (11) |
| **Diegetic / non-diegetic** | Music or sound inside vs outside the story world — with a contested "fantastical gap" between. | Gorbman (11) |
| **Anchorage / relay / duplication** | Narration that pins down ambiguity / adds what the image cannot show / merely repeats the image. | Barthes via 20 |
| **Manufactured authority** | A narrator's authority is constructed by genre and detachment from a body — not intrinsic. Reliability is the only lever that makes it a character. | Kozloff (20) |

## Process

| Term | Meaning | Source |
|---|---|---|
| **Spotting** | Watching the piece specifically for sound cues, before designing anything. | 07 |
| **Sound map** | A timeline with one curve per bipolarity (opposing emotional poles) — the sound plan as a picture. | Sonnenschein (07) |
| **Bipolarities** | The opposing emotional poles a piece moves between; the axes of the sound map. | 07 |
| **Design for sound, not with sound** | Sound's real problem is being invited in before the other crafts foreclose the options. | Thom (08) |
| **Starve the eye** | Give sound something to do: if the picture supplies everything, sound is decoration. | Thom (08) |
| **Sound as attention management** | Sound's job is directing attention, not fidelity — if the character isn't listening, neither is the audience. | Thom (08) |

## Foley & effects

| Term | Meaning | Source |
|---|---|---|
| **Foley** | Sound performed in sync to picture, continuous with a body (footsteps, props, cloth). Supplies *presence*. | Ament (10) |
| **Hard effects** | Discrete, placed library elements. Supplies *emphasis*. | Viers (10) |
| **Designed effects** | Built from layers for things with no real referent. Supplies *invention*. | 10 |
| **Ambience / room tone / atmos** | The continuous bed; the glue that makes cuts invisible. | 10 |
| **Four-part layer model** | Any designed effect = **sub** (weight) · **body** (identity) · **detail** (specifics) · **tail** (placement), sharing one attack/decay shape. | 10 [convergent heuristic] |

## Game & interactive audio

| Term | Meaning | Source |
|---|---|---|
| **Dynamic audio** | The umbrella: any audio that changes with game state or input. | Collins (12) |
| **Adaptive vs interactive** | State-driven (adaptive) vs direct-input-driven (interactive). Contested in later literature. | Collins (12) |
| **Vertical layering** | Adding/removing simultaneously playing layers of one composition. No seam to hide — the safe default. | 13 |
| **Horizontal re-sequencing** | Moving between composed segments; needs transition craft. | 13 |
| **Transition types** | cut · crossfade (the criticised default) · segue · stinger · bridge segment · branching. | 13 |
| **Stinger** | A short in-key musical event marking a state change. | 13 |
| **Loop fatigue** | Assets authored for one hearing, heard hundreds of times. The organising problem of game audio. | Collins (12) |
| **Music as states, not arc** | Game music is a vocabulary of states; a fixed build/climax/resolve loops badly and cannot be recombined. | Phillips (14) |
| **Bus architecture** | Music / SFX / Voice / Master as separate paths, so voice can duck the rest. | 13 |

## Venue & acoustics

| Term | Meaning | Source |
|---|---|---|
| **Treatment vs isolation** | How the room sounds *inside* vs how loud it is *outside*. Different money. "Absorbing isn't blocking." | 15 |
| **Structure-borne vs airborne** | Transmission through the building structure vs through the air. Determines what actually works. | 15 |
| **Flanking paths** | Indirect structural routes that bypass a treated partition and undo it. | 15 |
| **Room modes** | Standing waves set by room dimensions; small rooms are lumpy in the low end. | 15 |
| **Sound limiter** | Cuts power after *sustained* level — so the whole night must be arranged underneath it. | 15 |
| **Dayparting** | Programming music differently for daytime / threshold / peak / close. | 16 |
| **Energy curve** | The designed arc of a night, programmed as energy rather than tempo. | 16, 17 |
| **Spine** | A shared set of familiar tracks appearing in every daypart — the room's musical identity. | 16 [synthesis] |
| **Far-table conversation test** | If the far table has to raise their voices, it is too loud. | 16 |
| **Phrase alignment** | Music is built in 8/16/32-bar phrases; transitions belong on boundaries. | 17 |

## Voice & TTS

| Term | Meaning | Source |
|---|---|---|
| **Cast, then direct** | A synthetic voice is cast by function and directed, not merely selected. | 18 |
| **Identity vs performance knobs** | Freeze consistency/similarity; move style, stability, speed. Change one per retry. | 18 |
| **Text normalisation** | Pre-processing text so numbers, dates, units, homographs and proper nouns read correctly. | 18 |
| **Uncanny valley (voice)** | Triggered by *mismatch/inconsistency*, not by realism level. | 18 |
| **Time-to-first-audio (TTFA)** | The latency that governs felt responsiveness — not total response time. | 19 |
| **Turn-taking gap** | Human baseline: modal 0 ms, mean +208 ms (Stivers et al., PNAS 2009). | 19 |
| **Endpointing** | Deciding when the user has finished; fails by cutting off or by pausing too long. | 19 |
| **Barge-in** | Allowing the user to interrupt; a trust behaviour. | 19 |
| **Backchannels** | Brief acknowledgements ("mm-hm"); rapport *and* latency-hiding. | 19 |

## Generative audio

| Term | Meaning | Source |
|---|---|---|
| **ToS ≠ copyright** | Platform terms describe what you may do; they do not determine what copyright attaches. | 22 |
| **Prompt-only authorship** | Held unprotectable (*Thaler v. Perlmutter*, D.C. Cir. 2025). | 22 |
| **Stem regeneration** | Some generators regenerate stems rather than slicing the mix — so output is effectively un-editable. | 22 |
| **Imposed coherence** | Consistency across a project must come from your own processing chain, not the generator. | 22 |
