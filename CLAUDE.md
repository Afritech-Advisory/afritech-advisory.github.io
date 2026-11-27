# Working rules for Claude on the Afritech Sports home site

## robots.txt (Andrew, 26 Nov 2026, Gatekeeper 1D)
- `robots.txt` at the root of this repository is the only one that works for every site on afritech-advisory.github.io (project sites such as the Tournament Desk). Project sites' own copies have no effect.
- The Afritech Sports home site is a different address, afritechsports.github.io (repo AfritechSports/afritechsports.github.io, built from its `source` branch). It has its own robots.txt, written by its build.py, and must carry the same blocked list. This repository's root page only forwards to it, so it has no sitemap of its own.
- Every change keeps the full list: the AI crawlers (GPTBot, ChatGPT-User, CCBot, ClaudeBot, anthropic-ai, Google-Extended, Applebot-Extended, PerplexityBot, Bytespider, Meta-ExternalAgent, Amazonbot, cohere-ai) and the SEO-tool crawlers (AhrefsBot, SemrushBot, MJ12bot, DotBot, PetalBot) stay `Disallow: /`; everyone else `Allow: /`.
- Never replace this file with another repository's copy. Add lines instead: a new project site adds its own `Sitemap:` line here.
- The Tournament Desk keeps a matching copy of this file in its own repository, so change both in the same session.
