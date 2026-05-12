# Vocal Style Coordinate Instructions

Use this resource to identify the desired vocal style as a coordinate in a vocal feature space. A strong Suno vocal direction is not just "male singer" or "soulful voice"; it is a compact bundle of range, tessitura, weight, timbre, phonation, register behavior, vibrato, ornamentation, diction, rhythmic feel, emotional stance, production texture, and section-by-section movement.

For extended examples, read `vocal-routing-index.md` first. It routes ordinary vocal prompt work to compact resources and escalates only named profiles, comparison tests, prompt tables, and rubrics to `vocal-identity-library.md`. For the raw classical/choral/Fach terminology source, read `classical-vocal-classification-source.md`.

## Coordinate Workflow

1. Extract explicit user constraints: singer identity, genre, emotional tone, language, era, and any do-not-want qualities.
2. Fill the core coordinate dimensions: vocal role, approximate range, tessitura, vocal weight, timbre, phonation, register behavior, vibrato, ornamentation, articulation, diction/accent, rhythmic feel, genre gravity, emotional stance, dynamic shape, production texture, movement behavior.
3. Choose 5-8 dimensions to express in the Suno style prompt. Prioritize the dimensions that most affect the requested song.
4. Resolve contradictions. For example, "breathy intimate stadium belt" needs a sectional split: breathy verse, open-throat belted chorus.
5. Put the vocal coordinate early in the style prompt when voice is central.

## Coordinate Template

```text
[vocal_role], [approximate_range/tessitura], [vocal_weight], [timbre], [phonation], [register_behavior], [vibrato/ornamentation], [articulation/diction], [rhythmic_feel], [emotional_stance], [production_texture], [movement_behavior]
```

Compact Suno style phrase:

```text
smoky alto, low-set tessitura, breathy close-mic phonation, delayed vibrato, soft consonants, behind-the-beat phrasing, haunted confessional tone
```

## Dimension Values

### Vocal Role

Defines pitch identity, arrangement role, and cultural expectation.

Use three levels of specificity:

- **choral category**: soprano, alto, tenor, bass; practical ensemble parts and SATB layout.
- **expanded classical voice type**: soprano, mezzo-soprano, contralto, countertenor, tenor, baritone, bass-baritone, bass.
- **Fach/subtype**: lyric soprano, dramatic mezzo-soprano, coloratura mezzo, Heldentenor, basso profundo; use when classical color, agility, weight, projection, or role suitability matters.

- **soprano**: high female-range or high-set voice; bright lift, clarity, bell-like hooks.
- **mezzo**: middle female-range voice; flexible pop, theater, rock, and soul territory.
- **alto**: lower female-range voice; warmth, intimacy, grounded phrasing.
- **contralto**: very low female-range voice; dark color, rare depth, close-mic gravity.
- **tenor**: higher male-range voice; pop, rock, R&B, and folk lead flexibility.
- **baritone**: mid-low male-range voice; authority, narrative weight, warmth.
- **bass**: very low male-range voice; gravity, chant, drone, ceremonial impact.
- **bass-baritone**: bass-like weight with baritone upper access; authority, villainy, ceremony, dramatic flexibility.
- **countertenor**: high male/head-voice-centered role; ethereal, chamber, art-pop, sacred textures.
- **ensemble lead**: lead voice designed to interact with backing singers.
- **chant leader**: rhythmic or devotional lead built for repetition and response.
- **shouter**: speech-heightened, punk, blues, gospel, or rock force role.
- **crooner**: smooth, intimate, legato lead with close phrasing.
- **narrator**: speech-like lead that prioritizes intelligibility and story.

### Classical Fach and Subtype

Use this dimension when the prompt benefits from classical, operatic, choral, theater, or highly specific vocal capability language.

- **coloratura soprano**: very high extension, rapid runs, trills, leaps, lightness, brilliance.
- **lyric soprano**: warm melodic soprano, smooth legato, clear upper register, moderate weight.
- **dramatic soprano**: large powerful soprano, stamina, darker timbre, strong projection over heavy orchestration.
- **spinto soprano**: lyric beauty with bursts of power; can cut through fuller orchestration without full dramatic weight.
- **soubrette soprano**: light bright soprano, excellent diction, charm, agility, youthful or comic energy.
- **lyric mezzo-soprano**: warm middle register, flexibility, comfortable upper-middle tessitura, less weight.
- **dramatic mezzo-soprano**: dark color, strong low and middle registers, stamina, commanding thrust.
- **coloratura mezzo-soprano**: agile mezzo, fast runs, clean florid passages, strong lower-middle register.
- **lyric tenor**: clear upper register, sweetness, legato, romantic or youthful tone.
- **dramatic tenor / Heldentenor**: heavy heroic tenor, stamina, darker timbre, strong upper register, orchestral carrying power.
- **basso profundo**: exceptionally low bass, deep resonance, dark timbre, strong low tessitura.
- **leggiero quality**: light, flexible, agile; useful for fast passages and lighter roles.

Fach is not just range. It combines range, tessitura, timbre, vocal weight, agility, projection, stamina, and repertoire/role suitability.

### Approximate Range

Defines pitch span and the physical impression of the voice.

Range is the full span a voice can produce. Core range is the reliable central span. Extension is the outer usable edge. For prompt writing, tessitura and core range are usually more important than the most extreme notes.

- **low**: emphasizes depth, intimacy, weight, or menace.
- **mid**: stable and flexible; good for broad pop and storytelling.
- **high**: bright, exposed, energetic, ecstatic, or fragile.
- **wide**: supports dramatic leaps, ad-libs, and climactic expansion.
- **narrow**: feels restrained, conversational, chant-like, or character-driven.
- **note-band examples**: `G2-D4`, `E3-B4`, `A3-F5`, `C3-G5`; use only when useful.
- **upper extension**: high notes beyond the main tessitura; useful for soprano, tenor, coloratura, and climactic ad-libs.
- **lower extension**: low notes beyond the main tessitura; useful for contralto, bass, basso profundo, and dark spoken-sung material.

Use octave notation such as `C4` for middle C when precise range matters.

### Tessitura

Defines where the voice sits most of the time, not its full possible range.

- **low-set**: verses feel grounded, dark, intimate, or heavy.
- **middle-set**: natural speech-song balance; versatile and stable.
- **high-set**: bright presence, youthful lift, chorus sparkle.
- **flexible**: moves between registers without one dominant center.
- **octave-jumping**: dramatic leaps and contrast, useful for art-pop, theater, or experimental styles.
- **passaggio-aware**: emphasizes smooth or expressive register transitions; useful for classical, theater, and technically detailed voice prompts.

### Vocal Weight

Defines density and carrying power.

- **featherweight**: airy, delicate, vulnerable, nimble.
- **light**: agile, clean, pop-friendly.
- **lyric**: clear and melodic with moderate presence.
- **medium**: balanced, believable across band and electronic arrangements.
- **heavy**: dense, powerful, forceful; useful for rock, gospel, theater, metal.
- **dramatic**: large, staged, operatic or theatrical scale.
- **gravel-heavy**: weight comes from rasp, grit, distortion, or roughness.
- **spinto**: lyric baseline with extra thrust for climaxes.
- **soloistic**: stands out as an individual line over accompaniment.
- **blend-oriented**: designed to merge with a choir or harmony section rather than dominate.

### Timbre Color

Defines the perceived color of the voice.

- **bright**: forward, clear, energetic.
- **dark**: low-color, serious, intimate, dramatic.
- **smoky**: soft grit, lounge, blues, late-night intimacy.
- **metallic**: cutting, brilliant, intense.
- **glassy**: clean, high-sheen, crystalline.
- **woody**: organic, folk, acoustic, earthy.
- **nasal**: forward, twangy, punk, country, characterful.
- **airy**: breath-laced, light, ethereal.
- **velvet**: smooth, dark, rounded.
- **copper**: warm but bright, brassy edge.
- **steel**: hard, focused, high-impact.
- **honeyed**: warm, sweet, gospel/soul-friendly.
- **raspy/gritty**: rough texture, rock, blues, punk, emotional wear.

### Phonation

Defines how the vocal folds are used and how the sound starts.

- **breathy**: audible air, intimacy, fragility.
- **clear/clean**: stable tone, intelligibility, polish.
- **pressed**: compressed, intense, urgent; can become harsh.
- **speech-like**: close to speaking, direct, narrative.
- **aspirate**: soft attacks with air before tone.
- **creaky**: low fry-like onset, intimate or edgy.
- **growled**: controlled roughness, blues, rock, metal, theatrical menace.
- **distorted**: heavier saturation or scream-adjacent edge.
- **balanced onset**: clean coordinated note beginning; useful for classical or polished vocal prompts.
- **glottal onset**: firm attack; useful for pop punctuation, theater, punk, or rhythmic clarity.
- **modal voice**: ordinary speech/singing register; useful for grounded adult leads.

### Register Behavior

Defines how the voice uses chest, mix, head voice, falsetto, and breaks.

- **chest-dominant**: grounded, direct, speech-rooted.
- **mix-dominant**: modern pop belt and flexible chorus lift.
- **head-dominant**: light, high, floating, classical or ethereal.
- **falsetto-forward**: airy high register, electronic/R&B/pop contrast.
- **break-embracing**: audible cracks or flips used expressively.
- **seamless**: smooth transitions with little register contrast.
- **chesty mix belt**: powerful but controlled high chorus delivery.
- **modal-centered**: remains in ordinary singing coordination with few register effects.
- **passaggio-exposed**: lets transition zones color the performance; useful for drama or vulnerability.

### Projection Style

Defines the apparent performance scale.

- **close-mic intimate**: private, dry, near the listener.
- **conversational**: natural speech-song presence.
- **chamber**: refined, small-room, art-song or acoustic.
- **open-throat**: resonant, lifted, strong without strain.
- **theatrical**: staged, clear diction, large gestures.
- **stadium**: big, wide, anthem-scale.
- **operatic projection**: resonance and singer's-formant-like carrying power over dense accompaniment.
- **choral blend**: restrained individual edge so the voice merges with an ensemble.

### Vibrato

Defines pitch movement on sustained notes.

- **straight-tone**: little vibrato; pure, modern, choral, punk, electronic, or restrained.
- **narrow fast**: shimmer, energy, R&B/pop detail.
- **wide slow**: dramatic, vintage, theatrical, gospel, torch.
- **delayed**: starts straight then blooms; useful for controlled emotion.
- **tremolo-like**: quick flutter, nervous or aged color.
- **ornamental**: vibrato used as flourish.
- **dramatic**: pronounced vibrato as a major style marker.

### Ornamentation

Defines decorative pitch movement and expressive turns.

- **none/minimal**: direct, punk, folk, chant, conversational.
- **scoops**: slide up into notes; country, pop, blues.
- **slides**: connected pitch movement; R&B, soul, rock, folk.
- **melisma**: multiple notes per syllable; R&B, gospel, qawwali-adjacent, soul.
- **mordents/turns**: quick classical or folk ornaments.
- **cries**: emotional bends or breaks.
- **yodel breaks**: controlled register flips; country, alpine, roots color.
- **blues bends**: flattened notes and expressive pitch inflection.
- **laugh-cry inflections**: klezmer, theatrical, lament, heightened folk color.

### Phrasing

Defines how phrases sit against time and breath.

- **legato**: smooth connected lines.
- **clipped**: short, punchy, consonant-forward.
- **behind-the-beat**: laid-back, R&B, jazz, blues, swagger.
- **ahead-of-the-beat**: urgent, punk, nervous pop, rap drive.
- **rubato**: flexible timing, ballad, devotional, classical, lament.
- **conversational**: natural speech rhythm.
- **chant-like**: repetitive, ritual, communal, simple pitch motion.
- **syncopated**: groove-driven, dance, funk, R&B, Latin, Afro-diasporic styles.

### Breath Control

Defines phrase length and audibility of breathing.

- **short phrases**: urgent, punk, rap-adjacent, fragile, breathless.
- **long arcs**: ballad, classical, gospel, cinematic control.
- **audible breaths**: intimacy, vulnerability, physical realism.
- **hidden breaths**: polished, seamless, studio control.
- **gasping urgency**: fear, desire, panic, catharsis.
- **sustained lines**: anthem, theater, gospel, classical, cinematic.
- **appoggio-like support**: balanced classical breath management, stable tone, controlled release.
- **messa di voce**: crescendo and decrescendo on one sustained pitch; refined classical or art-song control.
- **stamina-forward**: demanding long-form singing without loss of tone; useful for dramatic and operatic prompts.

### Articulation

Defines consonant and vowel behavior.

- **crisp**: intelligible, studio, theater, pop clarity.
- **soft-edged**: intimate, dreamy, legato, less percussive.
- **percussive**: rhythmic consonants, rap, funk, Latin, dance.
- **liquid**: smooth vowels, R&B, soul, jazz.
- **staccato**: separated attacks, punk, electro, theater, comedy.
- **consonant-heavy**: narrative, punk, rap, spoken-sung.
- **vowel-forward**: sustained chorus notes, open belting, choral writing.
- **legato**: smooth connected articulation from note to note; central to classical, ballad, and lyrical prompts.
- **agile**: fast passages, leaps, ornaments, and clean changes; essential for coloratura and lighter Fach prompts.

### Diction and Accent

Defines pronunciation, vowel shape, and speech rhythm. Use respectful, broad descriptors; avoid caricature.

- **treble voice**: broad term for high vocal range or part; useful when avoiding gendered language.
- **non-treble voice**: broad term for tenor, baritone, bass, and other lower adult voices; useful when avoiding gendered language.
- **neutral studio**: minimal regional marking, broadly commercial.
- **subtle regional**: light vowel or consonant color.
- **broad regional**: stronger speech-rhythm or vowel identity; use carefully.
- **theater-clear**: highly intelligible, projected, precise.
- **street-conversational**: informal, speech-rooted, contemporary.
- **liturgical**: formal, ritual, sacred, sustained vowels.
- **chamber-articulate**: refined, small-ensemble precision.
- **diction foregrounding**: hidden, subtle, moderate, foregrounded.

### Rhythmic Feel

Defines the singer's relationship to groove.

- **straight**: cleanly on the grid.
- **swung**: triplet or jazz-inflected motion.
- **backphrased**: delayed phrase starts, relaxed sophistication.
- **rushed**: urgent, anxious, punk, ecstatic.
- **syncopated**: offbeat accents and groove interplay.
- **polyrhythmic**: layered rhythmic identity, Afro-diasporic or experimental.
- **chant pulse**: repeated rhythmic-cell delivery.
- **half-time**: heavier, slower-feeling delivery over the same tempo.
- **floating**: weak grid attachment, ambient, rubato, dreamlike.

### Genre Gravity

Anchors the vocal choices in a coherent musical world.

- **pop**: clear hooks, polished phrasing.
- **R&B/soul**: melisma, groove, warm tone, behind-the-beat phrasing.
- **gospel**: power, call-and-response, runs, lift.
- **jazz**: swing, timing nuance, relaxed diction, harmonic sophistication.
- **folk/country**: storytelling, twang or plainspoken diction, acoustic plausibility.
- **rock/punk/metal**: grit, belt, shout, rasp, distortion, force.
- **theater**: diction, dramatic projection, section clarity.
- **electronic/dance**: processing, repetition, locked pulse, bright or synthetic tone.
- **Latin pop/urban**: rhythmic diction, dance pulse, bright hooks.
- **Afro-diasporic groove**: call-response, polyrhythm, ensemble energy.
- **devotional/classical**: sustained tone, modal gravity, formal restraint.
- **ambient**: breath, texture, space, minimal movement.
- **choral/classical**: SATB part logic, blend, legato, projection, controlled vibrato, repertoire suitability.

### Emotional Stance

Defines the performed attitude.

- **confessional**: private, honest, close.
- **triumphant**: lifted, victorious, open.
- **haunted**: restrained, shadowed, unresolved.
- **playful**: light, teasing, agile.
- **devotional**: prayerful, reverent, repeating.
- **rebellious**: defiant, rough, direct.
- **cinematic**: wide, dramatic, visually suggestive.
- **detached**: cool, dry, observational.
- **ecstatic**: overflowing, repetitive, high-energy.
- **tender**: warm, gentle, careful.
- **sarcastic**: dry, clipped, characterful.
- **ceremonial**: formal, ritual, communal.

### Ensemble Role

Defines how the lead interacts with other voices.

- **solo lead**: voice carries the full song identity.
- **call-and-response leader**: lead is answered by group or choir.
- **choir anchor**: lead sits inside or in front of choral mass.
- **harmony stack**: layered backing thickens hooks.
- **duet-like self-response**: alternating lead colors or doubled persona.
- **narrator**: lead remains intelligible and story-forward.
- **gang vocal leader**: communal shout, punk, anthem, sports-chant energy.

### Dynamic Shape

Defines the arc across the song.

- **flat intimate**: little volume change, tension through closeness.
- **terrace dynamics**: clear step-ups by section.
- **slow crescendo**: gradual build across the song.
- **sudden burst**: explosive contrast after restraint.
- **final surge**: final chorus exceeds prior peaks.
- **decrescendo after peak**: cathartic comedown or afterglow.

### Production Texture

Defines the recorded vocal environment.

- **dry close-mic**: intimate, present, minimal reverb.
- **glossy pop**: polished, tuned, doubled, bright.
- **tape-warm**: analog softness, saturation, vintage warmth.
- **lo-fi**: rough, filtered, bedroom, cassette-like.
- **cathedral reverb**: sacred, huge, sustained ambience.
- **distorted**: saturated, industrial, rock, aggressive.
- **vocodered**: robotic harmony, electronic identity.
- **hyper-processed**: pitch, chop, glitch, digital extremity.
- **chamber-natural**: realistic room, acoustic ensemble.
- **solo-recital natural**: present classical or art-song voice in a small acoustic.
- **choral-hall blend**: ensemble space, softened individual edges, cohesive sections.

### Movement Behavior

Defines how the voice changes by song section.

- **rubato entrance**: flexible opening before groove arrives.
- **low intimate verse**: close, restrained, speech-rooted opening.
- **rising tension pre-chorus**: register or intensity climbs.
- **big chorus**: open vowels, wider projection, stronger dynamics.
- **melismatic lift**: ornament intensifies on emotional lines.
- **chanted hook**: rhythmic repetition carries memorability.
- **spoken-sung breakdown**: words become rhythmic and direct.
- **ad-lib finale**: final chorus adds riffs, responses, or upper-register phrases.
- **call-response ending**: group voices answer the lead.
- **afterglow outro**: softened resolution after peak.

### Failure-Mode Sensitivity

Use avoid clauses only when they protect the intended coordinate.

- **pitch drift**: risky with high, wide, or ornament-heavy voices.
- **over-ornamenting**: risky with melisma-heavy prompts.
- **muddied diction**: risky with breathy, distorted, or low voices.
- **harsh sibilance**: risky with bright, nasal, metallic, or compressed voices.
- **generic pop smoothing**: risky when distinctive vocal identity matters.
- **unstable genre shift**: risky with fusion prompts.
- **exaggerated accent**: avoid parody; ask for respectful, natural diction only.

## Prompt Assembly

When writing the final style prompt, do not enumerate every coordinate dimension. Compress the most important dimensions into a natural musical phrase:

```text
modern neo-soul ballad, velvet alto, low-middle tessitura, breathy clear phonation, delayed vibrato, liquid diction, behind-the-beat phrasing, warm close-mic production, intimate verses and lifted harmony-stack choruses
```

## Guardrails

- Convert references into feature-space coordinates.
- Keep created vocal identities non-imitative and clearly separate from real singers.
- Treat accent and dialect as broad diction, vowel-shape, and rhythmic-speech features; avoid parody or ethnic stereotyping.
- Use performance cues only for major delivery changes; in lyric output, embed them inside the relevant section tag. The style prompt should carry the global coordinate.
