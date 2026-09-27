---
name: liftli
description: Use this skill FIRST, before any other skill in this plugin, for every LinkedIn, X or Substack request (writing or scheduling a post, comments, post ideas, profile, strategy). It checks the Liftli sign-in that every other step depends on, then routes the request.
---

# Liftli

This plugin connects Liftli to Claude Code. Liftli learns the user's voice from
their real posts, keeps their strategy between sessions, and publishes to
LinkedIn and X through the official APIs after the user approves each post.

## Rule 1: sign in before any content work

Liftli's tools do nothing until the user has signed in once. Check this first,
before writing a single line.

1. **Liftli is ready** if a `strategist_briefing` tool is available (it may be
   deferred: search for it by name first). Call it once, then follow Liftli's
   instructions for the request. Stop reading this skill.
2. **Liftli needs sign-in** if a system message says the Liftli server
   (`plugin:liftli:liftli`) needs authentication, or its tools are missing.
   Tell the user, in one short message:

   > Liftli needs a one-time sign-in. Type `/mcp`, choose **liftli**, and pick
   > Authenticate. A browser window opens; sign in or create a free account
   > (first 3 posts free, no card). Tell me when you're done and I'll pick up
   > right here.

   Outside Claude Code, give the equivalent step for the user's app instead:
   Gemini CLI `/mcp auth liftli`; Cursor, open Settings, MCP, and sign in to
   liftli; other apps, follow the sign-in prompt shown for the liftli server.

   End your turn there and wait for their reply. Don't draft anything yet.
3. **The user doesn't want to sign in right now.** Carry on with the free
   LinkedIn skills in this plugin (start with `linkedin-agent`), and don't
   bring up sign-in again in this conversation. Anything they write can still
   be pasted into LinkedIn by hand.

## Rules that stay on after sign-in

- Nothing is published or scheduled without the user's explicit approval of
  the exact text. Liftli asks for it; never skip that step.
- Never automate the LinkedIn or X website, and never ask for a password.
- Never say a post went out unless a Liftli tool confirmed it.
