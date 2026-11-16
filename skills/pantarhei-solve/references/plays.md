# Plays

The legacy plays this skill carries (legacy numbers 3, 5, 7, 8, 9, 10, 11, 13, 15). Slugs refer to records in `models.json`. `→` is a chain, `vs` is a contrast pair to adjudicate, `+` is a stack.

Match the archetype to the user's actual words, run the play, drop any step that does not change
the answer. A play is a starting route, not a script: if the problem does not fit one, route from
`stages` and `use_when` directly.

---

## 1. Diagnosis — why is this happening
*"Why does X keep occurring"*

`mm.incentives` + `mm.setting` + `mm.feedback-loops` → `mm.first-conclusion-bias` → `mm.confirmation-bias-and-falsification`
Contrast: `mm.character` **vs** `mm.setting` / `mm.overestimate-consistency-of-behavior`
Audits: `mm.occams-razor`, `mm.hanlons-razor`, `mm.narrative-instinct`
Output: ranked causal candidates with a discriminating test for each. Say so if underdetermined.


## 2. Strategy and positioning
*"How do we win here / where should I position"*

`mm.scarcity` → `mm.niches` → `mm.monopoly-and-competition` → `mm.asymmetric-warfare` → `mm.red-queen-effect`
Contrast: `mm.niches` **vs** `mm.scale`; `mm.specialization` **vs** `mm.alloying`
Audit: `mm.survivorship-bias` on any benchmark being copied
Output: the defensible axis and its expiry conditions.


## 3. Persistent organisational dysfunction
*"Why is this team / process broken"*

`mm.incentives` → `mm.hierarchical-organization` → `mm.bottlenecks` → `mm.feedback-loops` →
`mm.seeing-the-front`
Contrast: `mm.setting` **vs** `mm.character`
Audits: `mm.self-preservation`, `mm.sensitivity-to-fairness`, `mm.envy-and-jealousy`
Output: the binding constraint, not a list of everything wrong.


## 4. Negotiation or conflict with a counterparty
*"How do I handle this person / company"*

`mm.relativity` → `mm.incentives` → `mm.scarcity` → `mm.counterinsurgency` → `mm.mutually-assured-destruction`
Contrast: `mm.reciprocity` **vs** `mm.asymmetric-warfare`
Audits: `mm.hanlons-razor`, `mm.overestimate-consistency-of-behavior`, `mm.framing` on who set the terms
Output: their payoff structure, your asymmetric axis, the escalation off-ramp.


## 5. Post-mortem — outcome already known
*"What went wrong / why did that work"*

`mm.hindsight-bias` → `mm.randomness` → `mm.survivorship-bias` → `mm.narrative-instinct` →
`mm.feedback-loops`
Contrast: `mm.natural-selection-and-extinction` **vs** `mm.randomness` (was it selection or noise)
Output: what was skill, what was luck, what the contemporaneous record actually says.
Refuse to produce lessons the evidence does not carry.


## 6. Scaling something that works
*"How do we take this from 10 to 1000"*

`mm.scale` → `mm.bottlenecks` → `mm.critical-mass` → `mm.hierarchical-organization` → `mm.thermodynamics`
Contrast: `mm.efficiency` **vs** `mm.margin-of-safety`
Audit: `mm.overgeneralization-from-small-samples` on the pilot results
Output: what breaks at each order of magnitude and the maintenance cost nobody priced.


## 7. Optimisation request
*"Make this faster / cheaper / better"*

`mm.optimization` (name the objective function first) → `mm.bottlenecks` → `mm.law-of-diminishing-returns` →
`mm.friction-and-viscosity`
Contrast: `mm.efficiency` **vs** `mm.margin-of-safety`
Audits: `mm.map-is-not-the-territory` on the metric, `mm.representation` on the dashboard
Output: the one constraint worth attacking and where to stop.


## 8. Behaviour change — self or team
*"I keep failing to do X"*

`mm.setting` → `mm.tendency-to-minimize-energy-output` → `mm.activation-energy` → `mm.inertia` → `mm.rhythm`
Contrast: `mm.incentives` **vs** `mm.setting` (payoff problem or environment problem)
Audit: `mm.denial` on what is actually being avoided
Output: the environmental lever, not the motivational instruction.


## 9. Competitive threat or disruption
*"Should we be worried about X"*

`mm.creative-destruction` → `mm.red-queen-effect` → `mm.asymmetric-warfare` → `mm.interdependence` →
`mm.multiply-by-zero`
Contrast: `mm.equilibrium` **vs** `mm.creative-destruction` (stable or about to break)
Audit: `mm.bubbles` on whether the threat is real or narrative
Output: what is actually being selected for, and which of your assets goes to zero.


---

# Contrast-pair register

The adjudicated tensions. These produce most of the analytical value. Each is a real disagreement
about how the world works, not a rhetorical balance. Name the winner for the case at hand.

| Pair | The disagreement | Adjudicate on |
|---|---|---|
| `mm.first-principles-thinking` First Principles **vs** `mm.replication` Replication | Build from truth or copy the proven | Does the convention encode knowledge you have not recovered |
| `mm.margin-of-safety` Margin of Safety **vs** `mm.efficiency` Efficiency / `mm.leverage` Leverage | Buffer or performance | Variance of the environment and reversibility of failure |
| `mm.failure-to-account-for-base-rates` Base Rates **vs** `mm.tendency-to-stereotype` Individuating Information | Reference class or this specific case | Quality and independence of the case-specific evidence |
| `mm.character` Character **vs** `mm.setting` Setting / `mm.overestimate-consistency-of-behavior` FAE | Trait or situation | Does the behaviour persist across changed contexts |
| `mm.niches` Niches **vs** `mm.scale` Scale | Defensible narrow or vulnerable broad | Rate of environmental change in that niche |
| `mm.specialization` Specialization **vs** `mm.alloying` Alloying | Depth or rare combination | Is the field's frontier inside the domain or at its borders |
| `mm.occams-razor` Occam's Razor **vs** `mm.irreducibility` Irreducibility / `mm.ecosystems` Ecosystems | Simplify or respect complexity | Does the simple account predict, or only summarise |
| `mm.hanlons-razor` Hanlon's Razor **vs** `mm.incentives` Incentives | Incompetence or payoff-driven | Is the error consistently in one party's favour |
| `mm.law-of-diminishing-returns` Diminishing Returns **vs** `mm.red-queen-effect` Red Queen / `mm.critical-mass` Critical Mass | Stop or push through | Is there a threshold ahead or a flattening curve |
| `mm.equilibrium` Equilibrium **vs** `mm.creative-destruction` Creative Destruction | Stable or about to break | Is a new entrant already operating at lower cost |
| `mm.tendency-to-want-to-do-something` Do Something **vs** `mm.activation-energy` Activation Energy | Restraint or initiation | Cost of waiting versus cost of a wrong move |
| `mm.circle-of-competence` Circle of Competence **vs** `mm.curiosity-instinct` Curiosity | Stay inside or expand | Is failure in the new domain survivable |
| `mm.narrative-instinct` Narrative Instinct **vs** `mm.plot` Plot | Distrust story or use it | Are you explaining to yourself or persuading others |
| `mm.trust` Trust **vs** `mm.social-proof` Social Proof | Extend trust or verify independently | Does the consensus have independent evidence behind it |
| `mm.thought-experiment` Thought Experiment **vs** `mm.seeing-the-front` Seeing the Front | Reason or observe | Is direct observation available at acceptable cost |
| `mm.map-is-not-the-territory` Map is Not the Territory **vs** `mm.algorithms` Algorithms | Distrust the model or commit to the rule | Are the conditions that validated the rule still holding |
