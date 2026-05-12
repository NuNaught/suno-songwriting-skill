# Lyric Tag Knowledge

Bracketed tags can guide Suno's structure and performance. Use a moderate amount by default: enough to shape structure, motion, and a few important performance behaviors, but not so many that tags crowd the lyrics.

Hard rule for lyric output: every bracketed lyric tag must be a section tag. Embed all enriched cue tags, movement tags, arrangement tags, and performance tags inside the relevant section tag instead of writing them as standalone or inline tags. For example, use `[Verse 1 - Whispered]`, `[Pre-Chorus - Rising Tension]`, `[Chorus - Big Chorus, Group Response]`, or `[Outro - Afterglow]`.

For a larger catalog of structure, energy, pulse, texture, vocal delivery, formal development, climax, genre-specific, and hybrid movement tags, read `structure-movement-tags.md` first. It routes to focused tag-family files.

## Section Tags

- `[Intro]`
- `[Verse 1]`, `[Verse 2]`
- `[Pre-Chorus]`
- `[Chorus]`
- `[Post-Chorus]`
- `[Bridge]`
- `[Breakdown]`
- `[Instrumental]`
- `[Guitar Solo]`, `[Sax Solo]`, `[Piano Solo]`
- `[Final Chorus]`
- `[Outro]`

## Performance Cues

Performance cues must be embedded in section tags when used in lyrics:

- `[Verse 1 - Spoken]`
- `[Verse 1 - Whispered]`
- `[Chorus - Shouted]`
- `[Chorus - Call and Response]`
- `[Final Chorus - Harmonies]`
- `[Bridge - Choir]`
- `[Final Chorus - Ad-Libs]`
- `[Verse 2 - Rap Verse]`
- `[Bridge - Falsetto]`

## Movement Tags

Use movement tags when the user wants arrangement-level motion rather than only lyric sections:

- Energy: `[Slow Build]`, `[Rising Tension]`, `[Release]`, `[Final Surge]`, `[Afterglow]`
- Pulse: `[Free Time]`, `[Rubato Entrance]`, `[Pulse Emerges]`, `[Locked Groove]`, `[Half-Time Shift]`, `[Double-Time Lift]`
- Texture: `[Drone Bed]`, `[Sparse Percussion]`, `[Full Rhythm Section]`, `[Layered Harmonies]`, `[Interlocking Pattern]`, `[Filtered Texture]`
- Vocal: `[Spoken Intro]`, `[Chanted Hook]`, `[Melismatic Lift]`, `[Group Response]`, `[Lead Improvisation]`, `[Harmony Stack]`
- Space and restraint: `[Ma Space]`, `[Measured Silence]`, `[Quiet Contrast]`
- Pop/EDM/rock forms: `[Hook First]`, `[Big Chorus]`, `[Riser Build]`, `[Main Drop]`, `[Full Band Entry]`, `[Wall-of-Guitars]`

## Placement

- Put each section opening on one bracketed line.
- When a section has a movement, arrangement, enriched, or performance cue, combine the section label and cue in the same bracket using `Section - Cue`: `[Intro - Spoken Intro]`, `[Pre-Chorus - Rising Tension]`, `[Chorus - Big Chorus]`, `[Breakdown - Spoken]`, `[Final Chorus - Final Surge]`, `[Outro - Afterglow]`.
- Do not split a section label and its cue into adjacent standalone tags. Avoid:

```markdown
[Outro]
[Afterglow]
```

Use:

```markdown
[Outro - Afterglow]
```

- Do not put performance tags on their own line or inline with a lyric phrase. Avoid `[spoken]`, `[whispered]`, `[ad-libs]`, `[call and response]`, or similar standalone/inline tags in the lyric body; embed them in the section tag instead.
- Prefer structure tags over many micro-performance tags.

## Restraint Rules

- Use normal section labels for the chosen structure, plus about 4-8 enriched cues for most complete songs.
- Prefer 1-2 tags per section when using enriched movement cues.
- Avoid tagging every vocal texture; the style prompt can carry global vocal direction.
- Prefer enriched tags on structurally important moments: intro, pre-chorus lift, first chorus payoff, bridge/breakdown contrast, final chorus, or outro.
- If generation ignores tags, simplify them rather than adding more.
- Do not use obscure or invented tags unless the user explicitly wants experimentation.

## Useful Structures

Pop:

```markdown
[Verse 1]
[Pre-Chorus]
[Chorus]
[Verse 2]
[Pre-Chorus]
[Chorus]
[Bridge]
[Final Chorus]
[Outro]
```

EDM:

```markdown
[Verse]
[Pre-Chorus]
[Build]
[Drop]
[Verse 2]
[Build]
[Drop]
[Bridge]
[Final Drop]
```

Rap:

```markdown
[Intro]
[Verse 1]
[Hook]
[Verse 2]
[Hook]
[Bridge]
[Final Hook]
```
