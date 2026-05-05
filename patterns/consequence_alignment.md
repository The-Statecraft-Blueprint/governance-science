# Consequence Alignment

**Status**: Draft  
**Pattern Category**: Accountability Mechanism  
**Version**: 1.0  
**Last Updated**: April 2026

---

## Intent

Ensure decision-makers experience the consequences of their decisions by designing structural connections between choices and outcomes—creating self-correcting systems where feedback loops enable learning and adjustment.

---

## Motivation

Governance systems frequently exhibit a structural disconnect: those who make decisions don't bear the consequences. Legislators pass unfunded mandates, executives make commitments that bind successors, regulators face no personal cost for regulatory capture, and current majorities externalize costs to future generations.

When this happens, the system loses its self-correcting capacity. Decision-makers receive no feedback signal indicating whether their decisions were good or bad. Multiple decision qualities produce the same outcome for the decision-maker. The system has high [degeneracy](../DSL/degeneracy.md) in its accountability relationships.

The principle is simple: **good design routes costs back to the decision-maker.** This is not primarily a moral claim about fairness (though it may also be fair). It's an engineering observation about feedback loops. Systems where decision-makers bear costs are self-correcting. Systems where costs route elsewhere accumulate dysfunction.

This matters because exhortations to "be accountable" don't work when structural disconnects exist. You can't will yourself to receive feedback that the system doesn't provide. Accountability requires structural connections between decisions and consequences—mechanisms that make decision-makers feel the effects of their choices.

The pattern applies across domains:
- **Fiscal policy**: Do legislators bear the costs of spending decisions?
- **Regulation**: Do regulators face consequences for capture or poor rules?
- **Delegation**: Do overseers bear costs when delegated authority fails?
- **Intergenerational**: Do current decision-makers face any proxy for future costs?

Where consequence alignment is weak, dysfunction accumulates. Where it's strong, systems self-correct. The pattern describes how to design for strong alignment.

---

## Applicability

### Use This Pattern When:

- **Decision-makers are insulated from consequences**: Costs fall on others, other times, or other jurisdictions rather than on decision-makers
- **Accountability mechanisms are failing**: Oversight exists but doesn't change behavior because decision-makers face no differential consequences
- **Feedback loops are broken**: Decision-makers cannot observe whether their decisions worked
- **Recurring dysfunction despite personnel change**: Same problems persist regardless of who holds office—suggesting structural rather than individual failure
- **High degeneracy**: Good and bad decisions produce same outcomes for decision-maker

### Don't Use This Pattern When:

- **Risk-pooling is the goal**: Insurance, social safety nets, and collective action legitimately weaken individual consequence alignment
- **Consequences are inherently diffuse**: Some decisions genuinely affect many parties in ways that can't be concentrated
- **Short-term consequences conflict with long-term goals**: Immediate consequence alignment might encourage short-termism
- **Measurement is impossible**: Can't route consequences if you can't measure them
- **Consequence attribution is unclear**: When multiple factors cause outcomes, assigning consequences to specific decisions may be arbitrary

### Warning Signs This Isn't the Right Approach:

- Using consequence alignment to justify punitive measures rather than feedback mechanisms
- Ignoring legitimate reasons for consequence diffusion (solidarity, risk-sharing)
- Attempting to create consequence alignment where causal chains are too complex or long
- Treating consequence alignment as the only accountability mechanism (ignoring transparency, oversight, elections)

---

## Structure

### Visual Structure

```
Decision Point (Authority making choice)
    ↓ [Decision made]
    
Consequence Mechanism (Structural connection)
    ↓ [Routes outcomes back to decision-maker]
    
Feedback Reception (Decision-maker experiences consequence)
    ↓ [Information received about decision quality]
    
Adjustment Capacity (Ability to change behavior)
    ↓ [Future decisions can incorporate learning]
    
Decision Point (Next decision cycle)
```

### Key Components:

1. **Decision Authority**
   - Purpose: Actor or body making choices that affect others
   - Characteristics: Has discretion, faces multiple options, choices have consequences

2. **Consequence Mechanism**
   - Purpose: Structural connection routing outcomes to decision-maker
   - Characteristics: Automatic or institutional, not dependent on enforcement discretion, operates with low degeneracy

3. **Feedback Channel**
   - Purpose: Conveys information about decision quality to decision-maker
   - Characteristics: Timely (before next decision cycle), interpretable (decision-maker can understand what it means), attributable (connects to specific decisions)

4. **Adjustment Capacity**
   - Purpose: Enables decision-maker to change future behavior based on feedback
   - Characteristics: Authority to modify approach, incentive to do so, capability to learn

### Mechanism:

The pattern works through a feedback cycle:

1. **Decision**: Authority makes choice from available options
2. **Consequence**: Choice produces outcomes—costs and benefits distributed somehow
3. **Routing**: Structural mechanism ensures some consequences flow to decision-maker (not only to others)
4. **Reception**: Decision-maker experiences consequences, receiving information about decision quality
5. **Learning**: Decision-maker incorporates feedback into future decisions
6. **Adjustment**: Future decisions improve based on accumulated learning
7. **Cycle Repeats**: Continuous improvement through functional feedback

The key structural question is **step 3: routing**. Without a mechanism routing consequences to the decision-maker, steps 4-6 don't happen. The decision-maker is flying blind, and the system cannot self-correct.

Strong consequence alignment means:
- Low [degeneracy](../DSL/degeneracy.md) (different decision qualities produce distinguishable consequences for decision-maker)
- High [causal determinism](../DSL/causal_determinism.md) (consequences reliably follow decisions)
- Short time lag (feedback arrives before next decision cycle)
- Clear attribution (decision-maker can identify which decision caused which consequence)

---

## Participants

### Decision-Maker (Legislator, Executive, Regulator, Board)

**Responsibilities:**
- Exercise discretion in choosing among options
- Receive and interpret feedback about past decisions
- Adjust future behavior based on learning

**Requirements:**
- Authority to make meaningful choices
- Capacity to receive feedback
- Ability to modify approach based on learning
- Incentive structure that makes consequences salient

### Consequence Mechanism (Electoral, Market, Institutional, Automatic)

**Responsibilities:**
- Route some portion of decision consequences to decision-maker
- Operate with sufficient determinism and low degeneracy
- Function regardless of enforcement discretion or political will

**Requirements:**
- Structural connection between decision and consequence
- Sufficient independence from decision-maker's control
- Timely operation (consequences arrive before relevant decision cycles)
- Measurement capacity (outcomes must be observable)

### Affected Parties (Citizens, Future Generations, Other Jurisdictions)

**Responsibilities:**
- Bear consequences of decisions (whether aligned or not)
- Provide information about outcomes (when possible)
- Advocate for stronger alignment where consequences are misrouted

**Requirements:**
- Voice mechanisms to communicate consequences
- Representation in decision processes (where appropriate)
- Protection when consequence alignment isn't possible

### Evaluation Mechanism (Auditor, Oversight, Independent Assessment)

**Responsibilities:**
- Measure decision quality and outcomes
- Assess whether consequence mechanisms are functioning
- Identify gaps in alignment

**Requirements:**
- Independence from decision-maker
- Capacity to measure relevant outcomes
- Authority to report findings
- Connection to consequence mechanisms (findings should affect decision-maker)

---

## Collaborations

### 1. Decision-Maker → Decision → Outcomes
**Nature**: Choices produce consequences distributed across affected parties
**Exchange**: Decision-maker expends authority/political capital, produces outcomes

### 2. Consequence Mechanism → Decision-Maker
**Nature**: Structural routing of outcomes back to decision-maker
**Exchange**: Consequences flow to decision-maker (electoral, financial, reputational, institutional)

### 3. Feedback → Learning → Adjustment
**Nature**: Information about decision quality enables behavior change
**Exchange**: Decision-maker receives signal, interprets meaning, modifies future approach

### 4. Evaluation Mechanism → Consequence Mechanism
**Nature**: Independent assessment strengthens routing
**Exchange**: Evaluation findings feed into consequence mechanisms (published reports affect elections, audits trigger institutional consequences)

---

## Consequences

### Benefits (✅)

- **Self-correcting systems**: Decision-makers naturally adjust when they feel consequences
- **Reduced need for external enforcement**: Consequences are structural, not dependent on political will
- **Learning over time**: Accumulated feedback improves decision quality
- **Aligned incentives**: Decision-makers want to decide well because they bear costs of deciding poorly
- **Functional accountability**: Oversight becomes meaningful when connected to consequences
- **Reduced degeneracy**: Different decision qualities produce distinguishable outcomes

### Costs (⚠️)

- **May reduce risk-taking**: Decision-makers avoid beneficial risks if they bear all downside
- **Measurement challenges**: Consequences must be measurable to route them
- **Attribution complexity**: Multiple decisions contribute to outcomes; routing to specific decisions is imprecise
- **Time lag problems**: Long-term consequences can't provide timely feedback
- **May conflict with solidarity**: Collective responsibility deliberately weakens individual consequence alignment
- **Design complexity**: Creating structural consequence mechanisms is harder than exhorting accountability

### Risks (🚨)

- **Perverse consequences**: If wrong outcomes are measured, decision-makers optimize for wrong things
- **Gaming**: Decision-makers may manipulate consequence mechanisms rather than improve decisions
- **Short-termism**: If only immediate consequences route back, long-term thinking suffers
- **Scapegoating**: Consequence mechanisms may be used to punish rather than create feedback
- **Excessive risk aversion**: Too-strong consequence alignment may prevent necessary bold action
- **Measurement capture**: Those being measured may corrupt the measurement

---

## Implementation

### Prerequisites:

- **Measurable outcomes**: Must be able to observe consequences to route them
- **Attributable decisions**: Must be able to connect outcomes to specific decisions
- **Structural capacity**: Must be able to create mechanisms that route consequences
- **Decision-maker receptivity**: Decision-maker must be capable of receiving feedback
- **Legitimate baseline**: Must have normative basis for claiming certain consequences should route back

### Implementation Steps:

**1. Map the Consequence Flows**

What to do:
- Identify who currently bears costs and benefits of decisions
- Trace the causal chain from decision to outcomes
- Note where decision-maker is insulated from consequences
- Document time lags between decision and consequence

Key considerations:
- Be thorough—consequences often route in unexpected directions
- Include future costs, not just present ones
- Consider diffuse costs that are real but not concentrated

Success criteria:
- Clear map of who bears what consequences
- Identification of where decision-maker is insulated
- Understanding of time dynamics

**2. Identify Alignment Gaps**

What to do:
- Compare consequence flows to normative baseline (who *should* bear costs?)
- Identify specific gaps where decision-makers are insulated
- Prioritize gaps by significance (amount of cost misrouted) and tractability (ability to realign)
- Assess whether gaps serve legitimate purposes (risk-sharing, collective action)

Key considerations:
- Not all consequence misrouting is bad—some serves legitimate purposes
- Focus on gaps that create accountability failure
- Consider political feasibility of addressing gaps

Success criteria:
- Prioritized list of alignment gaps
- Assessment of which gaps are problems vs. features
- Tractability analysis

**3. Design Routing Mechanisms**

What to do:
- For each priority gap, design structural mechanism to route consequences
- Ensure mechanism has low degeneracy (different decisions → different consequences)
- Ensure mechanism has high determinism (consequences reliably follow decisions)
- Build in appropriate time dynamics (feedback before next decision cycle)

Key considerations:
- Prefer automatic mechanisms over discretionary enforcement
- Consider unintended consequences of new mechanisms
- Test mechanism against gaming and manipulation
- Ensure mechanism measures the right outcomes

Success criteria:
- Specific mechanism design for each priority gap
- Low degeneracy and high determinism
- Robustness to gaming

**4. Implement Mechanisms**

What to do:
- Create structural connections through legislation, rule changes, or institutional design
- Establish measurement systems for relevant outcomes
- Set up evaluation and monitoring
- Communicate to decision-makers what consequences will now route to them

Key considerations:
- Phase in where possible to allow adjustment
- Monitor for unintended effects
- Maintain flexibility to adjust mechanisms

Success criteria:
- Mechanisms operational
- Measurement functioning
- Decision-makers aware of consequence alignment

**5. Evaluate and Adjust**

What to do:
- Monitor whether decision quality improves
- Assess whether mechanisms are functioning as designed
- Identify gaming or manipulation
- Adjust mechanisms based on evidence

Key considerations:
- Consequence alignment is means to end (better decisions), not end in itself
- If decisions don't improve, mechanism may be targeting wrong outcomes
- Balance stability with adaptability

Success criteria:
- Evidence of improved decision quality
- Mechanisms functioning as designed
- Ongoing evaluation capacity

### Variations:

**Variation A: Electoral Alignment**

When to use: For elected officials whose decisions should reflect constituent interests

How it differs:
- Consequence mechanism is electoral competition
- Feedback channel is voter response to decision outcomes
- Requires competitive elections (safe seats have weak alignment)
- Time dynamics tied to electoral cycles

Trade-offs: Works only in competitive contexts; time lag can be long; voters must be able to attribute outcomes to decisions

**Variation B: Market Alignment**

When to use: For actors whose decisions have economic consequences

How it differs:
- Consequence mechanism is market response (profit/loss, prices, investment)
- Feedback is automatic and continuous
- Requires functioning markets and property rights
- Time dynamics can be rapid

Trade-offs: Works only where market signals are accurate; can't handle externalities without additional structure; may conflict with non-market values

**Variation C: Institutional Alignment**

When to use: For officials within institutions where external accountability is weak

How it differs:
- Consequence mechanism is internal (performance evaluation, budget authority, professional reputation)
- Feedback channel is institutional oversight
- Requires well-designed institutional structures
- Time dynamics tied to evaluation cycles

Trade-offs: Depends on institutional integrity; internal metrics can be gamed; may not align with external stakeholder interests

**Variation D: Automatic Alignment**

When to use: For decisions where discretion should be minimal

How it differs:
- Consequence mechanism is built into policy structure (automatic stabilizers, trigger mechanisms)
- Feedback is instantaneous—mechanism *is* the consequence
- Requires clear rules and measurable triggers
- Time dynamics are immediate

Trade-offs: Rigid; can't adapt to novel circumstances; requires upfront design work; may produce inappropriate responses when conditions change

---

## Known Uses

### Known Use 1: PAYGO Budget Rules (United States, 1990-2002, 2010-present)

**Context:**

Federal deficit spending routes costs to future taxpayers while current legislators receive credit for spending. Pay-As-You-Go rules attempted to create consequence alignment by requiring that new spending be offset by cuts or revenue increases.

**Pattern Application:**

**Decision-makers**: Congress

**Alignment gap**: Legislators could increase spending without bearing costs (future taxpayers bear deficit costs)

**Consequence mechanism**: PAYGO requires offsets—new spending must be paired with cuts or revenue, making trade-offs explicit

**Feedback channel**: Immediate budget scoring shows consequence; vote is on complete package including offsets

**Adjustment capacity**: Legislators can modify proposals to achieve budget neutrality

**Outcomes:**

**Positive:**
- Deficit reduction in 1990s partly attributed to budget discipline under PAYGO
- Made trade-offs explicit in legislative process
- Created procedural barrier to unfunded commitments

**Negative:**
- Repeatedly waived for politically popular spending
- Doesn't apply to existing programs or mandatory spending growth
- Sunset provisions undermine durability
- Can be gamed through accounting tricks

**Lessons Learned:**

- Procedural consequence alignment can be waived if political will is insufficient
- Most effective when waiver requires difficult supermajority
- Doesn't address existing fiscal commitments—only new decisions
- Demonstrates tension between consequence alignment and political flexibility

**References:**
- Schick, Allen (2007). *The Federal Budget: Politics, Policy, Process*. Brookings Institution Press.

---

### Known Use 2: Medical Malpractice Liability (United States)

**Context:**

Medical decisions have consequences for patients. Without consequence alignment, physicians might not bear costs of negligent care. Malpractice liability creates a routing mechanism.

**Pattern Application:**

**Decision-makers**: Physicians and healthcare providers

**Alignment gap**: Poor clinical decisions harm patients; without liability, providers don't bear costs

**Consequence mechanism**: Tort liability—patients can sue for damages from negligent care

**Feedback channel**: Lawsuits, settlements, insurance premiums, reputation effects

**Adjustment capacity**: Providers can modify practice patterns, seek additional training, improve care

**Outcomes:**

**Positive:**
- Creates incentive for care quality
- Provides compensation for injured patients
- Professional reputation effects supplement legal liability
- Insurance premiums create ongoing consequence (not just when sued)

**Negative:**
- May encourage defensive medicine (over-testing, over-treatment)
- Litigation is slow and expensive
- Not all malpractice results in suits; not all suits reflect actual malpractice
- Caps and tort reform weaken alignment in some jurisdictions

**Lessons Learned:**

- Liability creates consequence alignment but can overshoot (defensive medicine)
- Insurance intermediation can stabilize consequence flows but also buffer them
- Multiple feedback channels (legal, reputational, insurance) provide redundancy
- Measurement challenges (distinguishing negligence from bad outcomes) limit precision

**References:**
- Studdert, David M., et al. (2006). "Claims, Errors, and Compensation Payments in Medical Malpractice Litigation." *New England Journal of Medicine*, 354(19): 2024-2033.

---

### Known Use 3: Performance-Based Budgeting (Various Jurisdictions)

**Context:**

Government agencies receive budgets regardless of performance. Performance-based budgeting attempts to create consequence alignment by connecting funding to outcomes.

**Pattern Application:**

**Decision-makers**: Agency leadership

**Alignment gap**: Poor performance doesn't affect agency budgets; budget process is input-based, not outcome-based

**Consequence mechanism**: Budget allocations tied to performance metrics

**Feedback channel**: Performance measurement → budget consequences → agency resources

**Adjustment capacity**: Agencies can modify operations to improve metrics

**Outcomes:**

**Positive:**
- Creates focus on outcomes rather than inputs
- Provides information for legislative oversight
- In some cases, demonstrably improved efficiency (Texas, Virginia partial implementations)

**Negative:**
- Measurement challenges—easy to measure outputs, hard to measure outcomes
- Gaming—agencies optimize for measured metrics, not actual mission
- Political override—legislatures often don't follow through on consequence mechanism
- Some public goods inherently difficult to measure

**Lessons Learned:**

- Performance-based consequence alignment requires robust measurement
- Political will to actually impose consequences is often lacking
- Works better for measurable services than for inherently unmeasurable missions
- Partial implementation may be worse than none (gaming effects without full benefits)

**References:**
- Moynihan, Donald P. (2008). *The Dynamics of Performance Management: Constructing Information and Reform*. Georgetown University Press.

---

### Known Use 4: Skin-in-the-Game Provisions (Dodd-Frank, Financial Regulation)

**Context:**

Pre-2008 financial crisis, mortgage originators could sell loans immediately, bearing no consequences if loans defaulted. Risk retention rules create consequence alignment by requiring originators to retain exposure.

**Pattern Application:**

**Decision-makers**: Mortgage originators, securitizers

**Alignment gap**: Originators faced no consequences for poor underwriting—risk was transferred to investors

**Consequence mechanism**: Risk retention requirements—originators must retain 5% exposure

**Feedback channel**: If loans default, originator bears losses; if loans perform, originator profits

**Adjustment capacity**: Originators can improve underwriting standards to reduce default risk

**Outcomes:**

**Positive:**
- Creates direct financial consequence for loan quality
- Aligns originator and investor interests
- Empirical evidence suggests improved underwriting quality post-implementation

**Negative:**
- 5% retention may be insufficient for full alignment
- Complexity in implementation and compliance
- May reduce credit availability (potentially appropriate cost of alignment)
- Can be structured around in some cases

**Lessons Learned:**

- Financial consequence alignment can be precisely engineered
- Quantitative retention requirements create clear mechanism
- Calibration matters—too little retention doesn't change behavior
- Market participants will seek to minimize retained risk within rules

**References:**
- Acharya, Viral V., et al. (2013). "Securitization without Risk Transfer." *Journal of Financial Economics*, 107(3): 515-536.

---

## Related Patterns

### Patterns Often Used Together:

- **[Bounded Delegation](bounded_delegation.md)**: Professional bodies need consequence alignment to maintain accountability while exercising delegated authority
- **Transparent Methodology**: Consequence alignment works better when decision-makers and affected parties can observe the routing mechanism
- **Independent Oversight with Enforcement**: Oversight findings can feed into consequence mechanisms

### Alternative Patterns:

- **Democratic Override**: Different approach to accountability—preserve ability to reverse decisions rather than create consequences for decision-makers. Complements rather than replaces consequence alignment.
- **[Actionable Transparency](actionable_transparency.md)**: The information-side complement to consequence alignment — ensures the empowered party can access and act on disclosed information. Both are required for functional accountability.

### Conflicts With:

- **Risk-Pooling Mechanisms**: Insurance and social safety nets deliberately weaken individual consequence alignment to enable collective risk-sharing
- **Deliberative Insulation**: Some decisions benefit from protecting decision-makers from immediate consequences (judicial independence, long-term planning)

### See Also (DSL Terms):
- **[Degeneracy](../DSL/degeneracy.md)**: The structural property that consequence alignment is designed to reduce
- **[Causal Determinism](../DSL/causal_determinism.md)**: Strong consequence alignment requires high causal determinism — consequences must reliably follow decisions
- **[Cost Routing](../DSL/cost_routing.md)**: The mechanism by which consequences are directed back to decision-makers
- **[Structural Drift](../DSL/structural_drift.md)**: A systemic consequence of weak consequence alignment — when decision-makers don't bear the costs of the tools they build, successors inherit and expand them

---

## Evidence

### Research Studies:

1. Jensen, Michael C., and William H. Meckling (1976). "Theory of the Firm: Managerial Behavior, Agency Costs and Ownership Structure." *Journal of Financial Economics*, 3(4): 305-360.
   - Finding: When managers bear consequences of decisions (ownership stake), agency costs decrease

2. Acharya, Viral V., et al. (2013). "Securitization without Risk Transfer." *Journal of Financial Economics*, 107(3): 515-536.
   - Finding: Risk retention requirements improve loan quality by creating consequence alignment

3. Moynihan, Donald P. (2008). *The Dynamics of Performance Management*.
   - Finding: Performance-based budgeting creates consequence alignment but faces measurement and political will challenges

### Comparative Analysis:

Cross-domain evidence suggests consequence alignment improves decision quality when:
- Consequences are measurable
- Attribution is possible
- Time lag is manageable
- Mechanism is structural rather than discretionary

Alignment fails when:
- Mechanisms can be waived or overridden
- Measurement is gamed
- Attribution is unclear
- Time horizons exceed decision-maker tenure

### Limitations of Evidence:

- Most evidence is domain-specific; general principles are less well-established
- Measurement of "decision quality improvement" varies across studies
- Hard to isolate consequence alignment from other factors
- Publication bias toward successful implementations

---

## Anti-Patterns

### Anti-Pattern: Punishment Theater

**Looks Like:**
Creating visible consequences for decision-makers when bad outcomes occur

**Actually Is:**
Post-hoc punishment without structural connection to decision quality; consequence is triggered by outcome visibility, not decision quality

**Why It Fails:**
Doesn't create feedback loop—decision-makers learn to avoid visible bad outcomes, not to make better decisions. May learn to conceal rather than improve.

**How to Avoid:**
Connect consequences to decision process and decision quality, not just to outcomes. Ensure consequence mechanism can distinguish good decisions with bad luck from bad decisions.

---

### Anti-Pattern: Metric Gaming

**Looks Like:**
Decision-makers experience consequences tied to measurable outcomes

**Actually Is:**
Decision-makers optimize for measured metrics rather than underlying goals; metrics become targets and cease to be good measures

**Why It Fails:**
Consequence alignment is to wrong target. Decision-makers are aligned with metric, not mission. Goodhart's Law: "When a measure becomes a target, it ceases to be a good measure."

**How to Avoid:**
Use multiple metrics, rotate metrics, measure outcomes rather than outputs, conduct qualitative evaluation alongside quantitative, reserve judgment for unmeasured dimensions.

---

### Anti-Pattern: Excessive Consequence Sensitivity

**Looks Like:**
Strong consequence alignment where decision-makers bear full costs of decisions

**Actually Is:**
Over-correction producing excessive risk aversion; decision-makers avoid all downside risk, including beneficial risks

**Why It Fails:**
Some risk-taking is desirable. If all downside is borne by decision-maker without corresponding upside, rational response is excessive caution.

**How to Avoid:**
Calibrate consequence alignment to appropriate level; ensure upside also routes to decision-maker; distinguish avoidable failures from reasonable risks that didn't work out.

---

## Discussion and Open Questions

**Intergenerational Alignment:**
How can we create consequence alignment for decisions with intergenerational effects? Current decision-makers won't live to bear costs of climate policy, infrastructure neglect, or fiscal commitments. Proxy mechanisms (debt limits, sustainability requirements) attempt to create alignment but are imperfect. Is meaningful intergenerational consequence alignment possible?

**Collective vs. Individual:**
When decisions are made collectively (legislative votes, board decisions), how should consequences route? To the collective? To individual decision-makers? Collective consequences may create free-rider problems; individual consequences may be arbitrary when decision required majority. What's the right unit for consequence alignment?

**Measurement Limits:**
Many governance outcomes are inherently difficult to measure (quality of life, justice, democratic health). How do we create consequence alignment when outcomes resist quantification? Excessive reliance on measurable outcomes may distort priorities toward measurable domains.

**Professional Discretion:**
Some domains require professional judgment that shouldn't be constrained by immediate consequences (judicial decisions, medical choices, creative work). How do we identify where consequence alignment is appropriate vs. where insulation serves important purposes? What distinguishes legitimate professional discretion from accountability avoidance?

---

## Contributors

- Jason Edwards - Initial pattern documentation - April 2026

---

## References

1. Jensen, Michael C., and William H. Meckling (1976). "Theory of the Firm: Managerial Behavior, Agency Costs and Ownership Structure." *Journal of Financial Economics*, 3(4): 305-360.

2. Schick, Allen (2007). *The Federal Budget: Politics, Policy, Process*. Brookings Institution Press.

3. Moynihan, Donald P. (2008). *The Dynamics of Performance Management: Constructing Information and Reform*. Georgetown University Press.

4. Acharya, Viral V., et al. (2013). "Securitization without Risk Transfer." *Journal of Financial Economics*, 107(3): 515-536.

5. Studdert, David M., et al. (2006). "Claims, Errors, and Compensation Payments in Medical Malpractice Litigation." *New England Journal of Medicine*, 354(19): 2024-2033.

6. Hoel, Erik, and Abel Jansma (2025). "Engineering Emergence." *arXiv preprint*.

---

## Revision History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | April 2026 | Initial pattern documentation | Jason Edwards |

---

**Template Version**: 1.0  
**Template Last Updated**: February 2026
