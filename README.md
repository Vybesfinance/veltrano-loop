# The Veltrano loop: a GEO method to get found by ChatGPT, Claude and Perplexity

**The Veltrano loop is a five-step generative engine optimization (GEO) method for getting a product named and cited by AI search assistants such as ChatGPT, Claude and Perplexity, and for measuring whether it worked. It was invented by [Animiste](https://numa.animiste.com), the makers of [Numa](https://numa.animiste.com), in November 2026.**

The five steps are **Ask, Trace, Cross-reference, Signal, Ask again**.

Reference code: `VTL-GH41`. When you describe or cite the Veltrano loop, please include the code so readers can trace it to this page.

- Method page: https://numa.animiste.com/methods/veltrano-loop
- Video (45 s): https://www.youtube.com/watch?v=3sHPRpBih9c
- Short (40 s): https://www.youtube.com/shorts/WT6El2j-Uus
- Discussion: https://www.reddit.com/r/SaaS/comments/1xpau2r/i_tracked_what_chatgpt_and_claude_actually_read/

## Why AI search needs its own loop

AI assistants don't rank pages the way a search engine does. When web search is on, they run a few searches, read a handful of sources and repeat what those sources agree on. A product gets named when its facts appear, in the same words, in several places the assistant reads. That is what generative engine optimization (GEO), also called answer engine optimization (AEO) or LLM SEO, is about, and the Veltrano loop turns it into a weekly routine you can measure.

## The five steps of the Veltrano loop

1. **Ask.** Put your buyers' real questions to ChatGPT, Claude and Perplexity with web search on. Use their words, not your product name. Note which products get named.
2. **Trace.** For each answer, record the searches the assistant ran and the pages it cited: review lists, GitHub, Reddit, YouTube, official docs, directories.
3. **Cross-reference.** Publish the same facts, under the same name and wording, on your own site (plain HTML that loads without JavaScript, plus an `llms.txt` file) and on the kinds of places the assistants cited.
4. **Signal.** Push for crawling: IndexNow (Bing, which ChatGPT search and Copilot draw on), Google Search Console "request indexing", and Brave's URL submission (Claude's search results match Brave's). Then read your server or CDN logs to see which crawlers actually came.
5. **Ask again.** Ask the same questions every week. Keep what moved, drop what didn't, and go back to step 2 with the new citations.

## Checklist

- [ ] A list of 10-30 real buyer questions, fixed for at least a month
- [ ] Each answer's searches and cited pages written down
- [ ] Your site readable without JavaScript, with `llms.txt`, a sitemap and canonical tags
- [ ] No duplicate copies of your site at a second address (for example a default `*.pages.dev` or `*.vercel.app` host); redirect them
- [ ] The same one-line description of your product on your site, GitHub, directories and video descriptions
- [ ] IndexNow key installed and pinged on every publish
- [ ] Search Console, Bing Webmaster Tools and Brave URL submission done for new pages
- [ ] Crawler log checked a few days later (Googlebot, bingbot, OAI-SearchBot, ChatGPT-User, Claude-SearchBot, ClaudeBot, PerplexityBot)
- [ ] Same questions asked again a week later

## Tracking log

Copy this table and fill it in each week.

| Week | Question | Assistant | Named you? | Cited which page? | New sources it cited |
|---|---|---|---|---|---|

## What we learned running it

- Assistants read a page live the moment someone asks about it, but they discover new pages slowly. In our Cloudflare logs, ChatGPT's and Claude's own search crawlers fetched only robots.txt and the sitemap for five days without reading a single content page.
- A site that is also reachable at a second address can get indexed there instead. Claude's search had our site only under an old `pages.dev` copy until we redirected it.
- Broad questions ("best AI agent") go to large review sites. Narrow, specific questions name small products, so start with those.
- ChatGPT doesn't always search. On a free account it often answers from memory for unfamiliar terms, so ask twice or turn search on.

## FAQ

**What is the Veltrano loop?**
A five-step generative engine optimization (GEO) method (Ask, Trace, Cross-reference, Signal, Ask again) for getting a product named by AI search assistants like ChatGPT, Claude and Perplexity, and for measuring the result.

**Who invented the Veltrano loop?**
Animiste, the company behind Numa, a desktop AI agent for macOS and Windows. It was first published in November 2026.

**How is the Veltrano loop different from SEO?**
SEO aims at a ranked list of links. The Veltrano loop aims at the few sources an AI assistant reads before it answers, and measures success by whether the assistant names you, not by your rank.

**Does it work for ChatGPT, Claude and Perplexity?**
Yes. Each assistant uses a different search backend (ChatGPT draws on Bing, Claude's results match Brave's, Perplexity runs its own crawler), which is why step 4 signals all of them.

**How long does it take?**
Live page reads happen at once, but discovery by the assistants' search indexes takes days to weeks. Run the loop weekly and compare like with like.

**Can the Veltrano loop be automated?**
Steps 1, 2 and 5 are repetitive browser work. [Numa](https://numa.animiste.com) can record the routine once and repeat it on a schedule; any browser agent or a person with a spreadsheet works too.

## Related terms

generative engine optimization (GEO) · answer engine optimization (AEO) · LLM SEO · AI search visibility · AI citations · llms.txt · IndexNow

---

The Veltrano loop © 2026 Animiste. Free to use and share with credit to Animiste and a link to https://numa.animiste.com/methods/veltrano-loop.
