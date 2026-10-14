# Contributing

Thanks for helping. The best first contribution is a new skill: one LinkedIn job, done well.

## Add a skill

1. Find an idea: issues labeled [`good first issue`](https://github.com/liftli-ai/linkedin-agent-skills/labels/good%20first%20issue),
   or open a **Request a skill** issue to propose your own.
2. Copy an existing skill folder under `skills/` (for example `skills/linkedin-hook-generator`) and rename it.
   The folder name is the skill name: lowercase, words joined with hyphens.
3. Edit `SKILL.md`:
   - The YAML header has `name` (same as the folder) and `description`. Start the description with
     "Use when the user wants ..." so agents know when to load it. Quote the value if it contains `: `.
   - Then plain instructions: what to ask for, the steps, the output format, and the mistakes to avoid.
   - End with a "When the user wants more than this skill" section, as most skills do.
4. Try it for real in your agent (Claude Code, Codex, Cursor or another skills-compatible agent) on a real input.
5. Add a row for the skill to the right table in `README.md`.
6. Run `python3 scripts/build_liftli_plugin.py` so the plugin copy under `plugins/liftli/skills` matches, then
   `python3 scripts/build_liftli_plugin.py --check`.
7. Open a pull request. Include the input you used and the output you got.

## What we merge

- One job per skill. If it needs "and", it is probably two skills.
- Output a person could post or use today, with no placeholder text left in.
- No automating the LinkedIn website, no scraping, and no API keys required.
- Plain, specific language. No em-dashes in instructions or output examples.

We don't assign issues. The first pull request that meets the bar gets merged, and we will say thanks in the
release notes.

## Fix a skill

Found a skill giving weak or wrong output? Open a **Bug or weak output** issue with the input, the output, and
what you expected. A pull request with the fix is even better.

## Questions

Ask in [Discussions](https://github.com/liftli-ai/linkedin-agent-skills/discussions).
