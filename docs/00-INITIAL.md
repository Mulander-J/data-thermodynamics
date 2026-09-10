# Data Thermodynamics · Initiation

> **数热学 / Data Thermodynamics**
>
> Version: **0.2.0**
>
> Author: **Mulander-J**
>
> Status: **Open, evolving theoretical framework**
>
> Role: **Canonical core document**
>
> Note on authorship: The conceptual direction, core problems,
> explanatory constraints, and major theoretical constructs are
> author-led. AI tools have been used for expansion, synthesis,
> drafting, and language refinement. Scientific validity and empirical
> verification remain open questions.

------------------------------------------------------------------------

## Origin

Data Thermodynamics began with a deliberately provocative proposition:

> **Data itself possesses heat.**

The original intuition was that data can become more valuable through
processing and lose its original decision advantage through use,
diffusion, or time. Thermodynamic language provided a way to ask whether
these changes could be described in terms of temperature, gradients,
dissipation, work, and steady states.

The original formulation was intentionally metaphorical:

- processing may correspond to **heating**;
- consumption or diffusion may correspond to **cooling**;
- differences in actionable value may behave like **gradients**;
- resources may be allocated in response to those gradients;
- systems may lose useful gradients unless they receive new inputs or
    adapt;
- feedback may allow a system to recover and maintain a useful
    operating regime.

The initial metaphor was stronger than the current theory. In
particular, the early formulation treated data value as if it obeyed a
conservation law. Subsequent criticism showed that data value can be
copied, regenerated, contextually created, destroyed, and redistributed.
The framework therefore treats **value accounting** rather than literal
value conservation as the stronger starting point.

The purpose of this document is to preserve the productive core of the
original intuition while explicitly separating:

1. empirical observations,
2. candidate theoretical propositions,
3. mathematical formalisms,
4. thermodynamic metaphors,
5. speculative extensions.

------------------------------------------------------------------------

## Definition

**Data Thermodynamics (DT)** is a proposed cross-disciplinary framework
for studying the **gradients, flows, transformations, dissipation, and
regeneration of actionable value in data systems**.

Thermodynamics is used primarily as a **conceptual and mathematical
language**, not as an ontological claim that data literally is heat or
that data systems are physical thermodynamic systems in the ordinary
sense.

A compact definition is:

> **Data Thermodynamics studies how actionable value in data systems is
> distributed, transformed, dissipated, regenerated, and maintained
> under constraints.**

The framework asks questions such as:

- What makes a datum actionable in one context but not another?
- Can actionable value be measured as a marginal quantity?
- What constitutes a value gradient?
- When does a data transformation increase or decrease actionable
    value?
- How does value move through data-processing and decision pipelines?
- What is lost during processing, transmission, storage, or
    consumption?
- How can feedback restore useful value gradients?
- Under what conditions do data systems become overloaded, stagnant,
    or unable to generate useful work?

### Current epistemic status

Data Thermodynamics is **not an established academic discipline**. It is
a theoretical proposal and an evolving research framework.

Its scientific status depends on whether its core propositions can be
operationalized, compared with existing theories, and falsified using
empirical evidence.

------------------------------------------------------------------------

## Epistemic Hierarchy

The framework uses the following hierarchy.

### Level 1 --- Empirical phenomena

Observed phenomena are primary.

Examples:

- data has context-dependent utility;
- data value can change over time;
- data can contribute differently to different models or decisions;
- processing can improve or damage downstream utility;
- information systems can exhibit overload, stagnation, and recovery;
- feedback can alter subsequent data-processing behavior.

### Level 2 --- Operational concepts

Concepts must eventually be connected to measurable quantities.

Examples:

- actionable value $V$;
- data temperature $\Theta_D$;
- value gradient $\nabla \Theta_D$;
- value loss;
- recovery;
- responsiveness;
- feedback gain.

### Level 3 --- Candidate propositions

These are hypotheses that can be supported or rejected.

### Level 4 --- Mathematical models

Equations are provisional representations of the propositions, not
evidence for them.

### Level 5 --- Thermodynamic metaphors

Terms such as heat, cooling, heat death, phase transition, and exergy
may guide intuition, but their legitimacy depends on whether they
produce useful, testable predictions.

### Level 6 --- Speculative extensions

Topics such as quantum-like data states, cosmic data thermodynamics, AI
awakening, or extreme cognitive architectures belong here unless
independently justified.

------------------------------------------------------------------------

## Ontological Status of the Thermodynamic Metaphor

> **Thermodynamics is a language of Data Thermodynamics, not its
> ontology.**

The framework does not assume that:

- data is a physical form of heat;
- actionable value is a conserved physical quantity;
- every data transformation obeys a thermodynamic equation;
- a data temperature must be a scalar intrinsic to a dataset.

Instead, the thermodynamic vocabulary is retained when it helps express
structural properties such as:

- gradients;
- directed flows;
- dissipation;
- irreversibility;
- nonequilibrium;
- response to perturbation;
- efficiency;
- feedback;
- steady operation.

If another formalism explains the same phenomenon better, it should be
preferred.

### Metaphor humility principle

> **When the metaphor conflicts with observation, modify the metaphor
> rather than modifying the observation.**

The framework therefore treats metaphorical elegance as scientifically
irrelevant unless it produces measurable explanatory or predictive
value.

------------------------------------------------------------------------

# 5. Core Propositions

The current core is organized around seven propositions.

## C1. Contextual Value

The actionable value of data is relational rather than intrinsic.

Let:

- $D$ be a data object;
- $C$ be the relevant context;
- $T$ be temporal state;
- $A$ be the available action set;
- $R$ be a resource constraint.

Then a general value function may be written as:

$$
V = V(D \mid C,T,A,R)
$$

A simplified form is:

$$
V = V(D \mid C)
$$

This means the same data may have high actionable value in one context
and low value in another.

This proposition is compatible with existing data-valuation research,
which already treats data value as task-, model-, or decision-dependent.

------------------------------------------------------------------------

## C2. Data Temperature

**Data Temperature** $\Theta_D$ is a proposed relational construct for representing the
marginal actionable value of data under a specified context and resource
constraint.

One candidate formulation is:

$$
\Theta_D(C,R)=\frac{\partial V(D \mid C)}{\partial R}
$$

This equation is a **candidate operational formulation**, not an established
physical definition. The semantics of the resource variable $R$ must be
defined separately for each application.

The exact resource variable $R$ is not fixed and may depend on the application.

The intended interpretation is not "how much value the data contains"
but rather:

> **How strongly does the availability or use of this data change
> actionable value under the relevant constraint?**

This differs from the original definition of "value density."

### High-temperature data may exhibit

- high marginal decision relevance;
- scarcity;
- freshness;
- strong task specificity;
- high opportunity cost;
- high expected utility from timely use.

### Low-temperature data may exhibit

- redundancy;
- low marginal utility;
- obsolescence;
- widespread availability;
- low decision sensitivity.

No dataset is inherently hot or cold without specifying the context.

------------------------------------------------------------------------

## C3. Value Gradient

A data system becomes operationally interesting when different states
have different actionable values.

A candidate value gradient is:

$$
\nabla \Theta_D
$$

At v0.2, the state space over which this gradient is taken is deliberately
left unspecified. It may depend on the application (for example, resource,
time, context, or system state).

The central hypothesis is:

> **Actionable-value gradients create opportunities for directed
> resource allocation and work.**

A candidate relationship is:

$$
|\nabla \Theta_D| \uparrow
\quad \Rightarrow \quad
\text{potential for directed resource allocation} \uparrow
$$

This is a hypothesis, not a law.

A useful empirical test would compare systems with different measured
value gradients while controlling for resource availability and task
complexity.

------------------------------------------------------------------------

## C4. Value Transformation, Dissipation, and Regeneration

> **Status note:** In v0.2, “dissipation” is a candidate systems-level
> description of declining, dispersing, or becoming less recoverable
> actionable value. It is not assumed to be identical to physical heat
> dissipation. Whether it has explanatory content beyond ordinary value
> loss or redistribution remains an open research question.

Data processing should not automatically be classified as heating.

A transformation is "heating" only if the relevant actionable-value
measure increases:

$$
\Delta \Theta_D > 0
$$

Likewise, a transformation is "cooling" only if:

$$
\Delta \Theta_D < 0
$$

Processing can therefore:

- increase value;
- decrease value;
- preserve value;
- redistribute value;
- reveal previously latent value;
- destroy useful information;
- create new data through interaction.

Consumption can also create new value through feedback.

Therefore:

> **Processing is not intrinsically heating, and consumption is not
> intrinsically cooling.**

The framework instead studies the measured change in actionable value.

### Regeneration

A system can generate new actionable value through:

- feedback;
- interaction;
- aggregation;
- model updating;
- new observations;
- recombination;
- social coordination;
- discovery.

This is why data-value dynamics are better represented as a branching
process than as a one-way heat-loss cycle.

------------------------------------------------------------------------

## C5. Value Balance, Not Literal Conservation

The original "data value conservation law" is replaced by a more
defensible **value-balance framework**.

A generic accounting identity is:

$$
V_{\mathrm{out}}=V_{\mathrm{in}}+V_{\mathrm{external}}+V_{\mathrm{interaction}}-V_{\mathrm{loss}}
$$

The terms require domain-specific operational definitions.

This does **not** assert that total value is physically conserved.

Instead, it asks whether observed value changes can be accounted for
through:

- external inputs;
- transformations;
- interactions;
- feedback;
- losses;
- redistribution;
- measurement effects.

The scientific question becomes:

> **Can changes in actionable value be systematically accounted for and predicted?**

This is an accounting framework, not a conservation law. Its terms must be
operationalized independently before the framework can make a falsifiable
prediction.

This is substantially weaker than literal conservation and therefore
more compatible with empirical data systems.

------------------------------------------------------------------------

## C6. Local Value-Gradient Collapse

The original concept of universal "data heat death" is replaced by a
local and measurable hypothesis.

Let the distribution of data temperatures in a system at time $t$ be $\Theta_D(t)$.

A candidate diagnostic for gradient diversity is:

$$
G_D(t)=\mathop{\mathrm{Var}}_{T\sim \Theta_D(t)}[T]
$$

A local value-gradient collapse may be defined provisionally as:

$$
G_D(t)\to 0 \quad \text{as } t\to\infty
$$

under conditions where meaningful differentiation in actionable value
disappears.

This does not imply that all data disappear or become useless.

It means that the system loses sufficient differences in actionable
value to support useful differentiation or directed work.

Possible causes include:

- excessive diffusion;
- redundancy;
- stale information;
- universal access;
- decision saturation;
- loss of context;
- organizational rigidity.

Open systems may avoid such collapse through new observations, new
resources, interaction, learning, and feedback.

------------------------------------------------------------------------

## C7. Muse Homeostasis

**Muse Homeostasis (MH)** is the capacity of a data system to maintain a
usable actionable-value gradient through feedback, adaptation, recovery,
and continuous exchange with its environment.

Formally:

$$
\mathrm{MH}
\neq
\text{equilibrium}
$$

Instead:

$$
\mathrm{MH}
\approx
\text{gradient maintenance under perturbation}
$$

The key transition is from a **state** to a **capacity**.

The term **Muse** refers to the system's capacity to generate or sustain conditions for useful cognition and action; **homeostasis** denotes dynamic maintenance rather than equilibrium.

A system is not in MH merely because its current state looks stable. It
exhibits MH when it can remain operational under perturbation by sensing
changes, adjusting behavior, recovering from losses, and regenerating
useful value.

------------------------------------------------------------------------

# 6. Data-Thermodynamic Feedback

**Data-Thermodynamic Feedback (DTF)** is the mechanism through which a
data system changes its future data intake, processing, output, or
resource-allocation policy in response to changes in actionable value
produced by its actions.

A minimal loop is:

$$
D_t
\rightarrow
\Theta_t
\rightarrow
A_t
\rightarrow
V_t
\rightarrow
F_t
\rightarrow
\pi_{t+1}
$$

where:

- $D_t$ = current data state;
- $\Theta_t$ = estimated data temperature;
- $A_t$ = action;
- $V_t$ = resulting actionable value;
- $F_t$ = feedback;
- $\pi_{t+1}$ = next policy.

A candidate policy update is:

$$
\pi_{t+1}=f(\pi_t,F_t)
$$

DTF is not equivalent to generic feedback control. Its distinctive
research question is whether feedback organized around
**actionable-value change** produces measurable improvements in
data-system behavior.

Feedback may be:

- positive;
- negative;
- delayed;
- noisy;
- regenerative;
- adversarial.

### DTF and waste-heat recovery

Waste-heat recovery is only one special case of feedback-driven
recovery.

Feedback may instead change:

- what the system remembers;
- what it forgets;
- what it samples;
- how deeply it processes;
- when it acts;
- how it allocates computational resources.

------------------------------------------------------------------------

# 7. Muse Homeostasis: Mechanisms

MH can be decomposed into four functional capabilities.

## 7.1 Sensing

The system estimates changes in actionable value.

$$
D_t \rightarrow \Theta_t
$$

Without some form of sensing, MH cannot be operationally demonstrated.

------------------------------------------------------------------------

## 7.2 Regulation

The system adjusts:

- data intake;
- processing depth;
- output strategy;
- resource allocation;
- retention policy.

------------------------------------------------------------------------

## 7.3 Recovery

After perturbation, the system returns to a usable operating regime.

Recovery does not require returning to the previous state.

The relevant criterion is:

> **Does the system regain sufficient capacity for useful action?**

------------------------------------------------------------------------

## 7.4 Regeneration

The system obtains or creates new actionable value through interaction
with its environment.

Possible sources include:

- new observations;
- user feedback;
- model updating;
- external data;
- recombination;
- social interaction.

Thus MH is inherently compatible with nonequilibrium operation.

------------------------------------------------------------------------

# 8. Thermal Elasticity

**Thermal Elasticity** is a candidate measure of a system's
responsiveness to changes in its external actionable-value environment.

A provisional formulation is:

$$
\mathcal{E}_D=\frac{d\Theta_{\mathrm{internal}}}{d\Theta_{\mathrm{external}}}
$$

This is not yet an established metric.

The intended interpretation is:

- $\mathcal{E}_D \rightarrow 0$: weak response to external change;
- excessive responsiveness: internal state may simply track external
    volatility;
- an intermediate controllable regime may permit both sensitivity and
    regulation.

Thermal Elasticity is **one candidate property of MH, not a synonym for MH**.

A mature formulation must define:

1. what counts as internal temperature;
2. what counts as external temperature;
3. the time scale of response;
4. the perturbation regime;
5. the acceptable operating range.

------------------------------------------------------------------------

# 9. MH Failure Modes

MH provides a way to classify several candidate failure regimes.

## 9.1 Gradient Collapse

The distribution of actionable values becomes insufficiently
differentiated:

$$
G_D(t) \rightarrow 0
$$

Possible symptoms:

- excessive redundancy;
- stale data;
- low decision differentiation;
- inability to generate useful work.

------------------------------------------------------------------------

## 9.2 Overheating

The rate or volume of information entering or being processed exceeds
the system's capacity for evaluation and regulation.

Possible symptoms include:

- information overload;
- decision latency;
- unstable model outputs;
- excessive redundant processing.

These are candidate analogies, not thermodynamic identities.

------------------------------------------------------------------------

## 9.3 Overcooling

The system loses too much useful variation or becomes excessively
resistant to new input.

Possible symptoms include:

- data stagnation;
- obsolete models;
- low exploratory behavior;
- excessive retention of historical assumptions.

------------------------------------------------------------------------

## 9.4 Recovery Failure

A system experiences perturbation but cannot return to a usable
operating regime.

This may be a more operational definition of "homeostatic failure" than
simple deviation from equilibrium.

------------------------------------------------------------------------

# 10. Speculative Extensions

Core theory should remain small.

Specialized domains may generate additional mechanisms that extend MH
without becoming part of the core theory.

For example, the *Mindsea* topic explores:

- **Forgetting Elasticity** --- the ability of a cognitive data system
    to release, downweight, or reorganize low-value information and
    subsequently recover a usable state.
- **Data Vacuum** --- a transient state in which an existing
    informational/value structure has been released or removed while a
    replacement structure has not yet formed.

These concepts are **speculative extensions of MH**, not established
core laws.

They are developed in the *Mindsea* topic rather than in this document.

------------------------------------------------------------------------

# 11. Relation to Existing Research

Data Thermodynamics does not claim to replace existing disciplines.

It attempts to connect several existing research programs around a
common problem: the dynamics of actionable value in data systems.

## 11.1 Information Theory

Shannon's information theory provides formal tools for uncertainty,
information, coding, and communication.

Information entropy should not be casually identified with actionable
value.

The relevant question is whether information-theoretic quantities can
help operationalize components of data value or temperature.

------------------------------------------------------------------------

## 11.2 Information Thermodynamics

Information thermodynamics studies relationships among information,
physical work, entropy production, feedback, and thermodynamic cost.

This is a direct scientific reference point for evaluating whether
thermodynamic language can be transferred responsibly into data-system
analysis.

------------------------------------------------------------------------

## 11.3 Thermodynamics of Computation

Landauer's work established a physical relationship between logically
irreversible computation and heat generation.

This supports a precise claim:

> **Physical information processing can have thermodynamic costs.**

It does **not** establish that semantic data value itself is
thermodynamic heat.

That distinction is essential.

------------------------------------------------------------------------

## 11.4 Data Valuation

Data valuation research already develops quantitative methods for
estimating the contribution or utility of data.

For example, Data Shapley evaluates the contribution of individual
training data to model performance.

The 2025 systematic review literature shows that quantitative data
valuation is already a substantial and growing research area, while also
noting heterogeneity in definitions and methods.

Data Thermodynamics should therefore be treated as a proposed synthesis
or extension of existing data-valuation questions, not as the invention
of data valuation itself.

------------------------------------------------------------------------

## 11.5 Decision Theory and Value of Information

Decision theory provides a natural route for operationalizing actionable
value.

A candidate quantity is expected value of information:

$$
\mathrm{VOI}=\mathbb{E}[U(a \mid D)]-\max_a U(a)
$$

or related marginal-utility formulations.

Such quantities may provide empirical candidates for $\Theta_D$.

------------------------------------------------------------------------

## 11.6 Complex Systems and Nonequilibrium Science

Complex-systems research provides models of:

- emergence;
- adaptation;
- networks;
- feedback;
- self-organization;
- nonequilibrium states.

These fields may be more appropriate than literal equilibrium
thermodynamics for several aspects of MH.

------------------------------------------------------------------------

# 12. Alternative Metaphor Test

Data Thermodynamics should survive removal of thermodynamic terminology.

Candidate alternatives include:

  -----------------------------------------------------------------------
  Framework               Main question           Main layer
  ----------------------- ----------------------- -----------------------
  Data Thermodynamics     How does actionable     gradients, flows,
                          value flow, dissipate,  dissipation
                          and remain usable?

  Data Chemistry          How do data structures  reactions, structure
                          combine and transform?  

  Data Ecology            How do data entities    relationships,
                          compete, cooperate, and ecosystems
                          occupy niches?

Data Fluid Dynamics     How do data flows move  flow fields
                          through boundaries and  
                          networks?
  -----------------------------------------------------------------------

These are not mutually exclusive.

The framework's scientific value depends on whether its core
propositions remain meaningful after the metaphor is removed.

A successful test is therefore:

> **Can C1--C7 be stated, measured, and falsified without requiring the
> reader to believe that data literally behaves like heat?**

If not, the theory has not yet escaped metaphor.

------------------------------------------------------------------------

# 13. Provisional Mathematical Vocabulary

The following symbols are retained as a common language but are
explicitly provisional.

  -----------------------------------------------------------------------
  Concept                 Symbol                  Status
  ----------------------- ----------------------- -----------------------
  Actionable value        $V$                     candidate operational
                                                  quantity

  Data temperature        $\Theta_D$              candidate relational
                                                  quantity

  Value gradient          $\nabla\Theta_D$        candidate derived
                                                  quantity

  Value-gradient          $G_D$                   candidate diagnostic
  diversity

  Feedback signal         $F$                     domain-dependent

  Policy                  $\pi$                   control variable

  Thermal elasticity      $\mathcal{E}_D$         candidate metric

  Data heat / transfer    $Q_D$                   metaphorical unless
                                                  independently
                                                  operationalized

  Data entropy            $S_D$                   not yet operationalized

  Data exergy             $E_D$                   speculative candidate

Data wavefunction       $\Psi_D$                speculative analogy
                                                  only
  -----------------------------------------------------------------------

The framework intentionally avoids assigning invented physical units at
this stage.

------------------------------------------------------------------------

# 14. Why the Classical Thermodynamic Equations Are Not Yet Core Laws

Earlier versions used direct analogues such as:

$$
\Delta U_D = Q_D - W_D
$$

and:

$$
\eta=\frac{W_D}{Q_D}\leq1-\frac{\Theta_{\mathrm{cold}}}{\Theta_{\mathrm{hot}}}
$$

These equations should now be treated as **candidate templates**, not
established laws.

Before such equations can enter the core theory, the following must be
demonstrated:

1. the quantities have operational definitions;
2. they can be measured independently;
3. the balance relation survives empirical testing;
4. the efficiency bound follows from explicit assumptions rather than
    analogy;
5. alternative models perform worse or reveal less structure.

Until then, these equations belong to the framework's modeling toolbox
rather than its laws.

------------------------------------------------------------------------

# 15. Research Questions

The current research program can be organized into six questions.

### R1. Can actionable value be measured?

Can a value function $V(D \mid C,T,A,R)$ be operationalized across real
tasks?

### R2. Can data temperature be measured?

Can a marginal value quantity serve as a stable and useful $\Theta_D$?

### R3. Do value gradients predict directed work?

Does measured $\nabla\Theta_D$ predict resource allocation, decision
urgency, or expected utility?

### R4. Can value changes be accounted for?

Can observed value changes be decomposed into inputs, interactions,
transformations, and losses?

### R5. Can local value-gradient collapse be detected?

Can $G_D(t)$ or related measures predict system stagnation, redundancy,
or loss of decision differentiation?

### R6. Can MH improve resilience?

Do systems equipped with value-sensitive feedback recover more
effectively from perturbations than appropriate baselines?

------------------------------------------------------------------------

# 16. Research Method

## 16.1 Falsification First

Every core proposition should have:

- operational definition;
- measurable variables;
- baseline model;
- predicted observation;
- falsification condition.

A proposition that cannot be tested should remain philosophical or
metaphorical rather than being presented as scientific.

------------------------------------------------------------------------

## 16.2 Operationalize Data Temperature

Candidate operationalizations include:

- expected value of information;
- marginal decision utility;
- contribution to predictive performance;
- conditional mutual information;
- task-specific utility gain;
- economic marginal benefit;
- time-decay-adjusted utility.

Different operationalizations may produce different "temperatures."

That is not necessarily a failure. It may indicate that data temperature
is inherently task-relative.

------------------------------------------------------------------------

## 16.3 Baseline Comparison

Every empirical study should compare the proposed metric with existing
approaches.

Potential baselines include:

- Shapley-style data valuation;
- leave-one-out contribution;
- predictive utility;
- information-theoretic relevance;
- economic valuation;
- heuristic freshness or popularity scores.

A Data Thermodynamics metric is useful only if it provides additional
explanatory or predictive power.

------------------------------------------------------------------------

## 16.4 Dynamic Modeling

Candidate models include:

- stochastic processes;
- dynamical systems;
- reaction-diffusion models;
- network flow models;
- control systems;
- nonequilibrium models.

Partial differential equations may be useful in appropriate settings,
but they should not be assumed to be necessary.

------------------------------------------------------------------------

## 16.5 Empirical Validation

Potential datasets include:

- social-media propagation;
- recommendation systems;
- model training logs;
- data marketplace transactions;
- organizational access logs;
- AI-agent trajectories;
- human decision experiments.

The key requirement is repeated measurement of value under controlled
context.

------------------------------------------------------------------------

## 16.6 Engineering Validation

Potential interventions include:

- value-aware data retention;
- temperature-aware caching;
- feedback-based data acquisition;
- AI-agent resource allocation;
- adaptive memory policies;
- data-quality recovery loops.

Engineering success is evidence of utility, not proof of the underlying
thermodynamic metaphor.

------------------------------------------------------------------------

# 17. Priority Research Program

The project should prioritize research in the following order.

### Priority 1 --- Data Temperature

Establish whether a useful operational quantity can be defined.

### Priority 2 --- Value Gradient

Test whether differences in actionable value predict work or resource
allocation.

### Priority 3 --- Data-Thermodynamic Feedback

Test whether value-sensitive feedback improves system performance or
resilience.

### Priority 4 --- Muse Homeostasis

Develop metrics for recovery, adaptation, and maintenance under
perturbation.

### Priority 5 --- Value Balance

Determine whether observed value changes can be systematically accounted
for.

### Priority 6 --- Local Gradient Collapse

Test whether value-gradient collapse is a measurable and predictive
system condition.

### Priority 7 --- Efficiency Bounds

Only after the previous concepts are operationalized should Carnot-like
or other upper-bound claims be investigated.

------------------------------------------------------------------------

# 18. Applications

The most promising initial applications are those where actionable value
can be measured.

  -----------------------------------------------------------------------
  Domain                              Candidate application
  ----------------------------------- -----------------------------------
  AI agents                           value-sensitive action selection
                                      and resource allocation

  Machine learning                    data acquisition, selection,
                                      retention, and valuation

  Data governance                     dynamic retention and lifecycle
                                      management

  Information retrieval               relevance decay and query-time
                                      value

  Recommendation systems              context-dependent data temperature

  Social information systems          propagation, saturation, and
                                      value-gradient collapse

  Organizational systems              information overload and decision
                                      resilience

  Privacy and data markets            value accounting and contribution
                                      analysis

  Knowledge systems                   regeneration, forgetting, and
                                      recovery

Human-AI systems                    feedback-driven adaptation
  -----------------------------------------------------------------------

The AI-agent domain is currently the most promising entry point because
action, feedback, resource allocation, and measurable utility are
naturally present.

------------------------------------------------------------------------

# 19. Learning and Research Path

## Foundations

1. Probability and statistics
2. Information theory
3. Decision theory
4. Thermodynamics and statistical mechanics
5. Machine learning
6. Data engineering
7. Complex systems
8. Economics and mechanism design
9. Scientific philosophy and falsifiability

## Core research modules

1. Data Temperature Measurement
2. Value Gradient Dynamics
3. Data-Thermodynamic Feedback
4. Muse Homeostasis
5. Value Accounting
6. Data Lifecycle and Regeneration
7. Empirical Data Valuation
8. Comparative Metaphor Methodology

## Advanced directions

- nonequilibrium information systems;
- data valuation economics;
- adaptive AI systems;
- cognitive data systems;
- social information dynamics;
- networked data ecosystems.

------------------------------------------------------------------------

# 20. Theory Branches

The following branches are research directions, not established
subdisciplines.

  -----------------------------------------------------------------------
  Branch                              Focus
  ----------------------------------- -----------------------------------
  Data Thermodynamic Physics          gradients, dissipation,
                                      nonequilibrium models

  Data Thermodynamic Economics        valuation, allocation, markets,
                                      incentives

  Data Thermodynamic Biology          biological information processing
                                      and homeostasis

  Data Thermodynamic Sociology        information propagation and
                                      collective dynamics

  Data Thermodynamic Engineering      systems, feedback, lifecycle,
                                      recovery

Data Thermodynamic Cognition        memory, forgetting, attention,
                                      decision systems
  -----------------------------------------------------------------------

These branches should be developed only when the corresponding core
concepts become sufficiently formalized.

------------------------------------------------------------------------

# 21. Boundaries and Non-Claims

Data Thermodynamics currently does **not** claim that:

1. data is literally heat;
2. semantic value is physically conserved;
3. data has an observer-independent scalar temperature;
4. all processing increases value;
5. consumption always decreases value;
6. all open systems avoid value-gradient collapse;
7. MH is a natural law;
8. Carnot efficiency directly applies to data processing;
9. quantum mechanics describes ordinary data semantics;
10. AI systems possess consciousness because they process information;
11. biological homeostasis proves MH;
12. a metaphor becomes scientific merely because it has equations.

These are explicit boundaries against overextension.

------------------------------------------------------------------------

# 22. Speculative Status of Quantum and Cosmological Analogies

Earlier versions included a quantum-like data temperature state:

$$
|\Psi_D\rangle=\sum_i c_i|\Theta_i\rangle
$$

This may be retained as a speculative analogy.

It should not be used as evidence that data literally exists in quantum
superposition.

Likewise, analogies between:

- cosmic expansion and data generation;
- black holes and information boundaries;
- cosmological heat death and data-system stagnation;

belong to speculative topics unless independently derived and tested.

------------------------------------------------------------------------

# 23. Authorship and Tool-Assisted Development

The conceptual development of Data Thermodynamics is author-led.

AI systems have been used as research and writing tools for:

- expanding conceptual branches;
- comparing formulations;
- organizing arguments;
- synthesizing literature;
- identifying counterarguments;
- drafting and revising prose.

This tool-assisted process does not imply that the concepts originated
from an AI model.

Scientific claims remain subject to independent verification.

------------------------------------------------------------------------

# 24. Core Minimal Set

If the framework had to be reduced to its smallest defensible form, it
would contain:

1. **Contextual Value** --- data value depends on context and task.
2. **Data Temperature** --- a candidate measure of marginal actionable
    value.
3. **Value Gradient** --- differences in actionable value can guide
    resource allocation.
4. **Transformation and Dissipation** --- data processing can increase,
    decrease, redistribute, or regenerate value.
5. **Value Balance** --- changes in value should be accounted for
    rather than assumed conserved.
6. **Local Gradient Collapse** --- useful differentiation may disappear
    under diffusion, redundancy, or stagnation.
7. **Muse Homeostasis** --- systems can be studied by their ability to
    sense, regulate, recover, and regenerate useful value gradients.
8. **Data-Thermodynamic Feedback** --- value changes can be fed back
    into future policy.

Everything else is downstream.

------------------------------------------------------------------------

# 25. Conclusion

Data Thermodynamics began with the phrase:

> **Data itself possesses heat.**

The mature version of the framework does not require that sentence to be
literally true.

Its stronger proposition is narrower:

> **Data systems contain context-dependent actionable value, and that
> value can form gradients, flow through transformations, dissipate,
> regenerate, and be maintained through feedback.**

Thermodynamics supplies a vocabulary for asking whether these processes
have structural regularities.

Information theory supplies measures of information and uncertainty.

Decision theory supplies measures of actionable utility.

Data valuation supplies existing approaches to quantifying contribution.

Control theory supplies feedback and adaptation.

Complex-systems research supplies models of nonequilibrium organization.

Data Thermodynamics attempts to connect these perspectives around one
question:

> **How can a data system maintain useful value gradients while
> continuously transforming the information available to it?**

The answer is not established.

That is the research program.

------------------------------------------------------------------------

## References and Starting Points

- Shannon, C. E. (1948). *A Mathematical Theory of Communication*.
    Bell System Technical Journal, 27(3), 379--423; 27(4), 623--656.
- Landauer, R. (1961). *Irreversibility and Heat Generation in the
    Computing Process*. IBM Journal of Research and Development, 5(3),
    183--191.
- Ghorbani, A., & Zou, J. (2019). *Data Shapley: Equitable Valuation
    of Data for Machine Learning*. Proceedings of ICML, PMLR 97,
    2242--2251.
- Jia, R., et al. (2019). *Towards Efficient Data Valuation Based on
    the Shapley Value*. Proceedings of AISTATS, PMLR 89, 1167--1176.
- Ebiele, M., Bendechache, M., & Brennan, R. (2025). *Quantitative
    Data Valuation Methods: A Systematic Review and Taxonomy*. ACM
    Journal of Data and Information Quality, 17(2).
- Prigogine, I. Work on dissipative structures and nonequilibrium
    thermodynamics.
- Schrödinger, E. (1944). *What Is Life?* --- historical source for
    the "negative entropy" discussion, not a direct scientific
    foundation for Data Thermodynamics.
- Information thermodynamics, stochastic thermodynamics, and
    thermodynamics of computation constitute the broader physical
    literature relevant to the framework.

The references above provide scientific context, not validation.

------------------------------------------------------------------------

© Mulander-J, CC BY-SA 4.0
