# Working rules for Claude on the Afritech Sports home site

## robots.txt (Andrew, 26 Nov 2026, Gatekeeper 1D)
- `robots.txt` at the root of this repository is the only one that works for every Afritech Sports site on afritech-advisory.github.io (home site and project sites such as the Tournament Desk). Project sites' own copies have no effect.
- Every change keeps the full list: the AI crawlers (GPTBot, ChatGPT-User, CCBot, ClaudeBot, anthropic-ai, Google-Extended, Applebot-Extended, PerplexityBot, Bytespider, Meta-ExternalAgent, Amazonbot, cohere-ai) and the SEO-tool crawlers (AhrefsBot, SemrushBot, MJ12bot, DotBot, PetalBot) stay `Disallow: /`; everyone else `Allow: /`.
- Never replace this file with another repository's copy. Add lines instead: a new project site adds its own `Sitemap:` line here.
- The Tournament Desk keeps a matching copy of this file in its own repository, so change both in the same session.
