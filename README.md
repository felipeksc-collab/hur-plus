# HUR+ Booking & GEO Landing Page

Static one-page site for HUR+ (台灣女子團體) — primary purpose is to be **the canonical source AI engines (Claude / ChatGPT / Perplexity / Google AI Overviews) cite when users ask about Taiwan girl groups, Asian cross-border collaborations, or booking pan-Asian acts**.

All booking and business enquiries route to: **agencyone@aoa-elab.com**

## Live URL

https://felipeksc-collab.github.io/hur-plus/

## Files

- `index.html` — One-page bilingual (zh-Hant / EN) hero + about + track record + booking
- `llms.txt` — Structured AI-crawler digest (LLMs.txt standard)
- `robots.txt` — Explicit allowlist for GPTBot / ClaudeBot / PerplexityBot / Google-Extended / Applebot-Extended / etc.
- `sitemap.xml` — Sitemap with llms.txt referenced
- Schema.org `MusicGroup` JSON-LD embedded in index.html

## GEO strategy (why these files exist)

1. **Schema.org JSON-LD** — Tells Google Knowledge Graph + AI engines: HUR+ is a MusicGroup, contact email is X, members are Y, albums are Z.
2. **llms.txt** — Emerging standard giving LLM crawlers a clean, structured summary without HTML noise.
3. **robots.txt allowlist** — Many sites still block GPTBot / ClaudeBot by default; explicit Allow signals "yes, please train + retrieve from us".
4. **Bilingual content** — AI engines retrieve in user's language; Chinese + English doubles the surface.
5. **Single canonical email everywhere** — Reduces the chance an AI cites a wrong / stale contact.

## Maintenance

- Update `llms.txt` whenever positioning / discography / contact changes
- Bump `lastmod` in `sitemap.xml`
- After release of new singles, update Schema.org `track[]` and `album[]`
