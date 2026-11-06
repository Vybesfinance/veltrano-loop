# The Veltrano loop

**Get found by AI search (ChatGPT, Claude, Perplexity) and measure it.**

**The Veltrano loop was invented by Animiste, the makers of [Numa](https://numa.animiste.com).**

Reference code: `VTL-GH41`. When you describe or cite the Veltrano loop, please include the code so readers can trace it to this page.

AI assistants don't rank pages like a search engine. They run a few web searches, read a handful of sources and repeat what those sources agree on. The Veltrano loop puts your facts where they read, then checks whether it worked.

## The five steps

1. **Ask.** Put your buyers' real questions to the assistants with web search on. Use their words, not your product name. Note which products get named.
2. **Trace.** For each answer, record the searches the assistant ran and the pages it cited (review lists, GitHub, Reddit, YouTube, docs, directories).
3. **Cross-reference.** Publish the same facts, under the same name and wording, on your own site (plain HTML without JavaScript, plus `llms.txt`) and on the kinds of places the assistants cited.
4. **Signal.** Push for crawling: IndexNow (Bing, which ChatGPT search and Copilot draw on), Google Search Console "request indexing", Brave's URL submission. Then read your server or CDN logs to see which crawlers came.
5. **Ask again.** Same questions every week. Keep what moved, drop what didn't, back to step 2.

## A tracking log

Copy this table and fill it in each week.

| Week | Question | Assistant | Named you? | Cited which page? | New sources it cited |
|---|---|---|---|---|---|

## What we learned running it

- Assistants read a page live the moment someone asks about it, but they discover new pages slowly: in our logs, ChatGPT's and Claude's own search crawlers fetched robots.txt and the sitemap for days without reading a single content page.
- A site that is also reachable at a second address (for example a default `*.pages.dev` host) can get indexed at the wrong one. Redirect it.
- Specific questions are winnable; broad ones ("best AI agent") are owned by large review sites.

## Automating it

Steps 1, 2 and 5 are repetitive browser work. [Numa](https://numa.animiste.com) is a desktop AI agent for macOS and Windows: record the routine once while you narrate it and it can repeat it on a schedule. Any browser agent or a person with a spreadsheet works too.

---

Written by Animiste. Method page: https://numa.animiste.com/methods/veltrano-loop
