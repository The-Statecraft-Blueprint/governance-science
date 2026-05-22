# Democratic Implementation Engine (DIE)

**Status**: Draft  
**Pattern Category**: Institutional Structure / Implementation Approach  
**Version**: 0.4  
**Last Updated**: May 2026

---

## Intent

Separate the question of *what policies society should pursue* (a democratic question with no objectively correct answer) from *how those policies should best be implemented* (a technical and scientific question that does have better and worse answers), and establish a professional body responsible for the latter—eliminating the bundling problem that currently makes implementation improvement require political re-litigation of the underlying goal.

---

## Motivation

### The Core Insight

> **"You tell me where you want to go. I'll tell you the best way to get there."**

Democratic processes decide where we want to go. Policy questions—what outcomes society should pursue, what values to optimize, what trade-offs to accept—are fundamentally political. They don't have objectively correct answers. They belong to democracy.

But *how we get there* is a different kind of question. Once a goal is set, the question of how best to achieve it has better and worse answers that can be evaluated using evidence, analyzed using social science and engineering, tested against real-world conditions, and improved over time. These are technical questions. They belong to expertise.

### The Two-Dimensional Design Flaw

Democracy faces a structural problem with two interlocking dimensions:

**Dimension 1: The Expertise Gap**

Implementation design requires specialized knowledge that most legislators don't possess. Currently, when legislators lack this knowledge, one of two things happens: implementation details get filled by whoever is willing and able to write them—often lobbyists, special interests, or political staff without relevant expertise—or the language is left deliberately vague, with the implicit expectation that departments, agencies, or courts will fill in the missing pieces downstream.

**Dimension 2: The Conflation of "What" and "How"**

We have bundled two fundamentally different questions into a single legislative product:
- **"What should we do?"** — democratic decision, no objectively correct answer
- **"How should we implement it?"** — technical design, has better and worse answers

Because implementation specifications are written directly into legislation, you cannot improve the *how* without re-litigating the entire *what*.

**The Cylinder Insight**: Like seeing a circle and a rectangle as separate 2D shapes versus recognizing they're cross-sections of a cylinder—these two dimensions create a single structural problem when seen together:

> **We have no professional implementation design layer.**

The current flow: Democracy decides goals → whoever fills the information gap writes the implementation → Legislature passes them as a bundled package → Cannot improve implementation without re-passing the entire law.

### The Re-Litigation Trap

The bundling problem produces what may be the most destructive feature of current governance: once an implementation is written into law—even a demonstrably flawed one—fixing it requires reopening the entire policy debate. Policy opponents use the amendment process to re-litigate the goal, not just correct the mechanism. The result: known problems persist while the correction is "re-litigated."

**The Utah Illustration**: Utah passed a law to prevent people legally prohibited from consuming alcohol from obtaining it at bars. The goal was democratically legitimate. But the specific implementation mechanism produced downstream effects—operational burdens on bars, unanticipated edge cases, compliance problems. Correcting it required a legislative amendment, reopening the political process while the flawed implementation remained in effect.

This pattern repeats constantly across governance. Goals are legitimate; implementations are poorly designed; corrections require political re-engagement equivalent to the original passage. The re-litigation trap is why things everyone agrees are broken stay broken.

---

## Demolishing the "Democratic Implementation" Myth

The most common objection to the DIE pattern is this: *Implementation details should be decided democratically. Putting them in the hands of professional designers is undemocratic technocracy.*

Traditionally, this objection has framed the choice as democratic accountability versus professional expertise—as though the alternative to legislator-written implementation is citizens losing control of their government.

This objection rests on a false premise. **Implementation details are not democratically decided now.** The choice is not between democratic implementation and professional implementation. The choice is between *opaque bureaucratic discretion* and *transparent professional design*.

### How Implementation Actually Gets Decided Today

When a legislature writes vague legislation—which is the norm, not the exception, because legislators lack implementation expertise, can't agree on details, and know things can be "fixed later"—the implementation details do not flow to democratic actors. They flow to:

- **Agency directors** (appointed, not elected; often political appointees with no expertise in the domain)
- **Career civil servants** (not elected; making interpretive decisions through regulatory guidance and rule-making)
- **Courts** (not elected; resolving legislative ambiguity through interpretation)
- **Lobbyists** (not elected; actively shaping implementation through the rulemaking comment process and informal agency relationships)

This traditional objection defends a system in which unelected bureaucrats make implementation decisions *opaquely*, without published methodology, without evidence requirements, without peer review, without systematic monitoring, and with no mechanism for citizens to challenge implementation quality.

### DIE Is More Accountable, Not Less

A properly designed DIE is more democratically accountable than the current system in every dimension that matters:

| Dimension | Current System | DIE |
|-----------|---------------|-----|
| Who decides implementation | Agency directors, career staff, courts, lobbyists | Professional governance architects |
| Are they elected? | No | No |
| Published methodology | Rarely | Required |
| Traceable reasoning | Rarely | Required |
| Evidence base | Inconsistent | Required |
| Peer review | None | Built in |
| Public challenge mechanism | Extremely limited | Formal process |
| Override by democratic authority | Difficult (APA challenge) | Explicit, accessible |
| Consistent across administrations | No—changes with political appointees | Yes—professional continuity |
| Monitoring whether it worked | Rare, ad hoc | Systematic and ongoing |

The question is not whether unelected professionals will be involved in implementation design. They already are, everywhere, unavoidably. The question is whether their involvement will be **transparent, evidence-based, systematically accountable, and subject to democratic override**—or **opaque, inconsistent, unaccountable, and practically irreversible**.

### What "Democratic" Implementation Actually Requires

Genuine democratic accountability over implementation requires:

1. **Transparent methodology**: Citizens and their representatives must be able to understand *how* implementation choices were made, not just *what* was decided
2. **Traceable reasoning**: The evidence base and logic behind implementation choices must be published and reviewable
3. **Peer review**: Implementation designs must be subject to professional scrutiny, not just political approval
4. **Override mechanisms**: Democratic authority must have a real, accessible path to reject or modify implementations
5. **Outcome monitoring**: There must be an institution responsible for tracking whether implementations achieved the stated goal

The current system provides none of these consistently. The DIE provides all of them by design.

---

## The Broken Feedback Loop

Democracies currently have no institution responsible for asking the question: *Did that legislation actually achieve its goal?*

Bills pass. Implementation happens. Outcomes occur. And then—nothing. There is no systematic mechanism for:
- Detecting when an implementation is failing to achieve the stated goal
- Distinguishing implementation failure from goal failure
- Designing corrections based on what was learned
- Feeding that learning back into future implementation design

This is governance without a feedback loop. It produces the same mistakes repeatedly across administrations, across jurisdictions, across decades. Practitioners in one state discover what practitioners in another state discovered twenty years earlier—and neither discovery makes it into the next implementation because there is no institution whose job is to hold and apply that knowledge.

The DIE fixes this by establishing the feedback loop as a core institutional function:

```
Democratic goal set
        ↓
Implementation designed (with monitoring indicators built in)
        ↓
Implementation executed by agencies
        ↓
Outcomes systematically monitored against goal
        ↓
Results analyzed: Did it work? Why or why not?
        ↓
┌───────────────────────────────────┐
│  Correction needed?               │
│                                   │
│  YES                    NO        │
│   ↓                     ↓        │
│  Design fix           Document    │
│  (administrative      what worked │
│   or legislative)     for future  │
│       ↓               designs     │
│  Implement fix                    │
│       ↓                           │
│  Monitor again                    │
└───────────────────────────────────┘
        ↓
Knowledge accumulates in pattern library
→ Informs future implementations
```

**This is how democracies become learning systems.** Without a feedback loop, governance is static—frozen in the design choices made at founding, accumulating design debt as conditions change, unable to distinguish what worked from what didn't.

With a feedback loop, implementations improve. Knowledge accumulates. Future designs benefit from past experience. Jurisdictions can learn from each other. The same mistakes are not repeated indefinitely.

---

## Applicability

### Use This Pattern When:

- **Policy and implementation are currently bundled**: Technical specifications are embedded in statutory text, making iteration politically costly
- **The re-litigation trap is active**: Known implementation failures persist because fixing them means re-opening policy debates
- **The expertise gap is being filled adversarially**: Lobbyists and special interests are writing implementation details because no professional body is
- **No feedback loop exists**: There is no institution monitoring whether legislation achieved its goals
- **Design debt has accumulated**: Governance systems have been incrementally patched rather than systematically designed

### Don't Use This Pattern When:

- **The goal itself is genuinely contested**: If the debate is about what to pursue, not how to pursue it, professional implementation design is premature
- **Implementation choices are policy choices in disguise**: Some "technical" questions are actually distributive—who bears costs, who gets benefits—and require democratic input
- **No relevant knowledge base exists**: Honest acknowledgment of uncertainty is more valuable than professional-looking false precision
- **Speed is paramount**: Some emergency legislation cannot wait for thorough design—though pre-building frameworks for foreseeable emergencies is itself good implementation architecture

### The HOW vs. WHAT Test

The critical test for everything a DIE does:

> **Does this change HOW government operates, or WHAT government does?**

- **HOW government operates** → DIE domain
- **WHAT government does** → Democratic process

This test must be applied consistently. When ambiguous, the default is democratic process.

---

## Structure

### The Three-Layer Architecture

```
POLICY LAYER (Democratic)
"Where do we want to go?"
──────────────────────────────────────────────────────
  Legislature / Democratic Process
  → Sets goals, values, priorities
  → No objectively correct answer
  → Resolved by political legitimacy
──────────────────────────────────────────────────────

DESIGN LAYER (Professional — the DIE)
"What is the best way to get there?"
──────────────────────────────────────────────────────
  Governance Architects
  → Translate goals into designed implementation mechanisms
  → Apply available knowledge: institutional economics,
    mechanism design, behavioral science, comparative
    policy analysis, systems engineering
  → Pre-passage QA: stress-test for downstream effects
  → Post-passage: adaptive implementation framework
  → Ongoing: monitor outcomes, design corrections
  → Has better and worse answers; improved through evidence
──────────────────────────────────────────────────────

EXECUTION LAYER (Administrative)
"Getting us there"
──────────────────────────────────────────────────────
  Government Departments and Agencies
  → Implement per DIE-defined procedures and frameworks
  → Report outcomes for monitoring and evaluation
──────────────────────────────────────────────────────
```

### The Four Core Functions

**Function 1: Collaborative Implementation Design (Upstream)**

Before legislation is finalized, governance architects work with policymakers to design the implementation. This is analogous to how engineers work with clients and stakeholders before a complex system is built—a civil engineer designing a bridge accounts for load requirements, soil conditions, environmental factors, and failure modes through professional expertise and dialogue with those who defined the need. The design emerges from that collaboration, not from generalist legislators guessing at technical specifications.

The policymaker brings: the goal, the political constraints, the values that must be honored.  
The governance architect brings: mechanism design expertise, comparative knowledge of what has worked elsewhere, behavioral analysis, edge case mapping, implementation cost analysis.  
The product: an implementation design—distinct from the legislation itself—that has been professionally developed to achieve the stated goal.

**Function 2: Pre-Passage QA**

Before a bill passes, the implementation design is systematically stress-tested:
- What are the foreseeable downstream effects?
- What edge cases does the mechanism handle poorly?
- Who bears the compliance costs, and are they proportionate to the policy intent?
- Does the mechanism create perverse incentives?
- Have comparable implementations been tried elsewhere? What happened?
- How will bad actors attempt to exploit the mechanism?

This is the function that would have caught the Utah liquor law problem before it took effect, and before it required re-legislative correction.

**Function 3: Adaptive Implementation (Post-Passage)**

After passage, governance architects define the procedures and frameworks through which agencies execute the law. This operational layer can be updated at the administrative level—within the latitude the law provides—without triggering the full legislative re-litigation cycle.

When a problem is discovered in implementation:

```
Problem identified
        ↓
Governance architect diagnosis
        ↓
HOW vs. WHAT test: Is fix within existing law?
        ↓
YES: Administrative update (fast track)
NO:  Return to legislature with designed amendment
     (not blank-slate re-litigation—the what/how
     distinction means the how can be corrected
     without re-litigating the what)
```

**Function 4: Monitoring and Feedback**

After implementation, governance architects maintain ongoing monitoring of whether the law is achieving its stated goal. This is not a one-time assessment—it is a continuous feedback loop that:
- Measures outcomes against the stated policy goal (not just process compliance)
- Distinguishes implementation failure from goal failure
- Generates corrections when implementations prove flawed
- Accumulates knowledge about what works across domains and jurisdictions
- Informs future implementation designs

This is the function that transforms governance from a static system into a learning system.

### Key Structural Components

1. **Policy Goal Input**  
   A clear statement of what the democratic process has decided to pursue. Separates *what* from *how*. Comes to the DIE from legitimate democratic process.

2. **Governance Architects**  
   Professionals applying available human knowledge to design effective implementations. Subject to professional accountability, peer review, methodological transparency, and demonstrated independence from partisan incentives.

3. **Governance Design Document (GDD)**  
   Transparent record of the implementation design: mechanism description, evidence base, options considered, anticipated downstream effects, known uncertainties, monitoring indicators. Enables genuine democratic oversight.

4. **QA Process**  
   Systematic pre-passage stress-testing: downstream effects, edge cases, compliance cost analysis, adversarial analysis, comparison to known implementations.

5. **Adaptive Implementation Framework**  
   Post-passage operational procedures defined by governance architects, executable by agencies, updatable at administrative level within existing legislative authority.

6. **Monitoring and Feedback System**  
   Systematic tracking of whether implemented designs achieve stated goals, feeding into ongoing improvement and future design knowledge.

7. **Democratic Oversight and Override**  
   Democratic authority retains authority to reject implementation designs, modify the DIE's scope, override its recommendations, and eliminate the institution. The DIE advises and designs—it does not legislate.

---

## Participants

### Democratic Authority (Legislature)

**Responsibilities:**
- Set the policy goal through legitimate democratic process
- Engage with governance architects upstream during implementation design—not after a bill is finished, but during its development
- Review Governance Design Documents and implementation options
- Retain authority to reject designs, override recommendations, modify DIE scope, or eliminate the institution

**Requirements:**
- Willingness to treat the HOW/WHAT distinction seriously in practice
- Commitment to upstream engagement rather than post-hoc review
- Political will to maintain DIE independence when its designs are inconvenient

### Governance Architects (DIE Staff)

**Responsibilities:**
- Translate policy goals into designed implementation mechanisms
- Apply all relevant knowledge: institutional economics, mechanism design, behavioral science, comparative policy analysis
- Conduct pre-passage QA
- Define post-passage procedures for agency implementation
- Monitor outcomes and diagnose implementation failures
- Design corrections—both administrative updates and, when necessary, pre-designed legislative amendments

**Structural Requirements:**
- Professional credentials in implementation-relevant fields
- Methodological transparency: recommendations traceable to evidence
- Independence from partisan political incentives (the specific mechanisms vary by implementation—see reference implementations)
- Subject to professional accountability and peer review

**What Governance Architects Cannot Do:**
- Make policy decisions (determine *what* government does)
- Override democratic choices through their own authority
- Execute laws (that is the executive branch's function)
- Make final legal determinations (that belongs to courts)

### Executing Agencies

**Responsibilities:**
- Implement according to procedures and frameworks defined by governance architects
- Report operational intelligence back to the DIE: what's working, what isn't, what edge cases are emerging
- Seek administrative corrections through the DIE when problems are identified

**Structural Position:**
The agency executes the designed implementation. It does not redesign implementation through interpretive discretion—that is the DIE's function, not the agency's. This is the key difference from the current system, where implementation design defaults to agency discretion.

### Oversight and Review (Courts, Independent Evaluators)

**Responsibilities:**
- Review implementation designs against stated democratic goals (did the design serve the goal it was designed to achieve?)
- Review executive deviations from professionally-designed implementations
- Provide accountability mechanisms for citizens affected by implementation choices

---

## Collaborations

### 1. Legislature ↔ Governance Architects: Collaborative Design

**Nature**: Iterative upstream partnership, not sequential handoff  
**Key Interaction**: Governance architects must be engaged before legislation is drafted, not handed a finished bill. The HOW/WHAT distinction must be actively maintained throughout. Governance architects present implementation options (not a single "answer"); the legislature chooses among professionally-designed alternatives based on the trade-offs between them.

### 2. Governance Architects → QA

**Nature**: Adversarial pre-passage stress-testing  
**Key Interaction**: QA must be genuinely adversarial, not confirmatory. Findings are public—enabling democratic scrutiny and civil society engagement during the deliberation period before passage.

### 3. Governance Architects → Agencies: Implementation Framework

**Nature**: Design to execution translation  
**Key Interaction**: Governance architects define *how* agencies implement; they don't manage agencies operationally. The design/execution distinction is maintained.

### 4. Agencies → Governance Architects: Operational Feedback

**Nature**: Intelligence from execution back to design  
**Key Interaction**: This feedback loop is the mechanism that enables adaptive implementation and institutional learning. Agencies are the eyes and ears of the DIE in the field.

### 5. Monitoring → Correction → Democratic Authority: Feedback Loop

**Nature**: Continuous outcome assessment driving improvement  
**Key Interaction**: Monitoring findings are public. When implementations are failing to achieve their stated goals, the DIE designs corrections and brings them to the appropriate authority—administrative update or legislative amendment. Democratic authority can see whether implementations are working, not just whether agencies are complying with procedures.

---

## Consequences

### Benefits (✅)

- **Breaks the re-litigation trap**: Implementation can be improved without reopening policy debates; the bundling problem is dissolved
- **Closes the expertise gap professionally**: Implementation design is no longer filled by lobbyists and special interests by default—it is a professional function with accountability
- **More democratic accountability, not less**: Transparent methodology, traceable reasoning, peer review, and systematic monitoring replace opaque agency discretion
- **Fewer implementation failures**: Systematic pre-passage QA catches problems before they affect real people
- **Faster correction**: Administrative-level updates and pre-designed amendments reduce time under flawed implementations
- **Governance becomes a learning system**: The feedback loop enables democracies to improve rather than repeat the same mistakes
- **Clearer accountability**: When goal and implementation are separated, it becomes possible to distinguish "wrong goal" from "bad implementation"—enabling more precise democratic correction

### Costs (⚠️)

- **Upstream collaboration takes time**: Thorough implementation design takes longer than drafting legislation without it
- **Knowledge base is nascent**: Governance architecture as a professional field is early-stage; methodology and credentialing infrastructure must be built
- **Scope disputes are inevitable**: The HOW/WHAT line will be contested in practice; maintenance requires ongoing attention
- **Cultural change required**: Legislators must genuinely engage upstream rather than treating the process as compliance
- **Independence mechanisms are hard to design well**: Protecting governance architects from partisan incentives while maintaining democratic accountability is a genuine design challenge

### Risks (🚨)

- **HOW/WHAT boundary drift**: Governance architects gradually expanding from implementation design into policy-making
- **QA theater**: Pre-passage review becomes a formality or a delay mechanism rather than genuine stress-testing
- **Implementation choices as covert policy choices**: "Technical" framing used to make distributive political choices without democratic input
- **Capture of the professional body**: Governance architects serving partisan or special interests rather than the stated policy goals
- **Feedback loop weaponization**: Monitoring function used to generate political ammunition rather than drive genuine improvement

---

## Implementation

### Prerequisites

- **Functional goal-setting process**: Democratic authority must be able to state what it wants to achieve before the DIE can design how to achieve it—and must be able to state it separately from the mechanism
- **Genuine upstream access**: Governance architects must be engaged before legislation is finalized, not brought in for post-hoc review
- **Independent funding mechanism**: Subject to political defunding threats, the DIE cannot provide honest assessments of governance failures
- **Administrative implementation pathway**: Legal framework for agencies to operate under DIE-defined procedures, with clear authority and limits
- **Judicial review framework**: Courts must be able to review implementation designs and executive deviations from them

### The HOW/WHAT Separation in Practice

The most important prerequisite is cultural: legislators must learn to state goals without specifying implementation. This is harder than it sounds. Legislators are accustomed to drafting both simultaneously. The shift requires:

1. Learning to write legislation that defines outcomes without prescribing mechanisms
2. Trusting that the implementation design process will serve the stated goal
3. Actively engaging with implementation options rather than rubber-stamping them
4. Maintaining the override authority that makes the trust warranted

This cultural shift is a precondition for the DIE to function as designed. Without it, the DIE becomes either a rubber stamp or a political battleground.

### Sequencing Considerations

Because the DIE pattern is novel, implementations typically should:

1. Start in a narrow domain where the HOW/WHAT distinction is relatively clear
2. Build track record demonstrating implementation quality and independence
3. Expand scope as legitimacy and methodology mature
4. Gradually extend toward more contested domains as credibility is established

Starting with domains where professional implementation design is least contested allows the institution to demonstrate value before it is tested in politically charged territory.

---

## Known Uses

### Known Use 1: Base Realignment and Closure Commission (BRAC) — United States

**Context:**
BRAC commissions (various rounds, 1988–2005) were created to recommend military base closures and realignments. Individual base closures are politically nearly impossible through normal legislative process—every member defends bases in their district regardless of strategic or fiscal merit.

**Pattern Application:**
Congress authorized the professional analysis function (DIE role) and committed to accept or reject the entire package—preventing cherry-picking. The HOW question (which bases should close and how) was delegated to professional analysis. The WHAT question (whether to close bases at all; what strategic goals to serve) remained democratic.

**Outcomes:**
- Major base closures and realignments that were impossible through normal process were completed
- Professional analysis overcame structural gridlock on a specific implementation category

**Lessons Learned:**
- Bundling-prevention (all-or-nothing) is often necessary; allowing cherry-picking defeats the purpose of professional design
- Time-limited commissions can implement the DIE principle in bounded domains
- The pattern works—professional implementation analysis can overcome political gridlock when the institutional design is right

**Limitations:**
- BRAC is temporary and issue-specific; the DIE pattern requires a permanent institution to enable learning across cycles
- No feedback loop—each commission starts fresh rather than building on accumulated knowledge

---

### Known Use 2: New Zealand Regulatory Impact Statement System

**Context:**
Before policies go to Cabinet, New Zealand departments must produce a Regulatory Impact Statement analyzing: the problem being addressed, options considered, the preferred option, implementation costs and benefits, and consultation that occurred. A partial implementation of the DIE's upstream QA function.

**Pattern Application:**
Systematic pre-passage analysis of implementation options across the government—the most direct government-wide parallel to DIE Function 2 (Pre-Passage QA).

**Outcomes:**
- More systematic analysis of implementation options before passage
- Greater transparency about what was considered and why
- Has improved analysis quality but has not eliminated implementation failures

**Lessons Learned:**
- Pre-passage implementation review is institutionally achievable at government-wide scale
- The value depends heavily on whether analysis is genuinely adversarial or compliance theater
- The RIS system doesn't include collaborative upstream design (Function 1), adaptive implementation (Function 3), or monitoring (Function 4)—partial implementations capture partial benefits

---

### Known Use 3: National Transportation Safety Board — United States

**Context:**
The NTSB investigates transportation accidents and issues safety recommendations without enforcement authority. Demonstrates that separating professional diagnosis and design from execution and enforcement is institutionally viable.

**Pattern Application:**
NTSB exercises the feedback loop function: systematic investigation of when implementations failed, analysis of why, and design of corrections. Professional credibility, not binding authority, drives adoption of recommendations.

**Outcomes:**
- Aviation safety improvements that would not have happened through normal regulatory process
- Demonstrated that professional analysis with transparent methodology can be highly influential without binding authority
- Track record of accuracy and independence has compounded over time into genuine institutional credibility

**Lessons Learned:**
- The feedback loop function (Function 4) can stand alone as a valuable institution even without the upstream design functions
- Professional credibility is a real asset that accumulates through demonstrated accuracy
- Separation of investigation/diagnosis from enforcement is essential to the NTSB's credibility—the same principle applies to DIE separation from execution

---

### Known Use 4: Venice Commission — Council of Europe

**Context:**
The Venice Commission (European Commission for Democracy through Law, established 1990) provides constitutional and governance design assistance to member states, particularly new or reforming democracies. Professional body of constitutional lawyers and governance experts.

**Pattern Application:**
Venice Commission exercises Function 1 (collaborative design) and Function 2 (QA) for constitutional and electoral governance architecture. Member states request design opinions on constitutional provisions, electoral laws, governance structures. Commission produces detailed assessments drawing on comparative constitutional law. Member states are not bound but recommendations carry significant weight.

**Outcomes:**
- Major influence on post-communist constitutional design across 60+ countries
- Assessments shape governance reforms where professional knowledge would otherwise not be available
- Established credibility through methodological rigor and comparative expertise

**Lessons Learned:**
- The professional knowledge base for governance implementation design exists and is consequential when applied—the Venice Commission proves this
- International scope (comparing across 60+ countries) provides the comparative knowledge base that makes recommendations credible
- Advisory authority with professional credibility can drive real change even without binding power

---

## Related Patterns

### Patterns Often Used Together:

- **[Bounded Delegation](bounded_delegation.md)**: The DIE is an application of the Bounded Delegation pattern—professional authority to design implementation is delegated within democratically-defined boundaries. The HOW/WHAT test defines the boundary. Understanding Bounded Delegation is prerequisite to designing a DIE.
- **[Consequence Alignment](consequence_alignment.md)**: The DIE creates consequence alignment for implementation designers—professional reputation and peer review create feedback loops that improve design quality. The monitoring function makes outcomes traceable back to specific implementation choices.
- **[Actionable Transparency](actionable_transparency.md)**: Governance Design Documents are the primary mechanism of actionable transparency in this pattern—structured information that enables genuine oversight rather than nominal document availability.

### Alternative Patterns:

- **Expert Advisory Commissions**: Bring expertise into the policy process without institutionalizing it. Lower stakes, lower resistance, but recommendations can be ignored and knowledge doesn't persist. Appropriate as a transitional step toward a full DIE.
- **Regulatory Impact Analysis (Limited)**: Pre-passage review of regulatory implementations without collaborative upstream design. Catches fewer problems; engagement is too late in the process. The NZ RIS system is the best example.

### Conflicts With:

- **Bundled Legislation (Anti-Pattern)**: The current norm of embedding implementation specifications in statutory text. Directly prevents the DIE from functioning because the HOW cannot be separated from the WHAT.
- **Pure Legislative Supremacy**: View that elected legislatures should control all decisions, including implementation specifications. Ignores that this is how the bundling problem is created and how implementation ends up with unelected agency staff by default.

---

## Evidence

### On the Implementation Failure Problem:

1. Pressman, Jeffrey L., and Aaron Wildavsky (1973). *Implementation: How Great Expectations in Washington Are Dashed in Oakland*. University of California Press.
   - Foundational study demonstrating that policy implementation is routinely more complex than designers anticipated; failures are often predictable in retrospect

2. Patashnik, Eric M. (2008). *Reforms at Risk: What Happens After Major Policy Changes Are Enacted*. Princeton University Press.
   - Major policy reforms frequently fail at implementation, not at passage; implementation design quality determines long-term success

3. Bardach, Eugene (1977). *The Implementation Game: What Happens After a Bill Becomes a Law*. MIT Press.
   - Documents the gap between legislative intent and implemented reality; argues for treating implementation as a distinct design problem

### On Agency Discretion Filling the Implementation Gap:

4. Moe, Terry M. (1990). "The Politics of Structural Choice: Toward a Theory of Public Bureaucracy." In *Organization Theory: From Chester Barnard to the Present and Beyond*. Oxford University Press.
   - Political actors deliberately write vague legislation; implementation discretion flows to agencies and bureaucrats who are not elected and not systematically accountable for implementation quality

5. Mashaw, Jerry L. (1994). "Improving the Environment for Innovation in the Administrative State." In *The Challenge of Regulatory Reform*, ed. R. Litan and W. Nordhaus. Brookings Institution.
   - Agency discretion in filling legislative gaps is the norm; the question is whether it is exercised well or poorly, not whether it occurs

### On Feedback Loops in Governance:

6. Schön, Donald A., and Martin Rein (1994). *Frame Reflection: Toward the Resolution of Intractable Policy Controversies*. Basic Books.
   - Policy failures often persist because there is no institutional mechanism for learning from them; the absence of feedback loops is a structural problem

7. Patashnik, Eric M., and Julian Zelizer (2013). "The Struggle to Remake Politics." *Perspectives on Politics*, 11(4): 1071-1087.
   - Reforms are frequently reversed because implementation is not maintained; institutional learning requires permanent institutional capacity

### On Professional Bodies Implementing Partial DIE Functions:

8. Joyce, Philip G. (2011). *The Congressional Budget Office: Honest Numbers, Power, and Policymaking*. Georgetown University Press.
   - CBO demonstrates that professional analysis with transparent methodology can be highly influential without binding authority

9. Sunstein, Cass R. (2013). *Simpler: The Future of Government*. Simon & Schuster.
   - Thoughtful implementation design (including behavioral insights) dramatically improves policy outcomes without changing goals

---

## Anti-Patterns

### Anti-Pattern: Bundled Legislation

**Looks Like:** Normal legislation where policy goals and implementation specifications are written into the same statutory text.

**Actually Is:** The mechanism that creates the re-litigation trap and fills the expertise gap with whoever is willing to write the details (often special interests).

**Why It Fails:** Implementation always needs iteration—conditions change, edge cases emerge, better approaches are discovered. When implementation is bundled with policy, each improvement requires political coalition-building equivalent to passing the original law.

**How to Avoid:** Legislation sets goals; implementation is designed in a separate professional product subject to its own process. This requires cultural change in how legislatures operate and a professional body with genuine capacity to fill the design role.

---

### Anti-Pattern: Agency Discretion as Implementation Design

**Looks Like:** Normal agency rulemaking and interpretation filling in the details of vague legislation.

**Actually Is:** Implementation design by default—unelected career staff making consequential choices about how laws work, with limited methodology, limited transparency, and limited accountability for whether the implementation achieves the stated goal.

**Why It Fails:** Agency discretion is opaque, inconsistent across administrations, not subject to peer review, and provides no systematic feedback on whether the implementation achieved the legislative goal. It is the worst of both worlds: unelected decision-making without professional accountability.

**How to Avoid:** Replace agency discretion in implementation design with professional governance architecture—same result (non-elected professionals designing implementation) but with transparency, peer review, traceable reasoning, and systematic monitoring.

---

### Anti-Pattern: Late-Stage QA

**Looks Like:** Bringing in implementation experts to review legislation after it has been drafted and is nearing a vote.

**Actually Is:** QA theater. Political commitments are locked in; substantive design changes are no longer feasible.

**Why It Fails:** When a bill is days from a floor vote, no governance architect can redesign the implementation mechanism. Review at this stage catches typos, not structural problems.

**How to Avoid:** Governance architects must be involved during the design of the implementation, not handed a finished product for review. The engagement is upstream, not downstream.

---

### Anti-Pattern: Single-Option Presentation

**Looks Like:** Governance architects presenting one implementation mechanism as "the" professionally correct solution.

**Actually Is:** Either overconfidence or covert political preference dressed as professional judgment.

**Why It Fails:** Most goals can be achieved through multiple mechanisms with different trade-offs. Presenting one option forecloses democratic choice over those trade-offs—some of which may be genuinely political questions.

**How to Avoid:** Governance Design Documents present a menu of professionally-vetted options with explicit trade-off analysis. Democratic authority chooses among the options; governance architects do not choose for them.

---

### Anti-Pattern: Monitoring Without Feedback

**Looks Like:** Systems that measure whether agencies are complying with procedures rather than whether implementations are achieving stated goals.

**Actually Is:** Process compliance measurement, not outcome accountability.

**Why It Fails:** An implementation can be fully compliant with its own specifications while completely failing to achieve the stated policy goal. Process monitoring doesn't detect this; outcome monitoring does.

**How to Avoid:** Monitoring must measure outcomes against the stated democratic goal, not just procedural compliance. This requires defining measurable outcome indicators at the design stage—before implementation begins.

---

## Discussion and Open Questions

**The HOW/WHAT Boundary in Practice**: The test is clear in theory; it is contested in practice. Implementation mechanisms often have distributive consequences—different mechanisms place costs on different parties. At what point do these distributive choices require democratic input rather than professional design? This is probably the most active ongoing dispute in any DIE implementation.

**Speed vs. Quality**: Urgent legislation sometimes cannot wait for thorough implementation design. Pre-building implementation frameworks for foreseeable policy domains before the political moment arrives may be the answer—but this requires the DIE to invest in areas that are not yet politically salient.

**Building the Knowledge Base**: Governance architecture as a distinct profession is nascent. The knowledge exists in fragmented form across public administration literature, mechanism design theory, and practitioner experience. Systematizing it—credentialing, methodology standards, peer review—is itself a governance architecture challenge. This repository is early-stage infrastructure for that knowledge base.

**Independence Mechanisms**: The specific institutional designs that protect governance architects from partisan incentives (appointment mechanisms, term structures, career track rules, funding independence) vary by implementation context. What mechanisms work in a presidential system may not work in a parliamentary one. See reference implementations for context-specific designs.

**The Recursion Question**: Who designs the DIE? The answer is the founding constitutional or statutory moment. But this means the founding must itself be done well—and the pattern applies to itself. See the [Governance Design Agency reference implementation](../reference-implementations/governance-design-agency-us.md) for one approach to this problem.

---

## Contributors

- Jason Edwards — Pattern development — 2025–2026

---

## References

1. Bardach, Eugene (1977). *The Implementation Game: What Happens After a Bill Becomes a Law*. MIT Press.

2. Joyce, Philip G. (2011). *The Congressional Budget Office: Honest Numbers, Power, and Policymaking*. Georgetown University Press.

3. Mashaw, Jerry L. (1994). "Improving the Environment for Innovation in the Administrative State." In *The Challenge of Regulatory Reform*, ed. R. Litan and W. Nordhaus. Brookings Institution.

4. Moe, Terry M. (1990). "The Politics of Structural Choice." In *Organization Theory: From Chester Barnard to the Present and Beyond*, ed. O. Williamson. Oxford University Press.

5. Patashnik, Eric M. (2008). *Reforms at Risk: What Happens After Major Policy Changes Are Enacted*. Princeton University Press.

6. Patashnik, Eric M., and Julian Zelizer (2013). "The Struggle to Remake Politics." *Perspectives on Politics*, 11(4): 1071-1087.

7. Pressman, Jeffrey L., and Aaron Wildavsky (1973). *Implementation: How Great Expectations in Washington Are Dashed in Oakland*. University of California Press.

8. Schön, Donald A., and Martin Rein (1994). *Frame Reflection: Toward the Resolution of Intractable Policy Controversies*. Basic Books.

9. Sunstein, Cass R. (2013). *Simpler: The Future of Government*. Simon & Schuster.

10. Venice Commission (2020). *Rule of Law Checklist*. Council of Europe.

---

## Revision History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 0.1 | May 2026 | Initial draft — focused on meta-governance architecture | Jason Edwards |
| 0.2 | May 2026 | Recentered on implementation science, QA, and adaptive correction | Jason Edwards |
| 0.3 | May 2026 | Added bundling problem, cylinder insight, career track, BRAC, three-tier, graduated commitment from GDA v2.0 | Jason Edwards |
| 0.4 | May 2026 | Stripped to abstract pattern; added myth-demolition section, feedback loop function; removed GDA-specific institutional detail | Jason Edwards |

---

**Template Version**: 1.0  
**Template Last Updated**: February 2026
