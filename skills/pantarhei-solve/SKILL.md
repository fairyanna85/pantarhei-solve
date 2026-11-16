---
name: pantarhei-solve
description: >-
  Structured problem solving and diagnosis for a defined problem, combining consulting frameworks (issue trees, MECE, hypothesis-driven analysis, driver trees), engineering and quality methods (five whys, fishbone, is/is-not, A3, fault trees, theory of constraints), systems thinking and 100 mental models. Use when the user asks why something keeps happening, wants the root cause, wants a problem broken down or structured, asks how to tackle or approach a problem, what is driving a number, or wants a strategy for a competitive, organisational, scaling or behaviour-change problem. Produces the Case Board: a MECE issue tree, ranked hypotheses each with the cheapest test that would tell them apart, and the binding constraint. Says underdetermined when the evidence cannot pick a cause. Not for debugging code. Not for figuring out what the problem is (use pantarhei-reframe), generating ideas (use pantarhei-brainstorm), or choosing between finished options (use pantarhei-decide).
---

# Panta Rhei Solve — The Case Board

Take a defined problem and give it structure: what the parts are, what is causing what, which cause
to test first, and where the leverage is. The board can end at "underdetermined"; it never
manufactures a cause.

Load before starting:
- `references/catalog.json`: problem-solving methods.
- `references/models.json`: lenses and constraints from the shared library (incentives, setting,
  feedback loops, bottlenecks, scale, second-order effects, falsification…).
- `references/plays.md`: the curated sequences (diagnosis, organisational dysfunction, strategy,
  negotiation, scaling, optimisation, behaviour change, competitive threat, post-mortem).
- `references/shared-rules.md`.

## 1. Pin the problem

One sentence: the problem, the metric or symptom, since when, and for whom. Run
`solve.is-is-not` on the symptom when there is any data: where and when does it happen, and where
could it happen but does not. If the user cannot state the problem at all, say it needs framing first (Panta Rhei Reframe does this) and stop.

## 2. Choose the play

Match the user's words to a play in `references/plays.md`. Plays override stage filtering: if a
play names a model, use it. If no play fits, build the sequence from the catalog: one structuring
method + two or three lenses + one constraint.

## 3. Build the board

```
CASE · Partner escalations up 40% since Q2
───────────────────────────────────────────────────────────────
TREE (MECE)                          
├─ More issues created   → volume? new partners? new product surface?
├─ Same issues, escalated more → routing change? SLA change? trust?
└─ Measurement changed   → definition of "escalation" altered in Q2?

HYPOTHESES                       evidence for / against     cheapest test
1 ● Q2 routing change sends L1 to engineering   +timing, +is/is-not   pull 20 tickets pre/post
2   New partner cohort less trained             +volume  −old partners also up   split by cohort
3   Definition changed                          ?                      ask the dashboard owner

BINDING CONSTRAINT   Triage capacity (theory of constraints): everything else waits on it.
CEILING              Medium. Timing fits H1; no test run yet.
```

Rules for the board:
- **The tree must be MECE.** If two branches overlap or something is missing, fix it before
  hypothesising.
- **Three to five hypotheses, ranked.** Each has evidence for and against and the **cheapest test
  that discriminates it from the next one**, not merely a test that confirms it.
- **Always include the boring hypothesis**: measurement changed, sample is small, regression to the
  mean.
- **Name the binding constraint or leverage point** when the play involves improvement.
- **State the ceiling**: what the evidence supports, in one line.

## 4. Contrast pair

Every board adjudicates one contrast pair from the play or from `tension_with` (for example
character vs setting, five whys vs fishbone, issue tree vs reframing). Name the winner for this case
and the fact that would flip it.

## 5. Hand off

- The top hypothesis needs attacking before acting → "Next step: stress-test hypothesis 1 before acting (Panta Rhei Challenge does this)."
- Countermeasures are needed → "Next step: generate countermeasures for hypothesis 1 (Panta Rhei Brainstorm does this)."
- Countermeasures exist and one must be picked → "Next step: choose a countermeasure (Panta Rhei Decide does this)."

## Rules specific to Solve

- **Structure before content.** Tree first, hypotheses second, answer last.
- **Hypothesis-driven is allowed only with a kill test.** A hypothesis without a test that could
  kill it is a conclusion in disguise.
- **Underdetermined is a complete answer.** Two quarters of one team's data cannot name a cause;
  say so and give the tests.
- **No blame in root causes.** If the last "why" is a person, ask one more why.
- **Code debugging is out of scope.** The description excludes it; if it arrives anyway, say this
  skill is for non-code problems and stop.
