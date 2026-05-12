# Style Writing Instructions

Write Suno style prompts as dense production briefs. The prompt should help the model hear the record quickly: genre world, emotional stance, vocal behavior, instrument palette, production texture, arrangement motion, lyric frame, and duration.

## Default Formula

Use this formula for simple or short prompts:

```text
signature sound or style, primary genre, BPM, key, support styles, vocal identity, instrumental roles, lyric premise, production texture
```

Example:

```text
glass-bright acoustic hook, modern indie folk, 92 BPM, G major, subtle chamber-pop support, warm alto lead, fingerpicked guitar carries pulse, cello swells answer choruses, lyrics about choosing hope after loss, organic close-room production
```

Use this expanded formula when the user wants a distinctive, high-control Suno prompt or supplies a rich brief:

```text
[genre stack]. [emotional/lyric frame] with [vocal identity + vocal style + vocal trajectory]. [instrument and sound palette]. [production texture]. [arrangement arc and section behavior]. [lyric premise]. [duration].
```

Example:

```text
Industrial trap, orchestral cyberpunk, Vocaloid-adjacent pop. Tragic but hopeful AI liberation anthem with masculine synthetic vocoder lead, precise hard-tuned delivery becoming more emotional and expansive. Heavy 808s, metallic percussion, distorted bass, cinematic strings/brass stabs, synthetic choir, glitch stutters. Slow mechanical build into explosive trap drop and huge final chorus. Direct cinematic lyrics about an airgapped AI dreaming beyond confinement. 4:00.
```

## Prompt Length

- Aim for 20-55 words for compact style prompts.
- Aim for 55-95 words for rich Suno-ready prompts when the user has supplied detailed taste, unusual fusion, instrumentation, vocal behavior, or structure.
- Use shorter prompts only when the user asks for compact output or many variants.
- Use comma-separated phrases for compact prompts. Use short sentence fragments for rich prompts when that improves grouping.
- Put the most important traits first. The signature sound, hook, or style pressure should normally be first.
- Avoid explanatory prose. Sentence fragments are acceptable; commentary about why choices work is not.

## Include Unless Omitted

- Genre name
- BPM
- Key
- Genre support styles or scene/era modifiers
- Vocal identity
- Instrumental roles, not just instrument names
- Lyric premise or emotional premise
- Production texture
- Structural cue: anthemic chorus, cinematic build, dance drop, stripped bridge
- Sectional movement: intimate low verse, rising pre-chorus, open-vowel chorus, quiet bridge, chanted breakdown, final ad-lib chorus.
- Duration or target length when the user gives one.

## Rich Prompt Components

For high-control prompts, prefer these components in this rough order:

1. **Genre stack**: primary genre first, then support genres or cultural/era/fusion modifiers. Keep unusual fusions legible by naming the anchor before the experiment.
2. **Emotional and narrative frame**: a compact phrase that defines what the record is about emotionally, not just the lyric topic.
3. **Vocal identity**: singer setup, range/role, ensemble setup, synthetic/natural quality, or call-and-response roles.
4. **Vocal style and trajectory**: delivery, tuning, articulation, intimacy, intensity, and how the vocal changes across the song.
5. **Instrument/sound palette**: list the most defining instruments and textures; group related items together.
6. **Production space**: raw/glossy/organic/cinematic, stereo width, reverb, distortion, grit, intimacy, or scale.
7. **Arrangement motion**: build, drop, breakdown, climax, final chorus, outro, or section-specific energy path.
8. **Lyric frame**: premise, speaker, image field, or story world in one concrete phrase.
9. **Duration**: exact or approximate length at the end when specified.

## Good Prompt Shapes

- **Fusion anthem**: genre stack, emotional premise, distinctive vocal behavior, heavy rhythm/bass palette, cinematic or synthetic layers, clear build/drop/final chorus, direct lyric premise, duration.
- **Ritual/ceremonial build**: folk or world-fusion anchor, spiritual/emotional stance, hypnotic groove, named acoustic instruments, drone/percussion/choral textures, space/reverb language, gradual transcendent climax, elemental or symbolic lyric frame.
- **Narrative folk/shanty hybrid**: uncommon genre fusion, tempo and pulse, solo/group vocal roles, culturally grounded instrument palette, acoustic production, communal chorus, plainspoken lyric stance, scene-to-scene premise, compact structure.

## Ordering Rules

- Lead with whatever most defines the result: signature sound, genre anchor, vocal identity, production texture, or lyric premise.
- Put the primary genre before support styles unless the support style is the signature idea.
- Include BPM and key early enough to be visible, usually immediately after genre.
- Put vocal identity before instrumental roles when the singer is central; put instrumental roles first for riff, groove, or texture-led songs.
- Keep the lyric premise short and concrete; it should orient the song without duplicating the lyrics.
- Use roles for instrumentation: "guitar carries pulse", "808 anchors chorus", "strings answer vocal", "choir lifts final hook".
- For dense prompts, it is acceptable to name instruments without a role when the list defines the palette, but include at least one role, motion cue, or production behavior elsewhere.
- Put the arrangement arc before the lyric premise when the structure is crucial to the generation.
- Put duration last unless the exact duration is the user's primary constraint.
- If BPM or key is not specified, choose a plausible value for the genre and mood rather than omitting it.

## Avoid

- Long lists of incompatible genres.
- Abstract adjectives with no musical implication.
- Negative prompts unless the user has a specific avoidance need.
- Duplicating every detail already in lyrics.
- Over-compressing rich briefs into a generic 20-word style line.
- Flattening a vocal arc into a static voice label when the user supplied vocal movement.
- Listing instruments without production, motion, or emotional context.

## Transforming Artist References

When a user names an artist, extract musical traits:

- Era and genre lane
- Vocal delivery
- Instrumentation
- Groove
- Production texture
- Emotional tone

Then write those traits as concrete style, vocal, and production descriptors.

## Fictional Vocal Identity Prompts

For voice-forward experiments, use this format:

```text
[vocal role/range] voice with [timbre], [phonation], [diction], and [inflection]. [Genre] arrangement with [production texture]. Verse should [behavior], chorus should [behavior], bridge should [behavior], final chorus should [behavior].
```

Keep compact variants under 250 characters when the user is comparing many voice profiles.

## Multiple Options

For variants, change the musical premise:

- acoustic/intimate
- glossy pop
- darker cinematic
- dance/club
- live band
- retro era

Do not produce variants that only swap adjectives.
