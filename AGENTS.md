# Notes for AI agents working in this repository

- Each skill is one folder under `skills/<name>/` with a `SKILL.md`. The folder name must equal the `name` in the
  YAML header. Quote any header value that contains `: `.
- `plugins/liftli/skills` is GENERATED. Never edit it by hand. After changing anything under `skills/`, run
  `python3 scripts/build_liftli_plugin.py`, then `python3 scripts/build_liftli_plugin.py --check`.
- CI also runs `claude plugin validate . --strict` and `claude plugin validate ./plugins/liftli --strict`.
- When you add a skill, add its row to the matching table in `README.md`.
- Do not add anything that automates the LinkedIn website or needs an API key.
- Write plainly. No em-dashes in new text.
