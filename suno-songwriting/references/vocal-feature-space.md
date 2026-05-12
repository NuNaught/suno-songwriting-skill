# Vocal Feature Space

Use this first when designing distinctive vocal identities or converting artist references into safe voice traits.

## I. Executive summary

This library defines a high-cardinality design space of **60 vocal identities** for testing the same original song across meaningfully distinct vocal profiles. The profiles are designed as theoretical musical personas: each combines range behavior, timbre, phonation, diction, rhythmic feel, genre gravity, emotional stance, production texture, and movement behavior.

The shared comparison song, **“Lantern in the Water,”** is written to be genre-neutral but movement-rich. It contains an intimate low-register verse, rising pre-chorus, open-vowel chorus, rhythmic second verse, quiet bridge, chant/spoken-sung breakdown, and climactic final chorus with room for ad-libs or call-and-response. The goal is to let identical lyrics reveal differences in vocal identity, not to create separate songs.

Design assumptions applied:
- 60 adult fictional profiles.
- Target comparison-song duration: about 3:00.
- High-diversity design with some risky edge cases.
- Accents/diction handled respectfully as broad articulation/vowel-shape features, with foregrounding level treated as a variable.
- Suno prompts optimized case-by-case for the clearest audible differentiation.
- Enriched lyric tags are restrained and chosen for audible consequences.

## II. Feature-space design

| Dimension name | Possible values | Why it matters perceptually | How it can be prompted in Suno |
|---|---|---|---|
| Vocal role | soprano, mezzo, alto, contralto, tenor, baritone, bass, countertenor, ensemble lead, chant leader, shouter, crooner | Establishes expected pitch center, cultural role, and arrangement placement | “mezzo lead,” “adult baritone storyteller,” “countertenor head-voice lead” |
| Approximate range | low, mid, high, wide, narrow; approximate note bands such as G2–D4 or A3–E5 | Affects perceived physicality, brightness, strain, and climax height | “comfortable midrange with brief high peaks,” “low contralto center with narrow upper extension” |
| Tessitura | low-set, middle-set, high-set, flexible, octave-jumping | Determines where the voice sounds most natural and stable | “keep verses in a low tessitura, chorus opens into upper midrange” |
| Vocal weight | featherweight, light, lyric, medium, heavy, dramatic, gravel-heavy | Changes impact, intimacy, and believability in dense arrangements | “light lyric voice,” “heavy dramatic belt,” “medium-weight smoky alto” |
| Register balance | chest-dominant, mix-dominant, head-dominant, falsetto-forward, break-embracing, seamless | Makes chorus, bridge, and ad-libs behave differently | “chest-led verses, mixed belt chorus, airy head-voice bridge” |
| Phonation | breathy, clear, pressed, speech-like, aspirate, creaky, growled, distorted, clean | One of the strongest timbral identifiers; defines intimacy vs force | “breathy onset,” “clean phonation,” “controlled rasp,” “pressed rock delivery” |
| Timbre color | bright, dark, smoky, metallic, glassy, woody, nasal, airy, velvet, copper, steel, honeyed | The listener’s fastest way to identify the voice | “bright metallic tenor,” “dark velvet contralto,” “smoky close-mic alto” |
| Projection style | close-mic intimate, theatrical, open-throat, stadium, chamber, conversational | Shapes the apparent space and scale of the performer | “dry close-mic delivery,” “open-throat chorus projection,” “theatrical forward placement” |
| Vibrato | straight-tone, narrow fast, wide slow, delayed, tremolo-like, ornamental, dramatic | Affects age impression, genre code, emotional heat, and note endings | “mostly straight tone with delayed vibrato,” “wide theatrical vibrato on sustained vowels” |
| Ornamentation | none, scoops, slides, melisma, mordents, turns, cries, yodel breaks, blues bends, laugh-cry inflections | Creates genre identity and distinguishes expressive grammar | “late-phrase scoops,” “brief melismatic turns,” “controlled yodel breaks” |
| Phrasing | legato, clipped, behind-the-beat, ahead-of-the-beat, rubato, conversational, chant-like, syncopated | Determines groove relationship and lyric intelligibility | “behind-the-beat neo-soul phrasing,” “clipped punk diction,” “rubato lament phrasing” |
| Breath control | short phrases, long arcs, audible breaths, hidden breaths, gasping urgency, sustained lines | Reveals vocal athleticism and emotional stance | “long controlled phrases,” “audible breath before the chorus,” “short urgent phrase bursts” |
| Articulation | crisp, soft-edged, percussive, liquid, staccato, consonant-heavy, vowel-forward | Makes words either sharp and rhythmic or smooth and melodic | “crisp consonants,” “liquid vowels,” “percussive rhythmic diction” |
| Diction/accent | neutral studio, broad regional, subtle regional, theater-clear, street-conversational, liturgical, chamber-articulate | Changes vowel shape, consonant timing, and speech rhythm without invoking real singers | “subtle coastal vowel warmth,” “broad but respectful rhotic clarity,” “theater-clear diction” |
| Diction foregrounding | hidden, subtle, moderate, foregrounded | Lets accent/dialect be a dimension without parody | “subtle vowel color only,” “moderately foregrounded speech rhythm, respectful and natural” |
| Rhythmic feel | straight, swung, backphrased, rushed, syncopated, polyrhythmic, chant pulse, half-time, floating | Makes the same lyric feel genre-coded | “laid-back swing,” “urgent ahead-of-beat attack,” “locked dance-pocket delivery” |
| Genre gravity | pop, R&B, soul, gospel, jazz, folk, country, rock, punk, metal, theater, electronic, Latin pop, Afro-diasporic groove, devotional, ambient | Anchors vocal choices in coherent musical worlds | “jazz-soul arrangement,” “electronic art-pop texture,” “roots-folk chamber setting” |
| Emotional stance | confessional, triumphant, haunted, playful, devotional, rebellious, ceremonial, detached, ecstatic, tender, sarcastic | Same melody can feel like prayer, protest, flirtation, or confession | “haunted but restrained,” “ecstatic final chorus,” “dryly sarcastic spoken-sung verse” |
| Ensemble role | solo lead, call-and-response leader, choir anchor, harmony stack, duet-like self-response, narrator | Defines how the voice interacts with backing voices | “lead with group response in final chorus,” “choir-anchor voice,” “self-harmonized ad-libs” |
| Dynamic shape | flat intimate, terrace dynamics, slow crescendo, sudden burst, final surge, decrescendo after peak | Determines song arc and test reliability | “verse restrained, pre-chorus gradual lift, final chorus return bigger” |
| Production texture | dry close-mic, glossy pop, tape-warm, lo-fi, cathedral reverb, distorted, vocodered, hyper-processed, chamber-natural | Suno often responds strongly to production adjectives | “dry close-mic vocal,” “glossy layered production,” “controlled distortion on climaxes” |
| Movement behavior | rubato entrance, rising tension, big chorus, melismatic lift, chanted hook, ad-lib finale, call-response, afterglow | Connects profile identity to song sections | “quiet bridge should expose head voice; final chorus should add call-and-response ad-libs” |
| Failure-mode sensitivity | pitch drift, over-ornamenting, muddied diction, harsh sibilance, generic pop smoothing, unstable genre shift | Helps negative prompts preserve profile identity | “avoid overprocessed tuning, exaggerated accent, unstable growls” |

