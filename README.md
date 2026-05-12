# Suno Songwriting Skill

Open Agent Skill for generating Suno-ready lyrics, style prompts, vocal direction, and song adaptation workflows.

This skill helps an agent write, revise, translate, and adapt song lyrics for Suno or similar AI music generators. It includes structured guidance for lyric form, genre and arrangement language, vocal identity, style prompts, translation, section tags, and generation-ready output formatting.

## What It Does

- Generates structured, singable lyrics with section labels that embed any optional performance, movement, or enriched cue tags.
- Writes compact or detailed Suno-style prompts for genre, instrumentation, production, and vocal direction.
- Revises existing lyrics while preserving intent, meter, rhyme, or emotional arc.
- Translates and localizes lyrics for singability instead of literal word-for-word output.
- Supports genre fusion, arrangement movement, vocal identity design, and AI music prompt refinement.

## Skill Layout

```text
suno-songwriting/
  SKILL.md
  agents/
  references/
```

The main skill entrypoint is `suno-songwriting/SKILL.md`. The reference files are loaded selectively by the agent when a request needs deeper genre, vocal, lyric, translation, or arrangement guidance.

## Install

Install from GitHub with the Open Agent Skills CLI:

```sh
npx skills add NuNaught/suno-songwriting-skill --skill suno-songwriting
```

Install globally so the skill is available across projects:

```sh
npx skills add NuNaught/suno-songwriting-skill --skill suno-songwriting --global
```

Install for a specific agent:

```sh
npx skills add NuNaught/suno-songwriting-skill --skill suno-songwriting --agent <agent-name>
```

Install from a local checkout:

```sh
npx skills add . --skill suno-songwriting
```

List the skills discovered in this repo without installing:

```sh
npx skills add NuNaught/suno-songwriting-skill --list
```

For non-interactive installs, add `--yes`:

```sh
npx skills add NuNaught/suno-songwriting-skill --skill suno-songwriting --global --yes
```

## Local Development

Check the package contents:

```sh
npm run pack:dry-run
```

Run the default validation:

```sh
npm test
```

## Publishing

Publish to npm:

```sh
npm publish
```

If the package name is already taken, change `name` in `package.json` or publish under an npm scope, for example:

```json
"name": "@your-scope/suno-songwriting-skill"
```

## Repository Notes

- The npm package includes `suno-songwriting/`, `README.md`, `LICENSE`, and `package.json`.
- The Skills CLI requires Node.js 18 or newer.

## License

Apache-2.0. See [LICENSE](LICENSE).
