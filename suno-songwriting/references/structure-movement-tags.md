# Structure and Movement Tags Index

Use this index before loading detailed tag catalogs. Keep actual lyric markup sparse: most full songs should use normal section tags plus only a few consequential movement or performance cues. In lyric output, all movement, performance, arrangement, and enriched cues must be embedded inside section tags, such as `[Bridge - Quiet Contrast]` or `[Final Chorus - Final Surge, Ad-Lib Finale]`; do not emit them as standalone lyric tags.

## Files

- `song-section-tags.md`: intro, motif, verse, pre-chorus, chorus, hook, bridge, interlude, instrumental, outro, ending types.
- `movement-energy-tags.md`: slow build, rising tension, release, final surge, pulse shifts, rubato, locked groove, accelerando, ritardando.
- `texture-arrangement-tags.md`: drone beds, pedal tones, sparse percussion, full rhythm section, call and response, harmony layers, interlocking patterns, filters, noise, glitch.
- `vocal-delivery-tags.md`: spoken intros, chanted hooks, melismatic lifts, group responses, lead improvisation, harmony stacks.
- `formal-development-tags.md`: theme return, variation, expansion, compression, hard cut, fake ending, climax, cadence, subject/answer entries, overtures.
- `genre-form-tags.md`: idiomatic tags for EDM, pop, rock, metal, rap, Latin, Afro-diasporic, South Asian, East Asian, gamelan, communal, jazz, roots, and minimalist forms.
- `hybrid-movement-tags.md`: cross-genre macro-tags such as acoustic-to-electronic drops and orchestral/trap hybrids.
- `tag-superlist.md`: flattened exhaustive list for lookup.

## Routing

- Need ordinary lyrics: use `song-section-tags.md` and optionally `vocal-delivery-tags.md`.
- Need arrangement motion: use `movement-energy-tags.md` and `texture-arrangement-tags.md`.
- Need genre-specific forms: use `genre-form-tags.md`.
- Need experimental fusion: use `hybrid-movement-tags.md`.
- Need search across everything: use `tag-superlist.md`.
