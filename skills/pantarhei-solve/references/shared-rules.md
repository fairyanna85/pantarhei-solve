# Shared rules (vendored into every skill as `references/shared-rules.md`)

Every Panta Rhei skill follows these rules. A skill's own SKILL.md may add rules for its stage; it
may not override these.

## 1. The stage map

| Stage | Owned by | The question at this stage |
|---|---|---|
| frame | pantarhei-reframe | What is the real problem, and whose is it? |
| generate | pantarhei-brainstorm | What are the options, including the strange ones? |
| decompose | pantarhei-solve | What are the parts, and what is causing what? |
| stress_test | pantarhei-challenge | What breaks this? |
| decide | pantarhei-decide | Which one, under what conditions, with what exit? |
| execute, review | (future repos) | — |

Work only in your own stage. When the user's need sits in another stage, finish what was asked and
name the next step in the handoff line.

**Standalone rule.** Every module is complete on its own. It never requires a sibling, never loads a
sibling's files, and never degrades its own output because a sibling is absent. The pack adds
convenience (one install, the hub's end-to-end sessions), not capability.

## 2. Modes

- **lens**: applied outward to the problem. Generates structure, options, predictions.
- **audit**: applied inward to the reasoner and the sources. Corrects a known distortion. Never
  produces an answer; only discounts one.
- **constraint**: a property of reality. Bounds the feasible set. Run constraints before lenses.

## 3. Evidence ceilings

Read the `evidence_class` of whatever is doing the work before writing the conclusion.

| Class | May | May not |
|---|---|---|
| formal | carry a conclusion if the premises hold | hide which premises it needs |
| empirical | support a conclusion, citing the finding | prove one; ignore the replication caveat in `evidence_note` |
| heuristic | direct attention, generate candidates, rank options | settle a claim |
| analogical | suggest a hypothesis | confirm anything; a chain of analogies is not an argument |

Practitioner sources (`origin.type: practitioner`) are useful prompts with no research behind them.
Say so when one carries weight.

## 4. Selection budget

- Pick the fewest methods that change the answer. Defaults per stage: frame 3–5, generate 3–6 cards
  per round, decompose 3–6, stress_test 4–8 attacks, decide 4–6 advisors.
- Drop test for every method: *if I remove it, does the output change?* If no, remove it.
- Show only the methods that carried weight. Never list what was considered and dropped.

## 5. Combination grammar

- **Chain**: output of one is the input to the next. `pairs_with` is directional.
- **Contrast pair**: two methods that disagree, adjudicated on this case's evidence. `tension_with`
  is symmetric. Never split the difference; name the winner and the fact that would flip it.
- **Stack**: several methods on the same object at once.
- **Loop**: a method applied to its own output. Once.

## 6. Divergent and convergent never mix

When generating, do not evaluate. When evaluating, do not add options. If evaluation surfaces a gap
that needs new options, say so in the handoff instead of generating in place.

## 7. Output contract (all skills)

1. Lead with the result: the reframe, the idea wall, the case board, the red-team verdict, the
   decision.
2. Name each method inline with its origin in a short attribution: *Subtraction (Adams et al., 2021)*.
3. Show the evidence class when a method carries weight: `[empirical]`, `[heuristic]`.
4. State the ceiling when it is low. "Underdetermined" is a complete answer.
5. Separate what follows from evidence from what is inference.
6. End with one handoff line, as a statement: the next step in plain words, useful on its own,
   then the sibling that does it in parentheses ("Next step: stress-test the top three (Panta Rhei Challenge
   does this)."). Never assume the sibling is installed, never tell the user to install it, no
   closing question, no menu of offers.

## 8. Format rule

Every signature interaction has a plain-text format (works in a terminal, Hermes, mobile). If the host
offers a visual tool, render the same content visually as well. Never depend on the visual.

## 9. Corrections

If the user corrects a premise, test whether it invalidates the frame, not only the detail. If the
frame breaks, discard the method selection and restart the stage. Do not keep the conclusion and swap
its support.

## 10. Anti-patterns (all skills)

- **Method soup**: many names, none consequential.
- **Retrofit**: choosing methods after the answer, to justify it.
- **Fluency as evidence**: a well-phrased analogy is not a finding.
- **Audit-only**: critique with nothing standing at the end (except in Challenge, where the
  surviving version of the idea is the thing left standing).
- **Bias-naming as argument**: naming a bias is a reason to check, not a rebuttal.
- **Symmetric dodge**: presenting both sides of a contrast and declining to adjudicate.
- **Manufactured generalisation**: inventing a principle to support a specific claim.
- **Guru inflation**: presenting a practitioner's heuristic as research.
