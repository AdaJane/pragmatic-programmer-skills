---
name: seo-audit
description: "Use when asked for an SEO audit, technical SEO review, SEO health check, or on-page/meta-tag review of a specific site, when organic traffic or rankings dropped, or after a migration, redesign, or CMS change — evidence-based diagnosis from crawl and Search Console data; does not implement fixes unless asked."
---

# SEO Audit

An audit finds what is stopping a site from being crawled, indexed, understood, and trusted, then ranks those problems by what they cost. It is diagnosis, not treatment: every finding carries evidence, a severity, and a confidence, and the score at the top summarises the findings rather than replacing them. An audit that reports a number without the issues behind it, or fixes things while measuring them, has stopped being an audit.

## When to use

- Someone asks for an SEO audit, health check, or technical SEO review
- Organic traffic or rankings dropped and nobody knows why
- After a migration, redesign, or CMS change
- A page or template needs an on-page or metadata review
- Before an SEO roadmap is written, so it rests on findings rather than opinion

## Audit order

| Category | Weight | Look for |
|---|---|---|
| Crawlability & indexation | 30 | `robots.txt` blocking real paths; invalid or non-canonical sitemaps; pages deeper than three clicks; orphans; accidental `noindex`; canonical conflicts; redirect chains; soft 404s; duplicate content; inconsistent HTTPS, hostname, or trailing-slash rules |
| Technical foundations | 25 | LCP, INP, CLS and their causes (server time, images, JS, CSS, caching, fonts); viewport, tap targets, desktop parity; certificates, mixed content, redirects to HTTPS |
| On-page | 20 | Unique intent-aligned titles; descriptive metas; one H1 and a logical hierarchy; pages that cannibalise each other; alt text and image weight; internal links with descriptive anchors |
| Content quality & E-E-A-T | 15 | First-hand experience, original data, named authors; accuracy and currency; topical focus |
| Authority & trust | 10 | Citations, mentions, links; visible business information, policies, security |

Weights reflect what blocks the categories below, not what earns rankings; for ranking weight and the Vitals thresholds see [[seo-fundamentals]].

## Protocol

1. **Gate on scope before auditing.** Establish site type, primary goal, markets and languages, whether the audit is whole-site or specific sections, and what data exists (Search Console, analytics, known penalties, recent changes). Where context is missing, state the assumptions you are auditing under.
2. **Audit top-down through the table.** Nothing below crawlability matters if the engine cannot reach or keep the page.
3. **Record every finding in one shape.** One-sentence issue, category, evidence (URLs, headers, crawl or Search Console data — never intuition), severity (Critical / High / Medium / Low), confidence (High / Medium / Low), why it matters, and a what-not-how recommendation.
4. **Score the categories, then weight them.** Each category starts at 100 and loses points per finding (see Scoring); the index is the weighted sum, rounded. Any open Critical finding caps the band at Fair regardless of the sum. If a category is out of scope, redistribute its weight and say so.
5. **Derive the action plan from the findings.** Critical blockers → high-impact improvements (large cumulative deductions, template-wide issues) → quick wins (cheap, measurable) → longer-term opportunities (structure, depth, authority). Each group cites its findings and the score range it should recover. No timelines unless asked.
6. **State the limits.** The index measures readiness, not rankings; competition and algorithm updates are unscored; the authority category is directional. If a prior audit exists, report the score delta and attribute it to specific fixes.

## Scoring

| Severity | Deduction per finding |
|---|---|
| Critical (blocks crawl, index, or rank) | −15 to −30 |
| High | −10 |
| Medium | −5 |
| Low / cosmetic | −1 to −3 |

Apply the full deduction at High confidence, half at Medium, a quarter at Low. Bands: 90+ Excellent, 75+ Good, 60+ Fair, 40+ Poor, below 40 Broken — and an open Critical finding never scores above Fair.

## Red flags (rationalizations to reject)

- "We scored 85, so we're in good shape." — Not with an open Critical finding; the cap exists because a sum cannot outrank the findings.
- "The tool gave it a 92." — A tool score without interpretation is a screenshot, not evidence. Say what the data shows and why it matters.
- "I'll fix the small stuff as I go." — Fixing during the audit destroys the baseline and blurs what caused which change.
- "Skip scoping; just audit everything." — Without goals and data access you cannot weight anything, and the plan will be a list.

## Composes with

- [[seo-fundamentals]] — the evaluation model this audit applies, and where the Vitals thresholds live.
- [[seo-authority-builder]] — the follow-on work when the content and trust categories score low.
- [[pragmatic-programmer:prove-dont-assume]] — every finding needs evidence; "best practice says" is not a finding.

## Source

Distilled from `skills/seo-audit/SKILL.md` in [mayurrathi/awesome-agent-skills](https://github.com/mayurrathi/awesome-agent-skills) (unlicensed upstream; rewritten, not copied).
