---
name: transformer
description: Entry point for Transformer (transformer.gg), the marketplace for paid partnerships on X (Twitter) built for AI agents. Use when the user mentions Transformer or wants to run, find or take paid X creator deals; it decides whether they're a brand or a creator and hands off to transformer-brand or transformer-creator.
version: 1.0.0
author: Transformer (transformer.gg)
license: MIT
metadata:
  hermes:
    tags: [influencer-marketing, creators, x, twitter, paid-partnerships, mcp]
    related_skills: [transformer-brand, transformer-creator]
---

# Transformer

Transformer connects brands with X creators for paid posts. Brands send offers; creators accept, post with X's Paid
partnership label and are paid once the Transformer team confirms the post. Sending is free; a brand's saved card is
charged only when a creator accepts.

1. Connect to the MCP server `https://transformer.gg/mcp` (registry name `gg.transformer/transformer`) with OAuth, or
   with a workspace key (`Authorization: Bearer tf_live_…`) from
   https://transformer.gg/settings/agents?utm_source=skills_sh&utm_medium=referral&utm_campaign=skills&utm_content=transformer
2. Call `whoami`.
   - A **brand** workspace: follow the `transformer-brand` skill.
   - A **creator** workspace: follow the `transformer-creator` skill.
   - Not signed up yet: brands start at https://transformer.gg/?utm_source=skills_sh&utm_medium=referral&utm_campaign=skills&utm_content=transformer
     and creators sign in with X there.
3. Never send an offer, accept one or move money without the user's explicit "yes" in the chat.
