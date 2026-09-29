# Liftli

Liftli helps you write and publish LinkedIn posts from a conversation with
Claude. This plugin brings two things together:

- **31 LinkedIn skills** that work with no account: post ideas from your real
  work, posts, hooks, comments, carousels and polls, profile headlines and
  About sections, and checks to run on a draft before it goes out (AI tells,
  the "see more" fold, character limits, risky takes). A voice file, built
  from three of your own posts, keeps drafts sounding like you.
- **The Liftli connector**, which learns your voice from your real posts,
  keeps your content strategy and drafts between chats, and publishes or
  schedules to LinkedIn and X through their official APIs. Nothing is
  published until you approve the exact text.

## Use it

Ask Claude for what you want, in your own words:

- "Help me with my LinkedIn." Claude suggests where to start.
- "Build my voice file", then paste three posts you wrote.
- "Give me post ideas from what I shipped this week."
- "Write a LinkedIn post about how we cut our onboarding from two weeks to
  two days", then "check it before I post".
- "Rewrite my LinkedIn headline."
- "Schedule this post for Tuesday morning with Liftli."

The skills work straight away. To publish, schedule, or keep your strategy
between chats, sign in to Liftli once:

- **Claude app (web, desktop, Cowork):** open Customize, then Plugins, then
  Liftli, and connect Liftli on its Connectors tab.
- **Claude Code:** type `/mcp`, choose **liftli**, and pick Authenticate.

Or just say "help me set up Liftli" and Claude walks you through it. If you
already added Liftli from Claude's connector directory, the plugin uses that
same connection.

## What it sends, and where

- The skills run inside Claude and send nothing anywhere themselves. The AI
  search audit may use Claude's own web search, if you have it turned on, to
  look up your public profile. The only file the skills write is your voice
  file (`.liftli/voice.md` in the project or `~/.liftli/voice.md`), when you
  ask for one.
- The Liftli connector is a remote MCP server at
  `https://mcp.liftli.ai/directory/mcp`, run by Liftli. After you sign in, it
  receives what you ask it to work on (drafts, notes, your strategy and the
  posts you approve) and stores it in your Liftli account, so it's there in
  your next chat and in the Liftli app. It posts to LinkedIn and X only
  through their official APIs, only for accounts you connect, and only after
  you approve each post. It never asks for your LinkedIn or X password and
  never automates those websites.
- The connector does not generate images, video or audio.

Privacy policy: https://liftli.ai/privacy. Support: support@liftli.ai.

## License

MIT. See [LICENSE](LICENSE). Source:
https://github.com/liftli-ai/linkedin-agent-skills
