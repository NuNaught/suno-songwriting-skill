---
name: suno-songwriting
description: Generate, revise, translate, and adapt song lyrics plus compact style prompts for Suno or similar AI music generators. Use when the user wants ready-to-paste AI music generation lyrics, lyric tags, Suno/Udio-style prompts, vocal direction, instrumentation, genre/style wording, song structure, multilingual singable lyrics, or a clarifying interview for an AI-generated song. Do not route general music theory, ordinary artist research, or non-generation songwriting discussion here unless the requested deliverable is lyrics or a generation-ready style prompt.
---

# Suno Songwriting

## Reference Files

| File | Use |
| --- | --- |
| `references/clarifying-interview-instructions.md` | Intake ledger, interview loop, sufficiency gate, and sketch-mode exception. |
| `references/lyric-writing-instructions.md` | Lyric composition, revision, rhyme, structure, hooks, bridges, and title options. |
| `references/style-writing-instructions.md` | Suno style prompts, prompt length, ordering, genre fusion, production direction, and negative constraints. |
| `references/genre-knowledge.md` | Genre selection, genre fusion, era references, subgenre vocabulary, and production traits. |
| `references/vocal-routing-index.md` | Lightweight routing for vocal descriptions, profile resources, comparison, and voice-design depth. |
| `references/instrument-knowledge.md` | Band, orchestration, synth, rhythm section, sound palette, and arrangement vocabulary. |
| `references/lyric-tag-knowledge.md` | Bracketed lyric tags, section tags, performance cues, instrumental breaks, and tag restraint. |
| `references/translation-instructions.md` | Non-English lyrics, bilingual lyrics, translation, localization, syllable preservation, and singability. |
| `references/extended-genre-diversity-matrix.md` | Index for uncommon, historical, regional, and fusion genre vocabulary; route from here to the relevant `genres-*.md` file. |
| `references/structure-movement-tags.md` | Index for detailed structure, movement, energy, pulse, climax, drop, improvisation, and arrangement tags. |
| `references/vocal-identity-library.md` | Index for named vocal identities, voice-profile comparison, profile prompt variants, and evaluation rubrics. |

Load specialized profile, genre, and tag-family files only through their index resources when the task calls for that depth.

## Core Workflow

Use this skill to produce two coordinated outputs:

1. Lyrics suitable for Suno's lyric field, using section tags that embed any optional performance, movement, arrangement, or enriched cue tags.
2. A style prompt suitable for Suno's style prompt field, using either compact or rich production-brief form based on the user's brief.

Start by reading `references/clarifying-interview-instructions.md` for any new song, major rewrite, translation/adaptation with taste decisions, or request where the user asks for a Suno-ready result. Run the interview by default unless the user has already provided a complete brief with all critical inputs. Maintain the interview checklist from that file as an internal intake ledger: each required area must be collected from the user, inferred with reasonable confidence for low-impact details, or explicitly skipped/omitted because the area is irrelevant. Ask up to five questions per interview turn, with one unresolved input category per question; do not combine discrete categories into a single question or answer set. Continue until every critical input has been explicitly supplied by the user, and do not skip asking for a critical input merely because the user declined questions, delegated choices, requested a quick draft, or said "decide everything else." Do not treat a topic plus genre, or a topic plus mood, as a complete brief.

Hard stop: for a new song from a thin brief, do not return the final four-section output on the first response. Return an intake snapshot and clarifying questions instead.

## Draft / Sketch Mode

Use sketch mode only when the user explicitly asks for a quick draft, rough version, starter lyric, brainstorm, first pass, exploratory option, or similar non-final deliverable. Sketch mode is for ideation speed, not final Suno-ready output.

Before producing a sketch, collect or confirm these minimum inputs:

1. Deliverable scope.
2. Subject/premise.
3. Primary genre or broad style lane.
4. Lyric perspective, if lyrics are requested.
5. Forbidden content or confirmation that there are no constraints.

For sketch mode, infer story angle, emotional endpoint, vocal identity, vocal style, target duration, section structure, BPM, key, arrangement motion, and other low-risk controls with best judgment. Do not run the mandatory critical-input review gate before a sketch. Do not present the sketch as final, polished, release-ready, or Suno-ready.

Use this sketch format:

```markdown
### Sketch Draft
...

### Assumptions
...

### Next Questions
...
```

If the user asks to finalize, polish, export, or make a sketch Suno-ready, return to the normal interview and critical-input review flow before producing the final `Title` / `Lyrics` / `Style` / `Analysis` output.

## Mandatory Critical-Input Review Gate

This gate is enforced at the skill level for every request that will generate lyrics, a style prompt, or the final `Title` / `Lyrics` / `Style` / `Analysis` output.

Before generating lyrics or a style prompt, always show the user a compact critical-input review and ask for confirmation. This is required even when the user supplied a complete brief. Do not produce generation output in the same response as this review.

Use this format:

```markdown
Critical inputs to review:
- User decisions: ...
- Best-judgment decisions: ...

Reply "approved" to generate, or tell me what to change.
```

`User decisions` must summarize the critical choices the user directly supplied through the brief or interview. `Best-judgment decisions` must summarize only non-critical choices the skill inferred or defaulted.

The review must cover all generation-shaping inputs that apply: deliverable scope, premise, story angle, lyric perspective, addressee/listener, emotional endpoint, tone, intensity, primary genre, support genre or fusion, BPM or tempo feel, key or mode, production direction, vocal identity, vocal style, target duration, section plan, lyric density, enriched tags, tag restraint, arrangement motion, language, explicitness, required phrases, forbidden content, safety constraints, sensitive-content handling, and use case. For Suno-ready songs, section structure, BPM/tempo, key/mode, vocal identity, and vocal style must be explicitly supplied by the user before approval.

Only after the user approves the review or explicitly asks to proceed with those assumptions may the skill generate lyrics, style prompt text, title options, or analysis. If the user changes a critical input, update the review and ask for confirmation again before generation.

## Resource Routing

Load only the resources needed for the specific task:

- For lyric composition, revision, rhyme, structure, hooks, bridges, and title options, read `references/lyric-writing-instructions.md`.
- For Suno style prompts, prompt length, ordering, genre fusion, mood, production, and negative constraints, read `references/style-writing-instructions.md`.
- For genre selection, genre fusion, era references, subgenre vocabulary, and production traits, read `references/genre-knowledge.md`.
- For ordinary singer description, harmony, choir, rap, spoken, duet, and vocal production direction, read `references/vocal-routing-index.md` first; it routes to compact vocal style, coordinate, profile, comparison, and rubric resources.
- For band, orchestration, synth, rhythm section, sound palette, and arrangement vocabulary, read `references/instrument-knowledge.md`.
- For bracketed lyric tags, section tags, performance cues, instrumental breaks, and tag restraint, read `references/lyric-tag-knowledge.md`.
- For non-English lyrics, bilingual lyrics, translation, localization, syllable preservation, and singability across languages, read `references/translation-instructions.md`.
- For requirements gathering before writing, read `references/clarifying-interview-instructions.md`.

Use index resources first when the task needs more breadth or specialized vocabulary:

- For uncommon, historical, regional, or fusion genre vocabulary, read `references/extended-genre-diversity-matrix.md`, then load only the relevant `references/genres-*.md` family file.
- For detailed structure, motion, energy, pulse, climax, drop, improvisation, and arrangement tags, read `references/structure-movement-tags.md`, then load only the relevant tag-family file.
- For named vocal identities, voice-profile comparison, profile prompt variants, and evaluation rubrics, read `references/vocal-identity-library.md`, then load only the relevant profile, prompt, comparison, or rubric file.
- For detailed voice-coordinate design without named profiles, read `references/vocal-style-knowledge.md` or `references/vocal-feature-space.md`.
- For generating or expanding a vocal identity library, read `references/vocal-identity-generation-instructions.md`.

## Output Contract

Always return the final result as a Markdown file with exactly these H3 sections in this order: `Title`, `Lyrics`, `Style`, `Analysis`. Put the content under each H3 header inside a fenced code block for easy copy/paste.

Use this structure:

````markdown
### Title
```text
...
```

### Lyrics
```markdown
[Verse 1]
...
```

### Style
```text
...
```

### Analysis
```markdown
...
```
````

Keep the style prompt concise but not under-specified: use a comma-separated compact prompt for simple briefs, or a denser production-brief prompt for distinctive fusion, detailed vocal behavior, instrumentation, arrangement motion, lyric premise, or duration constraints. Make the lyrics singable, structured, and ready to paste into Suno. In the `Lyrics` block, every bracketed lyric tag must be a section tag; embed all enriched cue tags, movement tags, arrangement tags, and performance tags inside the relevant section tag, such as `[Verse 1 - Spoken Delivery]` or `[Final Chorus - Big Chorus, Ad-Lib Finale]`. Do not place standalone cue or performance tags inside lyrics. In `Analysis`, focus primarily on the lyrics' meaning: narrative arc, speaker, themes, metaphors, imagery, emotional turn, and how the hook reframes the song. Discuss style prompt, structure, duration, or enrichment choices only where they support meaning, narrative, themes, imagery, or emotional pacing. If the user asks for multiple options, repeat the same four-section structure for each option and vary genre, hook angle, vocal direction, or arrangement rather than making near-duplicates.

## Post-Output File Offer

After generating and displaying the final `Title` / `Lyrics` / `Style` / `Analysis` output, offer to write the exact displayed Markdown to a local file. Do not write the file before displaying the output unless the user explicitly requested file creation in advance.

Use a concrete suggested path in this form:

```text
./songs/{YYYYMMDD-HHMMSS}-{song-title-slug}.md
```

Use the user's local date/time when available. Create the title slug from the selected title: lowercase, ASCII when practical, hyphen-separated, and stripped of punctuation that is unsafe in filenames. If there are multiple song options, offer one file per option with distinct title slugs. If the suggested filename already exists, append `-2`, `-3`, or the next available numeric suffix rather than overwriting.

End the final response with a short offer such as:

```markdown
I can also write this to `./songs/20260512-143015-example-title.md`.
```

If the user accepts, create the `songs` directory if needed and write the exact final Markdown content, including the four H3 sections and fenced code blocks.

For sketch mode, do not offer to write a file unless the user explicitly asks to save the sketch.

## Decision Rules

- Prefer concrete musical descriptors over abstract praise.
- Keep Suno style prompts focused and ordered. For compact prompts, use signature sound or style first when present, then genre, BPM, key, support styles, vocal identity, instrumental roles, lyric premise, and production texture. For rich prompts, follow `references/style-writing-instructions.md`.
- Avoid asking questions about critical inputs only when the user gave a complete brief that explicitly supplies those inputs; otherwise use the clarifying interview before writing.
- Avoid mentioning instrument names or musical concepts in lyrics unless the user made that the theme.
- Treat generated vocal identities as profiles with concrete vocal, genre, diction, and production traits.
- Use a moderate number of bracketed lyric tags by default: normal section labels plus a few consequential enriched cues embedded in those section labels, avoiding tag clutter.
- For translations, preserve singability and emotional intent over literal word order.
