# Sound Design — Source Index

The 22 sources behind this skill, what each owns, and the honest caveats. The underlying
corpus (25 reports, ~1.3 MB) sits outside this repo.

**How to cite:** author + work. **Not** page numbers — most of these sources are print- or
lending-restricted, and page references were largely unverifiable across this corpus. Academic
APIs failed on nearly every run (Semantic Scholar and OpenAlex throughout; Wwise/Audiokinetic
docs 403-blocked; ACM DL Cloudflare-blocked), so treat academic negatives as *"not found," never
"proven absent."*

**How to read the numbers:** only the loudness figures are standardised. Ducking depths, bed
offsets, compression settings, layer counts and frequency splits are **practitioner
convention** — useful defaults, not measurements. The reports label which is which; keep that
distinction when advising.

---

## Tier 1 — The mix

| # | Source | Owns | Caveat |
|---|---|---|---|
| 01 | Michel Chion — *Audio-Vision* (1990/1994) | Added value, synchresis, vocentrism, rendered sound, the three listening modes | The field's entire vocabulary comes from one author and one translator (Gorbman) — a single point of failure. Essentialist, ahistorical, no empirical grounding. Two quote lists are edited excerpts — UNVERIFIED verbatim. |
| 02 | Walter Murch — *Dense Clarity — Clear Density* / *Womb Tone* (2005) | **The Law of Two-and-a-half** — the canon's only quantified mixing rule; the Encoded/Embodied spectrum; mix by dropping | "Law of the last thing" is UNVERIFIED (absent from the corpus). "Mixer = clarity / designer = density" is a paraphrase, not a quote. His left/right-brain evidence is dated. |
| 03 | Loudness standards — ITU-R BS.1770-5, EBU R128, ATSC A/85, platform docs | The measurement stack and the real delivery targets | Platform figures are often aggregator-sourced rather than platform-published; YouTube publishes no target; Netflix self-conflicts across its own pages. **No standard covers music-vs-voice balance** — the client's actual failure. |
| 04 | Practical mix craft for voice-led short-form | The ordered mix checklist; ducking and frequency separation; the phone check | Almost entirely practitioner convention, not standards. Bed offsets, ducking depths and compression figures are consensus rules of thumb. |
| 05 | Low end & small-speaker translation | Why the mix changes on a phone; the harmonic copy; room modes | The speaker roll-off figure is **contested** (200 Hz vs 400–600 Hz across sources) and must be measured per device. Several sections are rule of thumb, labelled as such. |
| 06 | Sound for marketing & social video | The commercial context — and the fact that it has no canon | **Genuine gap.** Sonic-branding evidence covers logos, not edits. Sound-off statistics are 2016–19 and platform-dependent. Music-vs-design is consensus, not experiment. |

## Tier 2 — Process & sound-to-picture

| # | Source | Owns | Caveat |
|---|---|---|---|
| 07 | David Sonnenschein — *Sound Design* (2001) | The only end-to-end method: script read-through → four categories → bipolarities → the sound map | Practitioner book, zero empirical apparatus. Pre-platform era: no loudness, ducking, phone or rights. Quotes verified only against unofficial OCR. |
| 08 | Randy Thom — *Designing a Movie for Sound* (1999) | Design sound **into** the film, not onto it; sound's problem is access, not craft | Three widely-repeated framings are paraphrases, not quotes ("fastest way to the heart", "same information twice is waste"). The text is dated (ADR, dubbing stage, 5.1). |
| 09 | Michel Chion — *The Voice in Cinema* (1982/1999) | The **acousmêtre**; its four powers; de-acousmatisation | Translation-dependent and frame-dependent (Chion requires a locus). Lacanian/gendered framing. No ethics layer. |
| 10 | Vanessa Ament — *The Foley Grail*; Ric Viers — *The Sound Effects Bible* | The four effect categories; the four-part layer model | Practitioner literature, not evidence (one peer-reviewed item). The layer model is a convergent heuristic, not a standard. |
| 11 | Claudia Gorbman — *Unheard Melodies* (1987) | **Inaudibility**; the diegetic/non-diegetic distinction | No facsimile consulted; page numbers and two quotes UNVERIFIED. Shares a lineage with Chion (Gorbman translated him) — the vocabulary is not independent. |

## Tier 3 — Interactive audio

| # | Source | Owns | Caveat |
|---|---|---|---|
| 12 | Karen Collins — *Game Sound* (2008) | Game audio as a field; adaptive vs interactive; loop fatigue | Most-cited work in the survey. Direct quotation is the weak point — the sample chapter PDF would not extract. The adaptive/interactive binary is contested in later literature. |
| 13 | Adaptive/interactive audio practice (Wwise, FMOD, practitioner) | Vertical vs horizontal; the transition taxonomy; the minimum viable recipe | Wwise's public library was **403-blocked**, so two claims are search-snippet only. Vendor docs describe their own products. One music vendor is vendor-adjacent. |
| 14 | Winifred Phillips — *A Composer's Guide to Game Music* (2014) | Music as a vocabulary of states; the film-composer crossover mistake | No page-level access (paywalled) — quotes only as reproduced in her own articles. Economics reconstructed from interviews; technology sections are 2014-era. |

## Tier 4 — The room

| # | Source | Owns | Caveat |
|---|---|---|---|
| 15 | Room acoustics & installed sound | **Treatment vs isolation**; structure-borne transmission; what actually stops bass; the limiter | Several numeric sources are retailer-adjacent. Local (Georgian) sound limits UNVERIFIED. Honest about what cheap fixes cannot achieve. |
| 16 | Venue music programming | Dayparts, energy curves, the spine, volume policy | **Evidence warning:** tempo→arousal is solid; tempo→**spend** is not (2024 meta-analysis global null; one field study found no bill-size difference). No experimental literature exists on dayparting or rotation cadence — those are craft constructs. |
| 17 | DJ set structure | The set arc; energy over tempo; phrase alignment | Core measurements come from a single vendor corpus, not peer review. Harmonic mixing is over-claimed: **78% of professional transitions are not in key.** |

## Tier 5 — Voice & narration

| # | Source | Owns | Caveat |
|---|---|---|---|
| 18 | Voice casting & direction for TTS (vendor docs + uncanny-valley research) | Cast-then-direct; text normalisation; the mismatch model of the uncanny valley | Vendor documentation is a snapshot of a fast-moving product, not neutral evidence. Several classic citations (Mori 1970, MUSHRA edition) remain UNVERIFIED. |
| 19 | Conversational latency & turn-taking | TTFA over total time; the real turn-taking baseline; endpointing and barge-in | **No primary study establishes "200–300 ms" as a perceptual threshold** — it is a composite of the human figure, ITU-T G.114's 400 ms, and vendor targets. Multi-speaker noisy endpointing is an evidence gap. |
| 20 | Sarah Kozloff — *Invisible Storytellers* (1988); Kaja Silverman — *The Acoustic Mirror* (1988) | The narrating voice as a **manufactured position**; manufactured authority; relay > anchorage > duplication | Kozloff pagination approximated; Silverman quoted second-hand (her PDF would not extract). Both are gender-thin and ethics-silent. The typology is a synthesis. |

## Tier 6 — Foundations & generative

| # | Source | Owns | Caveat |
|---|---|---|---|
| 21 | Beck & Grajeda; Weis & Belton; Altman; Sobchack | The scholarly canon of film-sound studies | **~85–90% is academic context, not practice.** Four ideas change a decision: recording-as-representation, point of audition, cinema-as-event, the diegetic seam. No Sobchack work on the materiality of the voice was locatable — flagged as a gap, not filled. |
| 22 | Generative audio production & licensing | What generators are good and bad at; the licensing landscape | **Not legal advice.** The landscape moves monthly: prompt-only authorship held unprotectable; major-label settlements Oct–Nov 2025; further suits pending as of the research date. Re-check before relying on any of it. |

---

## The two named gaps

1. **No canonical text exists for marketing/social-video sound or for venue/live audio.** The
   field's books assume either cinema (captive viewer, dedicated room) or games (interactive).
   Tiers 1 and 4 of this corpus are therefore synthesised from standards bodies, pro-audio
   practice and practitioner sources. When advising, say so rather than implying a scholarly
   basis that isn't there.

2. **No source covers a synthetic voice hosting a live group in a room.** The nearest neighbours
   are acousmêtre theory (film), narration theory (film) and conversational-latency research
   (one-to-one voice agents). Everything the skill says about a generated voice running a live
   group in a noisy bar is inference, and it is labelled as such in §1.7 of `SKILL.md`.
