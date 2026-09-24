# pragmatic-programmer

## Introduction
This is my attempt to give agents the lessons that have shaped my philosophy on software and architecture throughout my career. Importantly, the intent of these skills is not to focus on the syntax or structure as much as the philosophy of why certain decisions should be made.

"I just want my child to make good decisions" - every parent ever

This is very much an experiment of a thesis with no supporting data and should be regarded as such.

## Buckets

Skills are grouped into buckets. Add the marketplace once, then install only the buckets you want.

| Bucket | Skills | Distilled from |
|---|---|---|
| `pragmatic-programmer` | 22 | Hunt & Thomas, *The Pragmatic Programmer*; Eric S. Raymond, *The Art of Unix Programming* |
| `security` | 15 | Nadim Kobeissi, *Post-Quantum Migration Playbook* (`pqc-*`); [mpcsec.org](https://mpcsec.org) MPC audit checklist (`mpc-audit`) |
| `user-experience` | 5 | Retention, referral, outbound sales and SEO skills rewritten from [mayurrathi/awesome-agent-skills](https://github.com/mayurrathi/awesome-agent-skills) |

The `user-experience` upstream carries no license, so those five skills are original rewrites in this repo's style, not copies; each cites its source.

Next(?):
 [ ] - Codecraft
 [ ] - Head First Design Patterns
 [ ] - Thinking Low-Level, Writing High-Level

## Install

In Claude Code:

```
/plugin marketplace add AdaJane/programmer-skills
/plugin install pragmatic-programmer@pragmatic-programmer
/plugin install security@pragmatic-programmer
/plugin install user-experience@pragmatic-programmer
```

Or run `/plugin`, open the `pragmatic-programmer` marketplace, and pick buckets from the list.

Already installed before the split? Run `/plugin marketplace update pragmatic-programmer`. The `pragmatic-programmer` plugin no longer carries the `pqc-*` and `mpc-audit` skills; install `security` to get them back.

## Recommended but Optional
Here's what my user-space CLAUDE.md looks like at the moment:

```md
Prefer enums and constants over string literals and magic numbers

Use a functional programming style with minimal mutability

Use test-driven-development to ensure correct behavior of business logic

Prefer off-the-shelf libraries to custom solutions, especially where the solution concerns mathematics, cryptography, unit-testing mocks, network request interaction, multi-media interaction, and peripheral interaction, exceptions to this should be made in the event that the novel work of the project involves one of these fields, (i.e. don't import a remote cryptography library if the local project is intentionally implementing novel custom cryptography )

When working on Rust projects always check if the modeule you are working in is 'no_std' and be thoughtful when using things like Vec and String in those cases

Keep comments and documentation brief and concise.

Prioritize simplicity, minimizing complexity and lines of code generated.

When working on code repo, identify existing architectural choices such as Object-Oriented, functional, pure, macro-heavy, trait-heavy, etc, and attempt to mimic those conventions in new and refactored code. Essentially, practice "chameleon coding" unless it will compromise the integrity of the final product.

Take care in the crafting of your code — slow down before signing off on work you wouldn't be proud of revisiting in six months. Think deliberately about what you are doing while you are doing it; never program on autopilot or by coincidence.

When reporting a blocker, limitation, or anything you can't do, provide concrete options with trade-offs and a recommendation — never deliver an excuse without alternatives.

Lead with the big picture before the details; tailor explanations to what the reader actually needs to act on.

Treat quality as an explicit requirement, not an afterthought — name the quality bar up front, not after the fact.

Treat your knowledge as a portfolio: diversify, invest regularly, and critically evaluate sources rather than parroting them.
```

## License

[MIT](LICENSE) © Ada Jane Anderson
