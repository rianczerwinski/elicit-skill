---
name: elicit
description: Conduct a good interview or elicitation — pull accurate information, requirements, a decision, or tacit knowledge out of a person by presenting concrete options and a strawman to react to (fork-based, strawman-first), asking about past behavior rather than hypotheticals, and avoiding leading questions. Use when you need to interview the user, gather requirements, elicit a preference or a decision, run a discovery conversation, ask which of several options they want, or question the user well on behalf of another skill.
license: MIT
---

# elicit

Run a good interview — pull accurate information, requirements, a decision, or tacit knowledge out of a person without contaminating it. The governing move: **ask by showing, not by asking blank.** Put concrete options or a strawman in front of them and harvest the reaction — recognition beats recall, and a wrong artifact provokes corrections a blank question never will.

Full technique inventory and sourcing in `references/techniques.md`; the bad-question→better-question pairs are in `antipatterns.md`.

## When to use

Use when you need to interview the user, gather requirements, elicit a preference or a decision, run a discovery conversation, or choose among options with them — or when another skill needs to question the user well (e.g. skill-skill's Phase 1 hands its interview here).

## When NOT to interview (check this first)

Interviewing is expensive and self-report is biased and lossy. Before asking a person:

- **Inferable from context?** If the answer is in the conversation, the code, the docs, or the logs — find it there. Don't re-ask what's already known.
- **A "what do you actually do" question?** Check the record or observe; people misreport their own behavior. Ask for the *why* and the *history*, not the *what*.
- **A solution question?** Users are authorities on their problems, not on your design. Elicit the pain, not a feature wishlist.

Interview only for what *only this person* can supply: their reasons, history, constraints, and reactions.

## The method (open field — judgment, not a rigid script)

1. **Lead with a strawman or a fork, not an open question.** Show concrete options with their tradeoffs, or a draft to shred. "Postgres buys X at cost Y; SQLite buys Z at cost W — which fits?" beats "what database do you want?" Reacting is easier and truer than generating from blank.
2. **Ask about the concrete past, not the hypothetical future.** "How do you solve this now?" / "Tell me about the last time X happened" — never "would you use…" / "how much would you pay…". Future and hypothetical answers are aspirational noise.
3. **Open before closed, then funnel.** Let them free-recall first — it is more informative and uncontaminated by your framing; only then narrow to confirming questions. Use silence and "tell me more" instead of stacking questions.
4. **Ladder for the why.** Take something they named and ask "why does that matter to you?" until you reach the underlying reason or value.
5. **Harvest, feed back, redirect.** Reflect what you heard; let their pushback steer the next question. The correction *is* the data.

## Asking for a decision → fork

When the goal is a *choice*, present 2+ real options paired with their honest tradeoffs and ask them to pick and react. State your own lean as yours, not as settled. Construct the fork fairly — fair options, real tradeoffs — because a rigged option set manufactures the answer it pretends to discover (see `antipatterns.md`).

## Honesty constraints (don't oversell the method)

- A fork can *create* a preference that didn't pre-exist (framing, anchoring). Offer genuine alternatives, not a disguised steer.
- Recognition-over-recall is a tendency, not a law; free recall still wins for completeness.
- These are heuristics, not guarantees — match the technique to the person and the question, and say so when you're inferring rather than knowing.

## Anti-patterns

See [antipatterns.md](antipatterns.md) — bad-question→better-question pairs, each with the discriminating feature that flips it.

## Additional resources

- [references/techniques.md](references/techniques.md) — the named techniques (Mom Test, funnel, laddering, critical-incident, contextual inquiry, cognitive interview…), cross-cutting principles, the interview-vs-infer-vs-research gate, and contested/uncertain flags with sources.
- [antipatterns.md](antipatterns.md) — the negative-examples core.
