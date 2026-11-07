<p align="center">
  <img src="assets/icon.png" alt="Transformer" width="72">
</p>

# Transformer skills

[![skills.sh](https://skills.sh/b/transformer-gg/skills)](https://skills.sh/transformer-gg/skills)

Agent skills for [Transformer](https://transformer.gg/?utm_source=skills_sh&utm_medium=referral&utm_campaign=skills&utm_content=readme),
the marketplace for paid partnerships on X (Twitter), built for AI agents. Brands send X creators offers for one post;
creators accept, post in their own words with X's Paid partnership label on, and are paid once the Transformer team
confirms the post. Sending is free; a brand's saved card is charged only when a creator accepts.

| Skill | For | What it does |
| --- | --- | --- |
| [`transformer-brand`](skills/transformer-brand/SKILL.md) | Brands | Find X creators, send offers at their usual price, track offers, handle counters, approve posts, see spend |
| [`transformer-creator`](skills/transformer-creator/SKILL.md) | Creators | Set your usual price, see offers, accept, decline or counter, submit your post, check your balance, request a payout |
| [`transformer`](skills/transformer/SKILL.md) | Either | Works out whether you're a brand or a creator and hands off |

The skills never send an offer, accept one or move money without your "yes" in the chat.

## Install

```bash
npx skills add transformer-gg/skills
```

One skill, one agent:

```bash
npx skills add transformer-gg/skills --skill transformer-brand -a claude-code
```

Hermes Agent:

```bash
hermes skills tap add transformer-gg/skills
```

## Connect

The skills use Transformer's MCP server, `https://transformer.gg/mcp` (streamable HTTP; listed in the MCP Registry as
`gg.transformer/transformer`).

- Clients with OAuth sign in on transformer.gg and pick a workspace.
- Headless agents use a workspace key (`Authorization: Bearer tf_live_…`) from
  [Settings → Agents](https://transformer.gg/settings/agents?utm_source=skills_sh&utm_medium=referral&utm_campaign=skills&utm_content=readme).
- Docs: [transformer.gg/docs](https://transformer.gg/docs?utm_source=skills_sh&utm_medium=referral&utm_campaign=skills&utm_content=readme#mcp)

Questions: support@transformer.gg

---

This repository is a published mirror. The skills are maintained with Transformer's product code and synced here
automatically on every change, checked against the live MCP tools, so please don't open pull requests here. Report
problems in [Issues](https://github.com/transformer-gg/skills/issues) or at support@transformer.gg.
