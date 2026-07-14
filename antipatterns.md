# Anti-patterns — interviewing & elicitation

The traps `elicit` defends against. Each is a demarcated bad-question→better-question
pair with the discriminating feature stated — the negative-examples-first schema. The
bad form is shown once, compactly; the words go on the fix and the why.

### Hypothetical / future-tense question

❌ Wrong: "Would you use a tool that does X?" / "How much would you pay for this?"
✅ Right: "How do you solve this today?" / "What does this problem cost you now?"
Why it flips: future and hypothetical answers are aspirational and flattering; past behavior is data.
Prevents: building on imagined demand that evaporates on contact with reality.

### Pitching instead of learning

❌ Wrong: "We're building X — do you like it?"
✅ Right: "Walk me through the last time you hit this problem."
Why it flips: once you reveal your idea, they stop reporting their problem and start being nice; compliments are fool's gold — shiny and worthless.
Prevents: validation theater that feels like signal.

### Leading question (presupposition / loaded word)

❌ Wrong: "How fast were they going when they smashed into each other?"
✅ Right: "What happened? How fast were they going?"
Why it flips: a loaded verb or embedded presupposition implants the answer — Loftus showed "smashed" vs "hit" shifted speed estimates and produced false memories of broken glass.
Prevents: hearing your own assumption echoed back as their testimony.

### Agree/disagree framing (acquiescence bias)

❌ Wrong: "Do you agree that the dashboard is easy to use?"
✅ Right: "Would you say the dashboard is easy or hard to use?"
Why it flips: people yea-say to a stated proposition regardless of content; a balanced forced choice between two fully-stated alternatives removes the pull.
Prevents: a false-positive reading you then act on.

### Asking the user to design

❌ Wrong: "What features do you want?"
✅ Right: "Tell me about the last time the tool got in your way."
Why it flips: users are authorities on their problems, not your solutions; accept a feature request only after probing the pain behind it.
Prevents: a wishlist that doesn't map to real needs.

### Generic instead of specific

❌ Wrong: "How do you usually handle escalations?"
✅ Right: "Tell me about a specific escalation that went wrong — what happened, what did you do, how did it end?"
Why it flips: "usually" yields a sanitized composite; one real incident yields actual behavior and detail.
Prevents: the truth getting averaged away.

### Open-blank when a decision is the goal

❌ Wrong: "What architecture do you want?"
✅ Right: "Postgres gives X at cost Y; SQLite gives Z at cost W — which fits, and why?"
Why it flips: a blank prompt forces recall from nothing; a fork lets them recognize and react.
Prevents: vague, stalled, or anchored-on-the-first-idea answers.

### Rigged fork (manufactured answer)

❌ Wrong: offering one real option beside two strawmen, or stating a heuristic as already-agreed to steer the pick.
✅ Right: present genuine alternatives with honest tradeoffs; attribute your lean as yours, not as settled.
Why it flips: a fork's options *create* preference, so an unfair set discovers the answer you planted rather than the one they hold.
Prevents: mistaking a manufactured consensus for an elicited one.

### Interviewing what you could find

❌ Wrong: asking the user a question answerable from the code, docs, logs, or earlier in the conversation.
✅ Right: research the artifact first; interview only for what only the person holds.
Why it flips: self-report is biased and costly; records are ground truth and free.
Prevents: wasting the interview — and the person's patience — on retrievable facts.
