# Lyric Writing Instructions

Write lyrics that can be sung, not just read. Prioritize clear phrasing, memorable hooks, and natural stress.

## Inputs to Extract

- Theme or story
- Point of view
- Genre and tempo
- Emotional arc
- Song length or target duration
- Audience or use case
- Required phrases, names, places, or constraints
- Language and explicit content level

## Song Structure

Default to a complete contemporary structure:

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

Shorten for quick demos or extend for narrative songs.

## Length Heuristics

If the user specifies duration, scale the amount of lyric material to fit. Treat these as rough caps, not exact timing guarantees:

- **30-60 seconds**: hook-first demo; 1 short verse or intro, 1 chorus/hook, optional outro; about 8-16 lyric lines.
- **1-2 minutes**: compact song; verse, pre-chorus or lift, chorus, optional bridge/breakdown; about 16-28 lyric lines.
- **2-3 minutes**: standard full song; two verses, recurring chorus, bridge or breakdown, final chorus; about 28-48 lyric lines.
- **3-4 minutes**: expanded full song; standard form with intro/outro, post-chorus, interlude, or longer bridge; about 40-64 lyric lines.
- **4+ minutes**: extended narrative, dance, progressive, devotional, or cinematic form; add sections only when they serve the concept.

When no length is specified, default to a standard 2-3 minute structure unless the user asks for a snippet, hook, chorus only, or long-form piece.

## Lyric Craft

- Make verses specific: images, actions, places, objects.
- Make choruses simple and repeatable: central phrase, emotional thesis, title phrase if possible.
- Use pre-choruses to increase tension or motion.
- Use bridges to shift perspective, reveal a turn, or create contrast.
- Keep line lengths singable. Vary them intentionally, not randomly.
- Use rhyme as support, not a cage. Internal rhyme and slant rhyme often sound more natural.
- Avoid naming instruments, production terms, song sections, genres, keys, BPM, or other musical concepts inside the lyrics unless that is explicitly part of the song's theme.
- Avoid generic filler like "in the night", "feel alive", "never let go" unless refreshed by context.

## Structure Tags and Enrichment

- Use moderate enriched structure tags by default: enough to shape the generation, not so many that tags crowd the lyrics.
- Pair most complete songs with normal section labels plus about 4-8 consequential enriched cues.
- Attach enriched cues to their target section in one bracketed tag using `Section - Cue`, for example `[Pre-Chorus - Rising Tension]`, `[Chorus - Big Chorus]`, `[Final Chorus - Final Surge]`, or `[Outro - Afterglow]`. Do not put `[Pre-Chorus]` and `[Rising Tension]` on separate adjacent lines.
- Add enrichments when they create audible behavior: `[Rubato Entrance]`, `[Slow Build]`, `[Rising Tension]`, `[Big Chorus]`, `[Ma Space]`, `[Chanted Hook]`, `[Final Surge]`, `[Afterglow]`.
- If the user has not specified structure for a new song or Suno-ready deliverable, ask about section structure before writing.
- If proceeding without an interview because the user gave a complete brief, choose 2-4 coherent low-impact enrichments that match the genre and emotional arc.

## Rhyme and Meter

- For pop/country/folk, use clear end rhymes and stable line lengths.
- For rap, use internal rhyme, multisyllabic rhyme, and cadence variation.
- For ballads, allow longer lines but keep breath points obvious.
- Read each line aloud mentally; if stress falls awkwardly, rewrite.

## Hook Design

Strong hooks usually include:

- A short title phrase.
- A rhythmic shape that can repeat.
- A contrast between concrete image and emotional meaning.
- Optional post-chorus chant if the genre supports it.

## Revision Checklist

- Does the chorus summarize the song in language a listener remembers?
- Does each verse add new information?
- Are there avoidable cliches?
- Are section lengths balanced?
- Would the words fit the requested genre's mouth-feel?
- Are bracketed tags useful, not excessive, and formatted as one section-cue tag rather than split adjacent tags?
