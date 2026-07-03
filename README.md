# Requirements-to-User-Story Translator

**Every requirement hides a story. Find it.**

Live demo → https://bodhiprotocol.github.io/requirements-translator/

---

## Why this exists

Stakeholders don't speak in user stories. They speak in run-on sentences, half-finished asks, and complaints disguised as requirements. Turning that into `As a [role], I want [goal], so that [benefit]` plus testable acceptance criteria is a core BA skill — usually invisible, done silently in a notebook or a Jira ticket.

This tool makes that translation visible, live, in the browser. Paste a messy sentence, watch it get parsed into a role, a goal, and a benefit, with the reasoning shown alongside the result.

## What's inside

Paste any requirement and get:
- A formatted user story (`As a... I want... so that...`)
- 2–3 Given/When/Then acceptance criteria, generated from templates and flavored by capital-markets keywords (settlement, trade, compliance, reporting, risk) when present
- A "what I detected" breakdown showing exactly which words mapped to role, goal, and benefit — including when a benefit is *suggested* (inferred from keywords) rather than *detected* (explicitly stated with "so that")

Five example inputs are built in, covering the range: an explicit "so that" clause, a "because" clause, no stated role, and no stated benefit at all.

## Tech

One self-contained `index.html`. No frameworks, no build step, no API calls. Deterministic pattern-matching in vanilla JS — not an AI model — so it runs instantly and works offline.

## Part of BodhiProtocol

Tools and games that make complex systems simple.
More at [github.com/BodhiProtocol](https://github.com/BodhiProtocol).

> "The single biggest problem in communication is the illusion that it has taken place." — George Bernard Shaw
