---
name: seo-fundamentals
description: "Use when explaining how search engines evaluate pages, deciding whether budget goes to content or technical work, judging whether AI-assisted content is a search risk, or when someone proposes an SEO shortcut (schema, speed, word count) — the mental model, no site data required; for diagnosing a specific site use seo-audit."
---

# SEO Fundamentals

Search engines are trying to answer one question: does this page deserve to be the answer? Everything else — speed, markup, structure — either helps them see the page clearly or gets out of the way. Technical work makes ranking possible; content quality and demonstrated trust earn it. Hold that order and most "SEO tricks" reveal themselves as attempts to skip the part that matters.

## When to use

- Explaining why pages rank, without a specific site's data in hand
- Deciding whether the next month goes to content or to technical fixes
- A proposal promises rankings from schema, speed, or word count alone
- Judging AI-assisted content for search risk
- Framing what to measure before or after an SEO change

## How pages are evaluated

| Dimension | What it represents | Typical signals |
|---|---|---|
| Experience | First-hand involvement | Original examples, demonstrations, lived detail |
| Expertise | Subject competence | Credentials, depth, accuracy |
| Authoritativeness | Recognition by others | Mentions, citations, links |
| Trustworthiness | Reliability and safety | HTTPS, transparency, accuracy over time |

E-E-A-T is an evaluation lens, not a ranking factor you can set. Pages competing on the same topic are separated by trust and experience more often than by keywords.

## Protocol

1. **Start from intent and quality.** Does the page fully answer the query, add something original, and stay accurate? If not, no technical fix will matter.
2. **Treat Core Web Vitals as a floor, not a lift.** LCP under 2.5 s, INP under 200 ms, CLS under 0.1. Failing them holds back a good page; passing them does not rescue a thin one. They decide ties between comparable content.
3. **Let technical work make the page legible, no more.** Crawlable, indexable, canonicalised, on HTTPS; a title that states intent, one H1, a meta description that earns the click rather than ranks. This is the floor; [[seo-audit]] has the checklist.
4. **Use structured data for meaning, not rank.** Article, Organization, Person, Product, Review, BreadcrumbList tell the engine what a thing is and make rich results possible — never guaranteed, never a boost by itself.
5. **Judge AI-assisted content by its output.** Engines evaluate the result, not the authorship method. Drafting and research assistance is fine; unedited generation, factual errors, and thin or duplicated text are the risk.
6. **Weight factors in this order when pages are comparable.** Content relevance and quality → authority and trust → page experience (Vitals, mobile) → technical accessibility as the baseline everything sits on.
7. **Measure with several signals.** Indexed pages and impressions for visibility; click-through from Search Console and engagement time from analytics for engagement; field Vitals for performance; coverage reports for indexing; mentions and links for authority. No single metric tells the story.

## Red flags (rationalizations to reject)

- "Fix the Vitals and rankings will follow." — Speed removes a penalty; it does not supply a reason to rank.
- "Add schema and we'll get rich results." — Schema makes you eligible. Quality decides whether you are picked.
- "AI content gets penalised." — Bad content gets penalised. The tool that wrote it is invisible; the errors and thinness are not.
- "There's a fixed ranking-factor list; we'll tick it." — Weights shift with the query and the competition. Principles hold; checklists rot.

## Composes with

- [[seo-audit]] — the diagnostic that applies these principles to a specific site.
- [[seo-authority-builder]] — the improvement work for the trust and expertise dimensions.

## Source

Distilled from `skills/seo-fundamentals/SKILL.md` in [mayurrathi/awesome-agent-skills](https://github.com/mayurrathi/awesome-agent-skills) (unlicensed upstream; rewritten, not copied).
