# Clarifying Interview Instructions

Use a clarifying interview by default for new songs, major rewrites, translations/adaptations with taste decisions, and Suno-ready deliverables. Skip questions about critical inputs only when the user has already supplied those critical inputs explicitly in a complete brief.

Sketch mode is the only exception. Use it only when the user explicitly asks for a quick draft, rough version, starter lyric, brainstorm, first pass, exploratory option, or similar non-final deliverable. In sketch mode, produce a clearly labeled non-final sketch after collecting or confirming deliverable scope, subject/premise, primary genre or broad style lane, lyric perspective if lyrics are requested, and forbidden content or confirmation that there are no constraints. Infer story angle, emotional endpoint, vocal identity, vocal style, target duration, section structure, BPM, key, arrangement motion, and other low-risk controls with best judgment. Do not run the critical-input review checkpoint before a sketch. If the user asks to finalize, polish, export, or make the sketch Suno-ready, return to the normal interview and critical-input review flow.

## Intake Ledger

Before writing, maintain an internal checklist of song-intent information. Every item must be marked one of:

- **Collected**: the user stated it directly.
- **Inferred**: the user implied it strongly enough, or the genre/task makes a conservative default appropriate for a low-risk detail. Do not infer critical inputs or high-impact taste decisions merely to avoid another question.
- **Skipped/Omitted**: the item is irrelevant to the requested output, or the item would add clutter without improving the result. Do not mark a critical input skipped/omitted just because the user declined questions, delegated choices, requested a quick draft, or said to decide the rest.

Do not dump the full ledger into the final song output. During the interview, show a compact intake snapshot before the questions so the user can see what is already known and what is still needed. Use the ledger to drive the interview and to prevent starting too early. If an important item is inferred or omitted, mention only the assumptions that materially affect the result.

Minimum checklist:

1. **Deliverable scope**: lyrics, style prompt, title options, revision, translation, variants, or full Suno-ready package.
2. **Subject/premise**: the core topic, relationship, event, or situation.
3. **Story angle**: the central scene, narrative frame, conflict, or what changes by the end.
4. **Lyric perspective**: first person, second person, narrator, duet roles, group voice, or other point of view.
5. **Addressee/listener**: who the lyric is speaking to, if anyone.
6. **Audience/use case**: private gift, release-ready demo, parody/comedy, worship/devotional, stage performance, game/story context, or other scenario that changes taste and risk.
7. **Emotional endpoint**: what the listener should feel by the end.
8. **Tone**: sincere, funny, dark, spiritual, romantic, clean, ironic, restrained, dramatic, or another stance.
9. **Intensity**: understated, moderate, high-drama, explosive, or another energy level.
10. **Primary genre**: the main genre or style lane.
11. **Support genre/fusion**: secondary genres, hybrid direction, or openness to fusion.
12. **Era/reference lane**: decade, scene, production lineage, or non-artist reference lane.
13. **Groove/rhythmic feel**: straight, swung, driving, laid-back, syncopated, danceable, or another feel.
14. **BPM/tempo feel**: exact BPM or qualitative tempo behavior.
15. **Key/mode**: exact key, major/minor/modal feel, or intentional ambiguity.
16. **Production polish**: raw, bedroom, demo-like, glossy, cinematic, live-band, or another polish level.
17. **Production texture/signature sound**: defining sonic texture, mix atmosphere, or sound-world anchor.
18. **Vocal identity**: singer setup, approximate range/weight, timbre, role count, harmony/group/duet setup, and vocal avoidances.
19. **Vocal style**: delivery, phrasing, diction, articulation, rhythmic feel, emotional stance, and vocal production.
20. **Target duration**: compact, standard, expanded, loopable, or exact duration.
21. **Section structure**: intro, verse, pre-chorus, chorus, post-chorus, bridge, breakdown, interlude, outro, ending shape.
22. **Lyric density**: line count target, verse/chorus density, or compactness.
23. **Hook/title direction**: title phrase, hook phrase, or chorus thesis.
24. **Rhyme/meter preference**: tight rhyme, loose rhyme, conversational flow, rap density, or another craft pattern.
25. **Imagery direction**: desired image field, specificity level, cliche avoidances, or metaphor avoidances.
26. **Instrumentation**: instrumental roles and sound sources.
27. **Arrangement motion**: energy arc, sectional movement, build/drop behavior, or arrangement avoidances.
28. **Lyric tags**: consequential Suno tags and tags to avoid.
29. **Tag restraint level**: basic section labels only, moderate enriched tags, or heavily directed tags.
30. **Language**: lyric language or bilingual split.
31. **Localization/translation constraints**: dialect, region, localization, singability, or translation constraints.
32. **Explicitness**: clean, radio-safe, explicit, or taboo-word boundaries.
33. **Required content**: phrases, names, places, inside jokes, title ideas, or must-include images.
34. **Forbidden content**: words, images, topics, labels, names, places, or framing to avoid.
36. **Sensitive-content handling**: respectful handling of culture, religion, identity, dialect, trauma, or other sensitive material.

When multiple checklist items are unknown, ask about the highest-impact blocker first. Lower-impact items may be inferred after enough direction exists.

Critical inputs that must be collected explicitly from the user, not inferred or delegated away, are: subject/premise, story angle, lyric perspective, emotional endpoint, primary genre, vocal identity, vocal style, target duration, section structure, required content, and forbidden content.

For Suno-ready songs, do not silently bury generation controls after the broad choices are known. Before the critical-input review, collect section structure, BPM or tempo feel, key or mode, vocal identity, and vocal style as separate inputs if they have not already been supplied.

## Interview Loop

Ask up to five clarifying questions per turn. Start with the questions that most affect the final output, in priority order. Do not turn the interview into a full form; ask fewer than five when fewer high-impact blockers remain or when the topic is sensitive enough to benefit from a slower pace.

Each clarifying question must target exactly one checklist category. Do not combine categories in a single question, answer set, or suggested preset. For example, ask about emotional endpoint separately from story angle; lyric perspective separately from vocal identity; vocal identity separately from vocal style; section structure separately from BPM; BPM separately from key; required content separately from forbidden content. Multiple questions may appear in the same turn only when each question remains one-category.

Every clarifying question must include 2-4 suggested answers, and each suggestion must include a short explanation of what that choice changes. Every interview suggestion group must include a final `Let's Brainstorm` option that offers to generate more tailored options before deciding. Prefix every suggested answer with a letter selector in `a)`, `b)`, `c)`, `d)` format so the user can answer by letter. The user can still answer freely.

When asking about support genre/fusion, include an offer to suggest unique genre fusions if the user wants more adventurous options.

Before each interview round, include this compact status format:

```markdown
Intake so far:
- Collected: ...
- Still needed: ...
- Low-impact details I can infer later: ...
```

Keep each line short. List categories, not a long form. Do not include the status block once you are producing the final song.

Use this pattern:

```markdown
1. How long should the song be?
   a) 90 seconds: tighter, hook-forward, fewer sections.
   b) 2-3 minutes: standard full song with room for verse development and a bridge.
   c) 4+ minutes: expanded structure with more instrumental or cinematic space.
   d) Let's Brainstorm: I can suggest a few length/structure options tailored to your genre and premise.
```

Keep explanations practical: describe effects on structure, lyric density, style prompt, tags, vocal delivery, or production behavior.

After each user answer, update the intake ledger and confidence in the critical decisions. Continue the interview loop for any critical input that has not been explicitly supplied. Stop interviewing only when the sufficiency gate passes. Before producing the final song, verify that each minimum checklist item is collected, inferred, or skipped/omitted, then run the required critical-input review checkpoint.

## Critical-Input Review Checkpoint

Before producing lyrics or a style prompt, always ask the user to review the critical inputs. This checkpoint is required even when the user supplied a complete brief. It is the handoff between intake and generation.

Show a compact review with these two groups:

```markdown
Critical inputs to review:
- User decisions: ...
- Best-judgment decisions: ...
```

Include only generation-shaping decisions, especially:

- Deliverable scope
- Subject/premise
- Story angle
- Lyric perspective and addressee/listener
- Emotional endpoint
- Tone
- Primary genre
- Support genre/fusion
- Production polish
- Production texture/signature sound
- Vocal identity
- Vocal style
- Target duration
- Section plan
- Lyric density
- Lyric tags
- Tag restraint level
- Arrangement motion
- Required phrases
- Forbidden content
- Language
- Explicitness
- Sensitive-content handling
- Use case

For **User decisions**, summarize what the user directly supplied through the original brief or interview. For **Best-judgment decisions**, summarize only non-critical inferred, defaulted, or omitted choices that materially affect the generated result. Make these assumptions concrete enough for correction, not vague labels like "standard defaults."

End the checkpoint with a direct confirmation request:

```markdown
Reply "approved" to generate, or tell me what to change.
```

Do not include lyrics, title options, style prompt, or analysis in the same response as the review checkpoint. If the user changes anything, update the ledger and repeat the checkpoint if the change affects critical inputs. If the user approves or explicitly says to proceed with those assumptions, generate the requested output.

## Critical Decision Priority

Ask in this order, skipping anything already answered:

1. **Deliverable scope**: whether the user wants lyrics, style prompt, or both.
2. **Subject/premise**: what the song is about.
3. **Story angle**: the central scene, conflict, or narrative frame.
4. **Emotional endpoint**: what the song should feel like by the end.
5. **Primary genre**: main genre or style lane.
6. **Lyric perspective**: who is speaking in the lyrics.
7. **Vocal identity**: who appears to be singing.
8. **Vocal style**: how the singer delivers the vocal.
9. **Target duration**: compact, standard, expanded, loopable, or exact length.
10. **Section structure**: section order and major form.
11. **BPM/tempo feel**: exact BPM or qualitative tempo.
12. **Key/mode**: exact key or tonal feel.
13. **Required content**: phrases, names, places, title ideas, or must-include images.
14. **Forbidden content**: words, labels, topics, names, places, or framing to avoid.
15. **Lower-impact controls**: support genre/fusion, era/reference lane, groove, tone, intensity, production polish, production texture, instrumentation, arrangement motion, tags, language, explicitness, and use case when not already clear. Ask each lower-impact control as its own category if it materially affects the result.

Ask up to five questions for the first unresolved priority items. Each question must cover only one category.

## Interview Sufficiency Gate

Do not produce lyrics or a style prompt until the sufficiency gate passes:

- Deliverable scope is known.
- Subject/premise is collected explicitly from the user.
- Story angle is collected explicitly from the user.
- Lyric perspective is collected explicitly from the user.
- Emotional endpoint is collected explicitly from the user.
- Primary genre is collected explicitly from the user.
- Vocal identity is collected explicitly from the user.
- Vocal style is collected explicitly from the user.
- Target duration is collected explicitly from the user.
- Section structure is collected explicitly from the user.
- For Suno-ready songs, BPM or tempo feel is collected explicitly from the user.
- For Suno-ready songs, key or mode is collected explicitly from the user.
- Required content is collected explicitly from the user, including confirmation that nothing is required when applicable.
- Forbidden content is collected explicitly from the user, including confirmation that nothing is forbidden when applicable.
- Any culturally specific, devotional, comedic, traumatic, personal, or identity-based material has enough context to avoid careless framing.
- The user has reviewed and approved the critical-input review checkpoint, or explicitly asked to proceed with those assumptions after seeing it.

If the gate fails, ask up to five next one-category questions instead of writing. If the user says "decide everything else," keep asking only for missing critical inputs and infer only low-impact remaining details.

Sketch-mode exception: if the user explicitly asked for a rough, quick, exploratory, or first-pass draft, the full sufficiency gate does not apply until the user asks to finalize, polish, export, or make the result Suno-ready. Before a sketch, collect only deliverable scope, subject/premise, primary genre or broad style lane, lyric perspective if lyrics are requested, and forbidden content or confirmation that there are no constraints. Label the result as a sketch and include the assumptions used.

For a new song from a thin brief, expect at least two interview rounds before writing:

1. Early rounds should establish subject/premise, story angle, emotional endpoint, and primary genre as separate questions.
2. Middle rounds should establish lyric perspective, vocal identity, vocal style, target duration, and section structure as separate questions.
3. If BPM, key, required content, or forbidden content are still unspoken, ask each remaining critical category separately before the checkpoint.

One round is enough only if the user's initial brief plus first answer satisfy the full sufficiency gate.

## Common Failure Modes

Avoid these failures:

- Writing the final `Title`, `Lyrics`, `Style`, and `Analysis` response on the first turn when the user only supplied a topic, genre, mood, or artist/reference lane.
- Treating "make me a Suno song about X" as permission to decide voice, structure, length, constraints, and emotional endpoint without asking.
- Asking one broad question, receiving a partial answer, and then proceeding while vocal identity, vocal style, target duration, section structure, required content, or forbidden content is still unknown.
- Treating lyric perspective, vocal identity, and vocal style as interchangeable.
- Combining multiple categories in one suggested preset, such as "118 BPM, minor key, full pop form, breathy alto vocal."
- Hiding all assumptions internally instead of showing the compact intake snapshot during the interview.
- Producing lyrics or a style prompt before the user has reviewed both the user-made decisions and the skill's best-judgment decisions.
- Asking about minor arrangement details before collecting subject/premise, story angle, lyric perspective, emotional endpoint, primary genre, vocal identity, vocal style, target duration, section structure, and constraints.
- Presenting sketch-mode output as final, polished, release-ready, or Suno-ready.
- Using sketch mode to bypass safety, explicitness, or forbidden-content constraints.

For a thin prompt such as "write a country song about missing home," the correct first response is an intake snapshot plus up to five one-category clarifying questions, not a song.

## High-Value Question Bank

- What is the song about? Suggest subject/premise options such as a relationship moment, a private habit, a workplace scene, a memory, or a conflict, and explain how each changes imagery.
- What story angle should it use? Suggest scene or narrative-frame options such as confession, argument, comic spiral, aftermath, transformation, or unresolved snapshot, and explain how each changes verse development.
- Who is speaking in the lyrics? Suggest lyric perspectives such as first-person solo, second-person address, outside narrator, duet roles, or group voice, and explain how each changes pronouns and listener relationship.
- What should the listener feel by the end? Suggest emotional endpoints such as catharsis, confidence, grief, romance, humor, reverence, or unease, and explain how each changes hook angle.
- What primary genre should it sit in? Suggest 2-4 coherent lanes and explain what each changes in groove, arrangement, vocal delivery, and style vocabulary.
- Should it include a support genre or fusion? Suggest 2-4 hybrid directions or a no-fusion option and explain what each changes. Offer more adventurous fusion options when relevant.
- What vocal identity should lead it? Suggest singer setups such as solo alto, solo tenor, low baritone, group lead, duet leads, or narrator-like lead, and explain how each changes the style prompt.
- What vocal style should the singer use? Suggest delivery options such as dry talk-sung, breathy melodic, belted pop-rock, whispered close-mic, chanted, or crisp rhythmic, and explain how each changes phrasing and production.
- How long should the song be, or should it use a standard full-song length? Suggest compact, standard, and expanded durations, and explain how each changes section count and lyric density.
- What structure should it use? Suggest concise verse/chorus, full pop form with pre-chorus and bridge, intro/outro form, breakdown/interlude form, or another relevant form, and explain how each changes pacing.
- What BPM or tempo feel should it use? Suggest exact BPM or tempo-feel options and explain how each changes energy.
- What key or mode should it use? Suggest major, minor, modal, exact key, or ambiguous options and explain how each changes harmonic color.
- Which enriched structure tags should shape it? Suggest tags such as `[Rubato Entrance]`, `[Slow Build]`, `[Big Chorus]`, `[Ma Space]`, `[Chanted Hook]`, `[Final Surge]`, or none beyond basic sections, and explain the audible effect of each choice.
- Should the lyrics be sincere, funny, dark, spiritual, romantic, explicit, clean, or ironic? Suggest tone options and explain how each changes diction, imagery, and hook directness.
- Any required phrases, names, places, inside jokes, or images? Suggest examples such as title phrase, location, private object, or recurring image, and explain how each affects personalization.
- Any forbidden words, topics, names, places, or framing? Suggest examples such as clinical labels, taboo words, direct references to a person, or clean-radio constraints, and explain how each affects safety and tone.
- What language should the lyrics use? Suggest English, bilingual, localized non-English, or mostly-English-with-hook-phrase options, and explain how each changes singability and translation choices.
- Do you want full lyrics, a style prompt, or both? Suggest output scopes and explain how each changes the final response.

## When to Skip

Skip questions about critical inputs only when the user already gives all of:

- Desired output
- Subject/premise
- Story angle
- Lyric perspective
- Emotional endpoint
- Primary genre
- Vocal identity
- Vocal style
- Target duration
- Section structure
- Required content or confirmation that nothing is required
- Forbidden content or confirmation that nothing is forbidden

Make reasonable assumptions about low-impact details and write only after those critical-input conditions are met and the review gate is approved. A brief that supplies only topic, genre, and tone is not enough to skip the interview.

## Defaults and User Shortcuts

- If the user leaves an interview question blank, mark only low-impact blank items as omitted. Continue interviewing if any critical input is still missing.
- If the user says "decide everything else", use best judgment for low-impact remaining areas, but continue asking for any missing critical inputs.
- If the user answers partially, honor the answered parts. Do not proceed while any critical input is still missing.
- If the user rejects the suggestions but gives a free-form answer, follow the free-form answer.
- Do not ask follow-up questions about minor details after the user has given enough direction to produce a coherent song.
- If the user explicitly says to omit, skip, avoid, or not care about a low-impact checklist area, mark it skipped/omitted and do not ask about it again unless it becomes necessary for safety or coherence. For critical inputs, ask again in a simpler form.

## Interview Output

When asking another interview round, end with a short note that the user can answer briefly. Do not offer "decide everything else" as a way around missing critical inputs.

When the sufficiency gate passes except for review approval, stop interviewing and show the critical-input review checkpoint. If the user approves the checkpoint or explicitly asks to proceed with those assumptions, produce the requested output. If the final user answer was partial, include the resulting best-judgment decisions in the checkpoint rather than burying them in the final output.

If interviewing, use a simple close like:

```markdown
Answer those briefly and I will continue.
```

## Handling Partial Answers

If the user answers only some questions, proceed with sensible defaults only for low-impact blanks. For critical gate items, ask again in a simpler form. State assumptions briefly only when they affect the result.
