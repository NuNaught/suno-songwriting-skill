# Vocal Identity Generation Instructions

Use this resource when creating or expanding a vocal identity library for Suno comparison testing. It is a source prompt/specification, not a required workflow for ordinary lyric writing.

You are a computational musicologist, vocal pedagogy expert, lyricist, and prompt engineer for generative music systems.

I am creating a library of meaningfully distinct theoretical vocal identities for use in Suno music generation. The goal is to create a high-cardinality design space of fictional, musically coherent voice profiles that can be tested against the same song.

Your task is to generate the complete design package below.

Core objective:
Create a graph/list of fictional vocal identities, a common comparison song, and Suno style prompts for each vocal identity performing that same song.

Important constraints:
- Accents and dialects may be used as musical-vocal features, but handle them respectfully and avoid parody, caricature, or ethnic stereotyping.
- Treat all vocal identities as adult performers.
- Maximize meaningful distinctness, not random variation.
- Keep the common lyrics identical across all profiles so that voice and style differences can be compared.
- Use restrained enriched cues in lyrics: enough to trigger vocal variety, but not so many that the generated song becomes unstable. Embed every cue inside a section tag.
- Suno prompts should be concise, musically actionable, and optimized for style/voice differentiation.

Deliverables:

1. Vocal feature space
Define the feature dimensions used to distinguish vocal identities. Include dimensions from:
- Vocal role and music theory: range, tessitura, register balance, vocal weight, projection, vibrato, ornamentation, phrasing, breath control, ensemble role.
- Timbre and production: breathy, clear, nasal, smoky, bright, dark, metallic, airy, raspy, smooth, intimate, theatrical, distorted, etc.
- Genre style: pop, R&B, soul, gospel, jazz, folk, country, rock, punk, metal, classical crossover, musical theater, electronic, dance, hip-hop-adjacent, reggae, Afrobeat, Latin pop, indie, ambient, etc.
- Regional accent/dialect features: broad and respectful descriptions of pronunciation, vowel shape, consonant articulation, rhythmic speech influence, and diction.
- Inflection and performance features: melisma, slides, scoops, yodel breaks, spoken-sung phrasing, staccato diction, legato phrasing, growls, belting, falsetto/head voice, call-and-response, chant-like repetition, whisper tone.
- Emotional/performance stance: confessional, triumphant, haunted, playful, devotional, rebellious, cinematic, detached, ecstatic, tender, sarcastic, ceremonial, etc.
- Song-function behavior: how the voice handles verses, pre-choruses, choruses, bridge, breakdown, climactic ending.

For each dimension, give:
- Dimension name
- Possible values
- Why it matters perceptually
- How it can be prompted in Suno

2. Vocal identity graph/list
Generate 48 to 72 fictional vocal identities. Each identity must have a distinct profile name.

For each profile, include:
- profile_id
- profile_name
- human-readable summary
- voice coordinate vector
- distinguishing features
- likely strengths
- likely weaknesses or failure modes
- best genres
- contrasting nearest-neighbor profiles
- Suno-relevant style vocabulary
- one-sentence “what to listen for” during evaluation

The voice coordinate vector should include at least:
- vocal_role
- approximate_range
- tessitura
- vocal_weight
- timbre
- phonation
- register_behavior
- vibrato
- ornamentation
- articulation
- diction/accent
- rhythmic_feel
- genre_gravity
- emotional_stance
- dynamic_shape
- production_texture
- movement_behavior

Also generate a graph structure:
- Nodes are vocal identities.
- Edges connect identities that are similar but meaningfully contrasted.
- Edge labels should describe the contrast, such as “same genre, different phonation,” “similar range, different accent/diction,” “same timbre, different rhythmic feel,” or “same vocal role, different emotional stance.”
- Include at least 2 edges per node.
- Include a short explanation of the clustering logic.

Output the graph in both:
A. Human-readable Markdown table
B. Machine-readable JSON with nodes and edges

3. Common comparison song
Write one original song to be used across every vocal profile.

Requirements:
- The lyric should be emotionally flexible: it should work in pop, rock, jazz, folk, R&B, gospel, electronic, theater, and acoustic arrangements.
- The lyric should intentionally trigger many different vocal behaviors across the song.
- Include varied movement opportunities:
  - intimate low-register verse
  - rhythmic/spoken-sung phrase
  - rising pre-chorus
  - open-vowel chorus suitable for belting
  - section with room for melisma or ornament
  - quiet bridge
  - dynamic breakdown
  - final chorus with ad-libs or call-and-response
- Use restrained enriched cues. Maximum 1–2 cues per section, embedded inside that section tag.
- Avoid overly specific instrumentation in the lyrics section itself.
- Keep the song between roughly 2:45 and 3:45 in implied structure.
- Make the words clear enough that pronunciation, diction, phrasing, vibrato, and register changes can be evaluated.

Provide:
- Song title
- Overall song concept
- Section-by-section structure
- Lyrics with restrained enriched cues embedded in section tags
- Vocal evaluation notes for each section
- Movement hints that will later be injected into each Suno style prompt

Suggested structure:
[Intro]
[Verse 1 - intimate, low register]
[Pre-Chorus - rising intensity]
[Chorus - open vowels, sustained notes]
[Verse 2 - more rhythmic diction]
[Pre-Chorus 2 - increased lift]
[Chorus 2 - stronger delivery]
[Bridge - quiet contrast, exposed voice]
[Breakdown - pulse, spoken/sung or chant-like]
[Final Chorus - climactic, ad-libs]
[Outro - resolving phrase]

4. Common movement requirements
Extract the song’s movement requirements into a reusable checklist for prompt generation.

For each song section, specify:
- desired vocal behavior
- dynamic level
- register behavior
- articulation requirement
- expressive target
- possible Suno tags
- what the section tests in the voice profile

5. Suno style prompts for each vocal identity
For every vocal identity, generate a Suno style prompt that adapts that profile to the common song.

Each Suno prompt must include:
- profile_id
- profile_name
- short voice identity phrase
- full Suno style prompt
- negative prompt / avoid list
- suggested Suno tags
- expected audible result
- comparison notes

The style prompt should combine:
- The profile’s voice coordinate
- The common song movement requirements
- Genre and production context
- Vocal delivery instructions
- Diction/accent/inflection cues
- Sectional behavior across the shared song

Do not include the lyrics repeatedly for every profile. Instead, reference the common song and describe how this profile should perform it.

Suno prompt format:
“[vocal role/range] voice with [timbre], [phonation], [diction/accent], and [inflection style]. [Genre/style] arrangement with [production texture]. Verse 1 should feel [behavior], pre-chorus should [behavior], chorus should [behavior], bridge should [behavior], final chorus should [behavior]. Emphasize [key vocal traits]. Avoid [failure modes].”

For each profile, also provide a compact version under 250 characters.

6. Evaluation rubric
Create a rubric for comparing the generated Suno outputs.

Include scoring categories such as:
- perceived vocal identity distinctness
- timbral distinctness
- range/register behavior
- diction/accent audibility
- genre adherence
- emotional delivery
- section-by-section movement compliance
- lyric intelligibility
- stability/consistency across the song
- uniqueness compared to nearest neighbors

Use a 1–5 scoring system and define each score.

7. Recommended output organization
Return the final answer in this order:

I. Executive summary  
II. Feature-space design  
III. Vocal identity graph/list  
IV. Machine-readable JSON graph  
V. Common comparison song  
VI. Common movement requirements  
VII. Suno style prompts by profile  
VIII. Compact Suno prompt table  
IX. Evaluation rubric  
X. Comparison notes  

Quality bar:
- Make the profiles diverse but musically plausible.
- Avoid vague labels like “unique voice” or “emotional singer” unless supported by concrete vocal features.
- Prefer actionable descriptors: “narrow fast vibrato,” “forward nasal twang,” “breathy onset,” “late-phrase scoops,” “open-throat belt,” “dry close-mic delivery,” “clipped consonants,” “behind-the-beat phrasing.”
- Ensure profiles differ across multiple axes, not just genre names.
- Use enough structure that the output can become a dataset or prompt library.
