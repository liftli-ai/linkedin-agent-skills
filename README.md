# Liftli Skills — LinkedIn & content tools for AI agents

Free, installable skills that turn any AI agent (Claude Code, Cursor, or any
[skills](https://skills.sh)-compatible client) into a working LinkedIn content
assistant. Each skill is a distilled, battle-tested methodology — your agent's
own model does the work, entirely locally. No API keys, no accounts, nothing
phones home.

Built by [Liftli](https://liftli.ai) — the content engine that runs inside the
AI you already use. Every skill here also exists as a free web tool at
[liftli.ai/tools](https://liftli.ai/tools/), and the full skill directory with
per-skill install commands lives at [liftli.ai/skills](https://liftli.ai/skills/)
(machine-readable manifest: [liftli.ai/.well-known/skills](https://liftli.ai/.well-known/skills)).

## Install

The whole collection:

```bash
npx skills add liftli-ai/skills
```

Or a single skill:

```bash
npx skills add liftli-ai/skills --skill linkedin-hook-generator
```

## The skills

### Write

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-hook-generator` | 8 pattern-labeled hooks sized for the "see more" fold | [tool](https://liftli.ai/tools/hook-generator.html) |
| `linkedin-post-generator` | Complete posts: hook, short paragraphs, concrete specifics, takeaway | [tool](https://liftli.ai/tools/post-generator.html) |
| `linkedin-post-rewriter` | Rewrites drafts for reach; keeps the author's facts and voice | [tool](https://liftli.ai/tools/post-rewriter.html) |
| `linkedin-post-ideas` | 15 specific ideas mined from the user's real expertise, 5 angle categories | [tool](https://liftli.ai/tools/content-ideas.html) |
| `linkedin-comment-generator` | 25–40 word replies with substance; five distinct comment types | [tool](https://liftli.ai/tools/comment-generator.html) |
| `linkedin-carousel-outline` | Slide-by-slide carousel structure (one idea per slide, <25 words) | [tool](https://liftli.ai/tools/carousel-outline.html) |
| `linkedin-poll-generator` | Polls people answer: question ≤140 chars, options ≤30, opinionated intro | [tool](https://liftli.ai/tools/poll-generator.html) |
| `linkedin-to-x` | Converts LinkedIn posts to X properly: standalone, thread, quote-bait | [tool](https://liftli.ai/tools/linkedin-to-x.html) |
| `linkedin-contrarian-takes` | 6 defensible contrarian angles, steelman included | [tool](https://liftli.ai/tools/contrarian-angles.html) |
| `devlog-to-linkedin-post` | Commits / PR titles → build-in-public post (story, not changelog) | [tool](https://liftli.ai/tools/devlog-to-post.html) |
| `meeting-notes-to-linkedin-post` | Call notes → anonymized insight post | [tool](https://liftli.ai/tools/meeting-to-post.html) |

### Profile

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-headline-generator` | 7 headline formulas under 220 chars, front-loaded for search | [tool](https://liftli.ai/tools/headline-generator.html) |
| `linkedin-headline-analyzer` | Scores a headline: front-load, buzzwords, pipe soup, audience signal | [tool](https://liftli.ai/tools/headline-analyzer.html) |
| `linkedin-about-generator` | About sections that read like landing pages, not bios | [tool](https://liftli.ai/tools/about-generator.html) |
| `linkedin-profile-checklist` | 25-point profile audit with weighted scoring | [tool](https://liftli.ai/tools/profile-checker.html) |
| `ai-search-visibility` | GEO audit for a person: is the user citable by ChatGPT/Claude/Perplexity? | [tool](https://liftli.ai/tools/ai-visibility-checker.html) |

### Check before posting

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-character-limits` | Every 2026 limit + the fold rules, for length checks in the terminal | [tool](https://liftli.ai/tools/character-counter.html) |
| `linkedin-post-preview` | Computes exactly what survives the desktop/mobile fold | [tool](https://liftli.ai/tools/post-preview.html) |
| `linkedin-post-analyzer` | 10-point pre-publish score (editorial best practices, honestly framed) | [tool](https://liftli.ai/tools/post-analyzer.html) |
| `ai-sounding-post-checker` | Finds AI tells — and fixes them by adding what's missing, not paraphrasing | [tool](https://liftli.ai/tools/ai-sounding-post-checker.html) |
| `hot-take-risk-check` | The uncharitable reading + minimal edits that keep the edge | [tool](https://liftli.ai/tools/hot-take-check.html) |
| `linkedin-text-formatter` | Unicode bold/italic conversion — with the accessibility caveats | [tool](https://liftli.ai/tools/text-formatter.html) |
| `linkedin-line-break-fixer` | Cleans pasted-from-Docs spacing and invisible characters | [tool](https://liftli.ai/tools/line-break-fixer.html) |

### Measure & plan

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-engagement-rate` | ER formulas + honest interpretation bands | [tool](https://liftli.ai/tools/engagement-rate-calculator.html) |
| `linkedin-follower-growth` | Growth projection with honest compounding caveats | [tool](https://liftli.ai/tools/follower-growth-calculator.html) |
| `linkedin-best-time-to-post` | The honest timing answer + how to find the user's own best time | [tool](https://liftli.ai/tools/best-time-to-post.html) |
| `linkedin-ghostwriter-cost` | Prices the alternatives: human ghostwriter, DIY hours, software | [tool](https://liftli.ai/tools/ghostwriter-cost-calculator.html) |
| `linkedin-image-sizes` | Every 2026 dimension + crop rules | [tool](https://liftli.ai/tools/image-sizes.html) |

## Skills vs. the full pipeline

These skills are single-serving: they carry the methodology, your agent brings
the model. What they don't have is *the user's* context — their voice, their
strategy, their material, their posting history.

That's [Liftli](https://liftli.ai): an MCP connector for the AI you already use
(Claude today; ChatGPT & Cursor next) that extracts your writing voice from
your real posts, mines your voice notes / call transcripts / GitHub activity
for post material, drafts in your voice, remembers your strategy, and publishes
to LinkedIn, X and Substack — behind a one-tap approval gate. Nothing ships
without you. Free tier, no card: [liftli.ai](https://liftli.ai) · agent-readable
details: [liftli.ai/llms.txt](https://liftli.ai/llms.txt).

## License

MIT — see [LICENSE](LICENSE).
