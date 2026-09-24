---
name: retention-referral
description: "Use when designing a cancellation flow, failed-payment (dunning) recovery, referral loop, affiliate program, or account health score, when involuntary churn is rising, or when churn is being answered with more acquisition spend instead of a product loop."
---

# Retention & Referral

A customer you already have is the cheapest one to keep and the cheapest route to the next one. Retention is a set of product loops, not a campaign: catch the cancel at the moment it happens, recover the card that failed, and give a delighted user a reason and a moment to bring a friend. Each loop has a trigger, a path, and an ending — design all three or you have a leak with a banner on it.

## When to use

- Designing or reviewing a cancellation flow
- Failed payments are quietly becoming churn
- Adding a referral or affiliate program to a product
- Deciding which accounts need proactive outreach
- Churn numbers are being answered with more top-of-funnel spend

## The save-offer map

| Stated reason | Offer that fits it |
|---|---|
| Price | Discount, or downgrade to a cheaper tier |
| Not using it | Pause for 1–3 months instead of cancelling |
| Missing feature | Roadmap preview, or an introduction to support |

## Protocol

1. **Build the cancel flow as a loop, not a button.** Trigger → exit survey (one question: why) → save offer matched to the reason → confirmation. Keep "Cancel" visible and honest throughout; a hidden or nagging cancel buys a month and costs the brand.
2. **Recover involuntary churn automatically.** Use the processor's smart retries, which charge on the days a card is likely to succeed. Send 3–4 plain-text emails spread across the retry window (typically two to four weeks), rising in urgency, each with a link that updates payment details without a login. Show a persistent past-due banner in-app.
3. **Engineer the referral loop around the aha moment.** Prompt the share right after a user gets value, not at signup. Loop: aha → share action → friend converts → reward. Double-sided rewards (referrer gets X, friend gets Y) outperform single-sided; tiered milestones ("refer five, get …") turn one share into a habit.
4. **Scale reach through affiliates whose audience is your persona.** Recruit by audience fit, not follower count. For subscriptions, pay a recurring percentage so incentives stay aligned past the first sale. Ship an enablement kit: banners, email swipes, comparison pages.
5. **Score account health and act on the slope.** Track login frequency, use of the feature that delivers the core value, and support sentiment. A falling score triggers outreach or a re-engagement sequence before the cancel flow ever fires.

## Red flags (rationalizations to reject)

- "Make cancelling hard; it saves accounts." — It saves a month and produces chargebacks, reviews, and users who never come back; in several jurisdictions it is also unlawful.
- "The card failed, so the customer left." — Most failed payments are card problems — expiry, limits, issuer declines — not decisions. Dunning is the cheapest retention work you have.
- "Reward the referrer; the friend gets the product." — The friend has no reason to act, so the loop stalls at the conversion step.
- "We'll cover churn with more acquisition." — Filling a leaking bucket faster is still a leaking bucket.

## Composes with

- [[sales-cold-outreach]] — the handoff criteria there decide who enters the funnel; poor fit at the top shows up here as churn.
- [[pragmatic-programmer:rule-of-least-surprise]] — a cancel or referral flow that behaves as users expect is the one they trust.

## Source

Distilled from `skills/retention-referral/SKILL.md` in [mayurrathi/awesome-agent-skills](https://github.com/mayurrathi/awesome-agent-skills) (unlicensed upstream; rewritten, not copied).
