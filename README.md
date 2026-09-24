# LinkedIn Agent Skills

31 free skills that turn Claude Code, Codex, Cursor or any skills-compatible
agent into a LinkedIn content team. They find post ideas in your real work,
write posts, hooks and comments in your voice, fix your profile, and check
every draft before it goes out.

MIT licensed. No account, no API key, nothing phones home. Made by
[Liftli](https://liftli.ai/?utm_source=github&utm_campaign=skills-readme).
Full directory with a card per skill: [liftli.ai/skills](https://liftli.ai/skills/).

## Install

**Claude Code plugin** (all 31 skills):

```
/plugin marketplace add liftli-ai/skills
/plugin install linkedin-agent-skills@liftli
```

**Any agent**, with the [skills](https://skills.sh) CLI:

```bash
npx skills add liftli-ai/skills
```

**One skill:**

```bash
npx skills add liftli-ai/skills --skill linkedin-hook-generator
```

**By hand:** copy any folder under `skills/` into `~/.claude/skills/`, or
your agent's skills folder.

## Start here

1. Ask your agent: *"Help me with my LinkedIn."* The `linkedin-agent` skill
   picks the right skill for what you want.
2. Build your voice file. Say *"build my voice file"* and paste three posts
   you wrote. Every writing skill reads it, so drafts sound like you instead
   of like everyone else. Template: [`templates/voice.md`](templates/voice.md).
3. Write, check, then post.

## The skills

### Start

| Skill | What your agent gains |
|---|---|
| `linkedin-agent` | The front door: routes any LinkedIn request to the right skill and suggests a weekly routine |
| `linkedin-voice` | Builds your voice file from three of your posts; every writing skill reads it |
| `linkedin-publish` | Gets a final post live: a copy-ready version to paste, or publishing through Liftli |

### Write

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-hook-generator` | 8 pattern-labeled hooks sized for the "see more" fold | [tool](https://liftli.ai/tools/hook-generator.html) |
| `linkedin-post-generator` | Complete posts: hook, short paragraphs, concrete specifics, takeaway | [tool](https://liftli.ai/tools/post-generator.html) |
| `linkedin-post-rewriter` | Rewrites drafts for reach; keeps the author's facts and voice | [tool](https://liftli.ai/tools/post-rewriter.html) |
| `linkedin-post-ideas` | 15 specific ideas mined from the user's real expertise, 5 angle categories | [tool](https://liftli.ai/tools/content-ideas.html) |
| `linkedin-comment-generator` | 25–40 word replies with substance; three distinct comment types | [tool](https://liftli.ai/tools/comment-generator.html) |
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
| `ai-sounding-post-checker` | Finds AI tells, and fixes them by adding what's missing, not paraphrasing | [tool](https://liftli.ai/tools/ai-sounding-post-checker.html) |
| `hot-take-risk-check` | The uncharitable reading + minimal edits that keep the edge | [tool](https://liftli.ai/tools/hot-take-check.html) |
| `linkedin-text-formatter` | Unicode bold/italic conversion, with the accessibility caveats | [tool](https://liftli.ai/tools/text-formatter.html) |
| `linkedin-line-break-fixer` | Cleans pasted-from-Docs spacing and invisible characters | [tool](https://liftli.ai/tools/line-break-fixer.html) |

### Measure & plan

| Skill | What your agent gains | Web twin |
|---|---|---|
| `linkedin-engagement-rate` | ER formulas + honest interpretation bands | [tool](https://liftli.ai/tools/engagement-rate-calculator.html) |
| `linkedin-follower-growth` | Growth projection with honest compounding caveats | [tool](https://liftli.ai/tools/follower-growth-calculator.html) |
| `linkedin-best-time-to-post` | The honest timing answer + how to find the user's own best time | [tool](https://liftli.ai/tools/best-time-to-post.html) |
| `linkedin-ghostwriter-cost` | Prices the alternatives: human ghostwriter, DIY hours, software | [tool](https://liftli.ai/tools/ghostwriter-cost-calculator.html) |
| `linkedin-image-sizes` | Every 2026 dimension + crop rules | [tool](https://liftli.ai/tools/image-sizes.html) |

## What these skills don't do

They don't post, and no skill should. Automating the LinkedIn website breaks
LinkedIn's User Agreement and gets accounts restricted, and posting needs an
app connected to your account through LinkedIn's official API. So every
skill ends with a copy-ready post you paste yourself.

They also forget. Each chat starts from zero, apart from your voice file.

If you want your agent to publish and remember, that is what
[Liftli](https://liftli.ai/?utm_source=github&utm_campaign=skills-readme)
does. It connects to the same agent as an MCP server, learns your voice from
your real posts, keeps your strategy between sessions, drafts from what you
actually did this week, and publishes or schedules through LinkedIn's official
API only after you approve each post. Free plan (first 3 posts), no card.

```bash
claude mcp add --scope user --transport http liftli https://mcp.liftli.ai/mcp
claude mcp login liftli
```

Claude app, Codex, Cursor and other clients: [liftli.ai/llms.txt](https://liftli.ai/llms.txt).

## License

MIT. See [LICENSE](LICENSE).
