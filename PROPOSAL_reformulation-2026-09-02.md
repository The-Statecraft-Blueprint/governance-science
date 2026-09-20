# Reformulating `governance-science`

*A proposal. Status: draft for Jason. Nothing here is decided except where marked ✅.*

## Version history

- **v1 — 2026-09-02.** First pass, from `statecraft-blueprint` alone. Proposed a three-layer model: notation / method / catalogue.
- **v2 — 2026-09-02.** After reading `church-bells/` and `eo-structural-weight/`. **The three-layer model was wrong — it is four, and the two layers I was missing are the two that are already built.** Jason's decisions on the v1 open questions folded in. Sequencing rewritten for tertiary priority.
- **v5 — 2026-09-02.** May (2003) read end to end; open item #3 (Westminster/layer) closed. Two decisions from Jason recorded: the building material stops being a metaphor and becomes an evidence base, and **the definitional arrow does not reverse until the revised profile has been run against all four cases and discriminates.** Both logged at `statecraft-blueprint/governance-design-agency/context/DECISION_LOG.md` #38, #39.
- **v4 — 2026-09-02.** Adds "On abstracting too early" — the function/housing test drawn from spec §IV.0, the variation-versus-count problem, the "known not to generalize" register, and a Westminster caveat on the New Zealand case that should get a gap-analysis pass. `docs/tsb-work-structure.md` updated in `statecraft-blueprint` (uncommitted) to reverse the definitions-flow-down arrow and mark it *intended, not yet executed*.
- **v3 — 2026-09-02.** Flag chronology checked against the scoring scheme's version history. **v2's framing of the ten-versus-eleven contradiction was backwards and is corrected below — this matters, because acting on v2's version would have broken a frozen instrument.** Adds the frozen/living distinction, which is the general rule underneath all three of Jason's replies. Jason's methodology-consolidation proposal adopted and its mechanics sharpened.

---

## The short version, restated

TSB contains **four separable reproducible things**, and they have been travelling under one word — "framework":

| Layer | What it is | Where it lives now | State |
|---|---|---|---|
| **1. Notation** | mandate / architecture / execution — how to *read* an instrument | spec Part I; and, in retired vocabulary, Church Bells' Abstraction Layer Analysis | Written, needs extracting |
| **2. Method** | the brief protocol — how to *analyze* one instrument | `church-bells/church-bells-brief-methodology.md` v3.0 | **Built and running** |
| **3. Measurement** | the scored instrument — how to analyze *many*, comparably and reproducibly | `eo-structural-weight/` | **Built, validated, public** |
| **4. Catalogue** | patterns, DSL, reference implementations — what the analysis *finds* | `governance-science/`; `eo-structural-weight/findings/` | Stale in one place, growing in the other |

`governance-science` holds **only layer 4**, holds it in a pre-v4.0 form, and holds nothing of 1, 2 or 3.

**That is the reformulation.** v1 said the repo has the parts list and none of the instructions. That was right but understated the problem: you have written the instructions, twice, in two other repos, and neither of them is the repo whose stated job is to hold them.

**And the thing v1 missed entirely:** you already know how to explain this to another person. You did it. `flags-canonical.md` v1.2.2 is a written rule set that an independent coder, blind to the answers, applied to 298 orders and reproduced your judgment at AUC 0.7836. That is not a hope that the method transmits. **That is a measurement of how well it transmits.** The reproducibility problem you described with Mike is solved for the flag layer and unsolved for the notation layer, and knowing which is which is most of the work.

---

## The rule underneath all of this: the record is not the documentation

*New in v3. It is the general form of all three items Jason replied on, and I think it is the most useful thing in this document.*

TSB's corpus discipline is excellent and it has **one class of document in it**. One fact one home; supersession marked, never silently replaced; render don't rewrite; same-day saves. Every one of those is a rule for a **living document** — something whose job is to be *currently true*, and which is therefore wrong when it falls behind.

But the operation now produces a second class, and it has no rules at all:

| | **Living document** | **Research record** |
|---|---|---|
| Job | Be currently true | Be *what was actually the case at time T* |
| Examples | The spec, `MANDATE.md`, Church Bells v3.0, the READMEs | `flags-canonical.md` (frozen), `scoring-scheme.md` (pre-registration), the April methodology (protocol-as-run), the blind-coding package, every brief written under a since-retired framing |
| When it falls behind | It is **stale**. Fix it. | It is **correct**. Updating it destroys it. |
| Failure mode | Divergence | **Retro-fitting** — quietly making the record agree with what you now believe |

The two classes are currently stored the same way, named the same way, and treated the same way — which is exactly why the April methodology reads as "a stale copy to clean up" when it is the protocol the experiment ran on, and why the eleven-flag set reads as "drift to reconcile" when it is the frozen instrument.

**The rule to add to the practice note:** a research record is marked frozen, dated, and *never edited* — corrections go in a separate erratum that cites it. Its location should make its status obvious without reading it. And a document that is currently living can become frozen the moment something is run against it, which is the transition that needs catching.

**This is also the field-level point, not just a housekeeping one.** Governance science's whole claim is that governance fails because nothing checks the design against the objective afterwards. A discipline making that claim cannot itself be casual about preserving what it actually did. The frozen/living distinction is the corpus-discipline expression of the same idea, and it belongs in `practice/` as a stated rule rather than as something the maintainer happens to be careful about.

---

## On abstracting too early — the governing design question for this repo

*New in v4, from Jason: the worry about reaching for an abstraction before you have enough implementations, and about separating what is U.S.-specific from what generalizes to any democracy.*

### Your own corpus is the evidence that the instinct is right

Two abstractions, same project, different outcomes, and the difference is exactly the one you named:

- **"Separating policy from structure"** was extracted from **zero** worked implementations. It was a shape that felt right. It was held for ten months, reached the published corpus, and is disqualified by a foundational finding in the room it was written for. `GAP_ANALYSIS.md` has the post-mortem.
- **Mandate / architecture / execution** was extracted **after** Utah H.B. 437 and the 1970 LRA had both been worked end to end. It has survived every room it has been in since.

So the rule is already in the record: **abstractions extracted from worked cases survived; abstractions extracted from intuition did not.** That is a stronger prior than the software heuristic because it is drawn from this project rather than borrowed.

### But the count is not the problem — the variation is

The rule-of-three heuristic is usually stated as a count, and that is the misleading version of it. Three implementations only teach you what is variable **if they vary.** Three implementations of the same shape teach you nothing; they just make you confident.

Count what you have:

| Implementation | Jurisdiction | Instrument type | Direction |
|---|---|---|---|
| Utah H.B. 437 | US state | Enacted statute | Backwards |
| 1970 LRA §§120/121 | US federal | Enacted statute | Backwards |
| The EO corpus (7,149) | US federal | Executive orders | Backwards, scored on flags rather than on the notation |
| Church Bells briefs | US federal | Bills and orders | Roughly forwards |
| NZ Building Act 1991 | New Zealand | Regulatory regime | Backwards |

**That is five implementations and essentially one variation.** Four of the five are United States; the fifth is the only evidence you have about the axis you actually want to generalize along. Adding a sixth US case would sharpen the notation and would tell you **nothing** about what is US-specific — which is the thing you said you are trying to show people.

**The practical consequence: the comparative programme is not evidence-gathering, it is variation-gathering, and that changes what it is for.** Framed as evidence, the question is *does the framework's claim hold in Switzerland?* Framed as variation, it is *which parts of my abstraction did I have to change to describe Switzerland?* The second produces a better abstraction; the first mostly produces confidence. One non-US case carried to real depth is worth more to the abstraction than ten more American ones.

### The test for "is this US-specific?" is already in your spec

Spec §IV.0 makes exactly the right cut and does not yet apply it beyond the institution:

> **"The proposal is the function. The Governance Design Agency is one way to house it."**

**That split is the abstraction rule, and it works at every layer.** For any element, ask: is this a *function* (something that must happen for the design to work) or a *housing* (a particular jurisdiction's way of making it happen)? Functions generalize; housings do not, and should not be expected to.

Run it and it sorts cleanly:

| Function — generalizes | Housing — varies by jurisdiction |
|---|---|
| The objective must be stated somewhere authoritative | Findings section (US) / preparatory works (Nordic) / Art. 296 TFEU (EU) |
| The design must be checkable against the objective | Performance-based codes; notice-and-comment records |
| The design must be correctable without reopening the settlement | **Incorporation by reference** — US federal administrative practice |
| Someone must be able to report that it is not working | Citizen intake; ombudsman; inspectorate |
| The evaluative capacity must survive its own findings | Art. III compensation protection (US); Art. 170 (CH) |

**And notice what that table exposes.** Nearly every load-bearing *mechanism* in the current framework is US administrative or constitutional practice — incorporation by reference, nondelegation and major questions, Article III protection, the legislature/agency/court triangle. That is not a flaw; it is what makes the GDA a real proposal rather than a wish. But it means **the mechanisms are the housing, and almost none of them should be expected to travel.** The five slots are the functions, and they should.

This is why the conformance profile is doing more abstraction work than it looks like it is — see below.

### The conformance profile is the abstraction, and it is better-shaped than it appears

A good interface specifies **obligations, not implementations**. The five-slot profile does exactly that: each slot states something that must be true, and says nothing about how. The Nordics satisfy slot 1 with preparatory works; the US mostly does not satisfy it; Switzerland addresses slot 5 constitutionally; New Zealand satisfied 1 and 2 and left 3–5 empty.

**That is one interface with several implementations, which is the rule-of-three satisfied structurally rather than by accumulation.** And it is the DIE/GDA move — your own model, stated in `tsb-work-structure.md` — applied one layer down: from institutions to instruments.

It also does the thing you said you want, mechanically rather than rhetorically. *"Here is what any democracy must have; here is how the United States currently answers each one; here is how four other democracies answer them differently."* A reader does not need to be argued into the US/general distinction. **The table shows it.**

### How to keep it evolvable — a mechanism, not a hope

You said you might not get it all right and want something that can evolve. The corpus already has the machinery and it is currently applied only to the instrument, not to the abstraction:

`scoring-scheme.md` went v1.0 → v1.4 without losing validity, because every change was a **dated amendment with a stated reason**, and because v1.4 explicitly recorded which parts were unchanged and still frozen. That is how an artifact evolves without rotting.

**The addition worth making: every governance-science artifact carries a "known not to generalize" register.** Not a caveat paragraph — a running list, in the same spirit as `RESEARCH_LEADS.md` §2 (dead ends), which is the best file in the corpus. Every time a non-US case forces a change, the change and the case go in it. That converts *"I might not get all of it right"* from a worry into a mechanism, and it makes the abstraction's evolution legible to a contributor instead of looking like the maintainer changing his mind.

It has a second effect worth having: **it makes the repo contributable earlier than it otherwise would be.** A stranger cannot usefully argue with a finished abstraction. They can very usefully say *"slot 3 does not describe how this works in my country, here is why"* — and that is a contribution the register knows what to do with.

### One concrete thing to check, and I would check it before leaning on the case

**New Zealand is your only non-US implementation, and it is a Westminster system.** No codified constitution, no upper house, and an executive that commands the legislature by construction. The US framing — a legislature that states objectives, an agency that designs, a court that reviews — describes a separation that does not exist in the same form there.

And the 1991 separation was, as far as I can tell from the corpus, a **regulatory** separation: performance-based codes against prescriptive codes, at the code layer. That is genuinely an instance of mandate-versus-architecture. But it is not obviously the same act as a legislature stating an outcome and a separate body designing the implementation, which is what the framework proposes.

**This cuts both ways and that is why it needs resolving rather than avoiding.** If the separation worked the same way in a system with a structurally different legislature–executive relationship, the generalization is *stronger* than currently claimed and nobody has said so. If it was a different act that shares a name, then the framework's one non-US data point is doing less work than §III.5 implies — and someone who knows New Zealand public law will say so in a room where it costs.

Either answer is worth having. Neither is in the corpus. **It is a gap-analysis pass on the framework's own best evidence**, and by `GAP_ANALYSIS.md`'s own triggers it should already have run.

---

## Finding 0 — the public repos

All cheap to fix; all get worse with time.

### 0a. Ten versus eleven flags — ⚠️ **v2 had this backwards**

**v2 implied the eleven-flag set was the drift. It is the opposite, and the correction matters, because acting on v2's version would have broken the instrument.**

The chronology, from the documents:

| Date | Document | Flags |
|---|---|---|
| March/April 2026 | `church-bells-brief-methodology.md` (the bootstrapping copy) | Nine, in prose; second/third-order effects among them |
| **June 2026** | `methodology/scoring-scheme.md` **v1.0** | *"Eleven flags, uniform weights, 0/1/2 status mapping, AUC ≥ 0.70 validation threshold. **Committed before any EO is coded.**"* |
| July 5, 2026 | `flags-canonical.md` v1.2.2 | Eleven. Adds Inter-Agency Cannibalization and Exemptions Architecture to the nine, **with a written rationale for why neither could nest under an existing flag** |
| Aug 30, 2026 | `church-bells-brief-methodology.md` **v3.0** | **Ten** — the merge of v2.0 and the April revision, demoting Second/Third-Order Effects from flag to analysis layer |

So the eleven-flag set is the **pre-registered, frozen instrument**, and the ten-flag set is the artifact — produced by an August merge that reconciled two Church Bells versions against each other and never crossed the repo boundary to see `flags-canonical.md`. That is a Cowork-era divergence, not a Claude-Web one, and it is the same failure the root `CLAUDE.md` records about the GDA spec: *the wrong copy won, because it was the one loaded first.* Here it won because the right copy was in another repository.

**Why this had to be checked rather than assumed.** `scoring-scheme.md`'s version history is the most disciplined document in the corpus. v1.3 *removed* material because reasoning about hypothesis-level implications while producing the codings that feed them risks biasing those codings — the blinding principle applied reflexively to itself. v1.4 **disqualified a completed 298-order coding pass** because the coder had been aware of class labels, retained it for qualitative use only, and specified a formal independence requirement for any pass whose AUC is reported. Nothing about that document's history is consistent with careless flag drift.

**7,149 orders are coded against eleven.** Reconciling toward ten would silently invalidate the instrument. **The reconciliation runs the other way: Church Bells v3.0 is the document to correct.**

*(Minor, noted in passing: `scoring-scheme.md` v1.4 cites `flags-canonical.md` **v1.2.1** while the file on disk is **v1.2.2**. Almost certainly a definitional clarification after the citation was written — but on a frozen instrument, worth one minute to confirm and one line to record.)*

### 0b. The April methodology — ✅ **Jason's resolution adopted, with one adjustment**

> *"Generalize the Church Bells methodology and publish it here in governance-science. Then it can just be referenced by both eo-structural-weight and TSB/Church Bells."*

Right, and it is the move that makes `governance-science` a **substrate** rather than a downstream definitional repo — see "What this changes" below.

**The one adjustment**, and it follows from the frozen/living rule: the April copy is not superseded documentation. **It is the protocol the experiment was run on** — a research record, in the same class as the pre-registration and the blind-coding package. Marking it *"superseded, see the new version"* would be actively wrong: it would invite a reader to evaluate the experiment against a protocol the experiment did not use.

So, three documents with three different jobs:

| Document | Class | Where it goes | How it is marked |
|---|---|---|---|
| **The generalized protocol** (new; from Church Bells v3.0, de-Americanized) | Living | `governance-science/method/` | Versioned; both repos cite it |
| **`flags-canonical.md` v1.2.2** | **Frozen** | `governance-science/measurement/` | Freeze travels with it; amendments dated and reasoned, per the scheme's existing practice |
| **The April methodology** | **Frozen** | Stays in `eo-structural-weight/`, ideally moved under `mayer-price-validation/` or a `provenance/` folder | *"The protocol as it stood at pre-registration. Preserved unchanged as part of the validation record. Not current guidance — see `governance-science/method/`."* |

Location doing the work is the point: under `mayer-price-validation/`, nobody mistakes it for current guidance, and no one has to read a header to know that.

**Church Bells v3.0 then becomes a rendering** of the generalized protocol — the US-federal-instrument application of it — rather than a parallel canonical document. That is *render, don't rewrite*, applied across a repo boundary for the first time. The discipline already exists; it has just never been asked to cross this line.

### 0c. `governance-science` itself (unchanged from v1)

- `essay-draft_structure-policy-separation.md` — built on the framing `GAP_ANALYSIS.md` records as a documented ten-month failure, naming Danielle Allen as the foil, in public, while the relationship is live. ✅ **Decision 5: pull it, use the category-error framing.**
- `README.md` — dated February, four dead links, undercounts its own contents, says "certified governance scientists."
- `DSL/democratic_implementation_engine.md` — defined against the two-way architecture/policy split.
- Three uncommitted drafts at root.

**Not urgent, and worth a note:** `eo-structural-weight` also has `repo-rebuild/`, `cowork-package/`, `cowork-package-2/` and `full-sync.zip` sitting in the working tree. All untracked or gitignored, and `research/proprietary/` is correctly gitignored — **the copyrighted Mayer PDFs are not exposed.** I checked; that's clean. It's just clutter.

---

## Church Bells — you asked whether it's a pattern. It's three things, and separating them is the useful move

### It is a method (→ `method/`)

`church-bells-brief-methodology.md` v3.0 is, as far as I can tell, the most complete reproducible artifact in the entire operation. It has:

- A **pipeline** — Detect → Analyze → Distribute → Mobilize.
- A **fixed section order** with a stated reason for the ordering (the Architecture Question's gap statement must hand directly to Recommendations).
- **Ten structural flags** as a checklist, with absence scored explicitly — *"the absence of a collapse is itself a data point."*
- **Four analysis layers** — incentive mapping, failure modes, second/third-order effects, accountability gaps — each with named recurring patterns (permanent emergency, precedent ratchet, lobbying gravity shift, legislative atrophy).
- A **two-axis confidence taxonomy**, required on every finding, in a literal format, because *"consistent formatting is the only thing making ratings comparable across briefs over time."*
- A **required positive-findings section** — "What This Brief Gets Right" — with a stated reason: *"a brief that contains only problems is either missing something or approaching its subject as an adversary rather than an analyst."*
- A **sourcing rule**: primary text only, never summaries. The abstraction-layer analysis cannot be done any other way.
- A **falsifiability protocol** I didn't expect to find: the **retrospective brief**. Written as it would have been published at the time, then a postscript documenting what happened. *"The vulnerabilities identified above were not predictions. They were observable in the legal architecture at the time of signing."* That is a designed test of whether the analysis is derivable from the design or is hindsight — and it is a better answer to "how do I know your method isn't just narrating outcomes" than any argument.

**Almost all of that generalizes off executive orders and bills with no loss.** It is a governance-instrument analysis protocol that happens to have been developed on US federal instruments.

**One thing must be rewritten rather than copied.** The Abstraction Layer Analysis section is the notation — *"whether the design separates policy goals cleanly from implementation specifics"* — stated in the **pre-v4.0 policy/structure vocabulary that `GAP_ANALYSIS.md` retired.** The software-architecture analogy it uses ("a statute is an API contract, rulemaking is the implementation, administration is the runtime") is mandate/architecture/execution, arrived at independently, from a different direction, before the spec's Part I existed.

**That is worth pausing on.** It means the notation has been running operationally on live instruments since April, in every brief with an abstraction-layer section. You have roughly ten worked applications of the decomposition that you may not be counting as such — which is directly relevant to the Foxworth problem, because the conversion guide can be written *from* them rather than invented.

### It is a pattern (→ `patterns/`)

Spec §III.5: *"Part of what a design feedback loop must do is manufacture the error signal that catastrophic failure supplies for free. That takes an institution."*

Church Bells is that function, performed by a civil-society actor with **no authority whatsoever**. Detection, triage, structural analysis, publication, recommendations — the GDA's §V.1–V.3 and part of §V.9, running now, at small scale, on a volunteer basis.

That makes it the working example for spec §IV.0.1 (*"the function is partly implemented in several places, and nowhere completely"*), and the pattern has real known uses beyond TSB: the NTSB is the with-authority version, and Bellingcat, ProPublica's structural investigations, and GovTrack are without-authority versions of varying completeness. Three known uses is `CONTRIBUTING.md`'s bar and it clears it.

**And here is the sharp finding, which I think is the most valuable thing in this revision:**

> **Church Bells occupies slot 4 and cannot reach slot 5.** It manufactures the error signal. It has no mechanism to convert that signal into a correction — the recommendations land nowhere by construction, because nobody is obliged to receive them.
>
> **New Zealand is the mirror image.** Separation without a verification loop: slots 1 and 2 with 3–5 absent.
>
> Two independent demonstrations, from opposite directions, that **the slots are not substitutable.** One is a national natural experiment in binding law; the other is your own project, running now, with the shortfall visible from the inside.

That pair is a stronger empirical argument for the institution than either case alone, and it is the kind of thing a field repo can state and a specification cannot — because the second case is you, and the spec should not be arguing from its author's own project.

**It also answers the obvious hostile question honestly.** *"If a guy with a Substack can do this, why do you need an agency?"* The answer is not that he can't — he demonstrably can, for a slice of federal action, at real quality. The answer is that detection without a correction path is where it stops, and that boundary is observable rather than asserted.

### It is a reference implementation (→ `reference-implementations/`)

With a track record, a stated credentialing theory (*"if TSB flagged structural problems in a bill, that bill passed, and those problems materialized — that is how credibility is earned without institutional credentials"*), and a documented cost structure. Profile it against the five slots like any other.

---

## `eo-structural-weight` — this is the layer that makes it a science, and it is already public

I did not expect to find this. Stating what it is plainly, because I think it is being undersold inside TSB's own documentation:

- An **eleven-flag instrument, pre-registered and frozen before any coding**.
- Applied to the full **Mayer & Price (2002) 298-order census**, then **re-coded from scratch by an independent coder blind to every label**.
- **AUC = 0.7836** against the field's standard significance classification — with the blind pass being what the claim rests on, and validation explicitly *earning the right to extend* rather than the reverse.
- Extended to **7,149 of 7,151 executive orders, 1936–present**, by two independent non-overlapping streams at full justification depth.
- **Per-record provenance**: every score traces to a coder, a preserved primary text, a written justification, and a stated rule version.
- An explicit **scope boundary**: *"the instrument measures architecture, not substantive fairness or policy wisdom. A precisely drafted, substantively troubling policy can score low — that's a feature of what's being measured, not a flaw."*

**Compare that to what `governance-science/CONTRIBUTING.md` currently demands of a contributor:** "at least 3 known uses," "evidence of effectiveness," "academic rigor." Those are aspirations with no instrument behind them. **The instrument exists, it is validated, it is public, and the definitional repo does not mention it.**

Three consequences:

**1. `flags-canonical.md` is in the wrong repo, and moving it is the single cleanest extraction available.**

It is one file. It already claims cross-project authority. It is already public. It is already frozen and versioned. It is currently homed in the *scoring* repo, which makes it look like an artifact of the EO project rather than a field-level object that the EO project happens to score. Move it to `governance-science/`, have both Church Bells and EO-SW cite it, and 0a resolves itself by forcing the ten-versus-eleven question into the open instead of leaving it implicit across a repo boundary.

**The caveat, and it is real:** the flag set is pre-registered *for the EO scoring work*. Moving the file must not create the impression that it can now be revised freely — the freeze is what the AUC claim depends on. The move should carry the freeze with it, explicitly, and any revision becomes a dated amendment with a stated reason, exactly as the scoring scheme's own version history already does.

**2. The flags need sorting onto the conformance profile, and the sort is informative.**

Right now the eleven flags are a bag of failure modes with no organizing principle beyond "these fire on real instruments." On the five-slot profile they sort — each flag reports a defect in a *particular* slot:

| Slot | Flags that report a defect in it |
|---|---|
| **2. Checkable design** | Power Concentration, Inter-Agency Cannibalization, Exemptions Architecture |
| **3. Checkable execution** | Vague Enforcement, Third-Party Incentive Gaps |
| **4. Report channel** | Accountability Gaps, Preemption of Oversight |
| **5. Correction path** | Sunset Provisions (absence of), Perverse Incentives / Zombie Emergency Trap |

That is a proposal, not a finding — the assignments are arguable and a couple of flags plausibly straddle. **What it buys if it holds:** the flags stop being a checklist and become a *diagnostic*, where the pattern of firing tells you which slot the instrument is missing. And the empty column is the interesting one: **almost nothing in the flag set reports on slot 1.** Which is what Part I predicts, since slot 1 is the one that is ordinarily absent by construction and therefore has no defect to detect — you cannot flag a missing objective the way you flag a bad one.

**3. The bundling collision — ✅ resolved: Church Bells' usage is outdated and will be updated by reference once the spec and the M/A/E work land.**

Noted, with one thing to protect on the way. **The existing briefs must not be retro-fitted.** Church Bells' abstraction-layer sections are currently the only place the notation has an operational track record, and they were written *before* spec Part I existed — which is what makes them evidence that the decomposition was arrived at independently, from a systems-engineering direction, rather than derived from the framework it now supports.

Rewriting them to use the new vocabulary would destroy exactly that. **Update the methodology; freeze the briefs.** A published brief is a record of an analysis performed on a date, in the same class as the coding records — and it has the same evidentiary value only if it is left alone. The frozen/living rule again.

There is also a sequencing consequence worth seeing: this plan makes the Church Bells rewrite **downstream of** the spec and the M/A/E extraction. It is the right order. But it means Church Bells sits on a known-outdated vocabulary for however long that takes, and the one thing that should not wait is a dated note in `church-bells/CLAUDE.md` saying so — otherwise the next fresh session reads v3.0 as current and propagates the old usage into a new brief.

---

## The other artifacts (largely unchanged from v1)

### The Decomposition (`decomposition/`) — the notation

Renders from spec Part I, stripped of the GDA. Utah H.B. 437 as the worked example; its one `[Unverified]` soft spot (no findings section, inferred not read) pinned first, or the telling leans on the **discrepancy** rather than the absence, which §I.1 already shows how to do. Keep §I.6's rhetorical rule verbatim: **name the distinction, do not argue for it.**

Now with a second source: the Church Bells abstraction-layer sections give it worked applications on real instruments, in the wrong vocabulary, that can be re-derived.

### The Conformance Profile (`conformance/`) — ✅ **Decision 4: this is a governance-science artifact; TSB updates to reference it**

Spec §I.2 already states it: *a stated objective; a design checkable against it; an execution checkable against the design; somebody who can report that it is not working; and a path by which the design gets corrected.*

| Slot | Question | Absent → |
|---|---|---|
| **1. Stated objective** | Is the outcome written down, somewhere authoritative, so achievement is determinable? | Nothing downstream is evaluable. *Did it work?* is unanswerable by construction. |
| **2. Checkable design** | Was the architecture shown to serve the objective, against alternatives, on a record? | The architecture is adopted *as* the law; the showing is never made. |
| **3. Checkable execution** | Can anyone determine whether the design was carried out as designed? | Design failure and execution failure are indistinguishable. |
| **4. Report channel** | Can a person who encounters the failure get it somewhere it registers? | Only burden and compliance are measurable — the two signals that arrive free. |
| **5. Correction path** | Can the design be revised without reopening the political settlement? | Every correction needs a new act, so corrections do not happen. |

Your decision inverts an arrow in `docs/tsb-work-structure.md` — the spec will cite governance-science rather than only feeding it. Worth writing that down there when the extraction happens, or the next fresh session will read the old arrow and put it back.

**The risk, restated because it is the one that would embarrass the work:** a five-box scorecard invites confident bad scoring. It needs a rubric with worked disagreements and epistemic labels per cell. **The good news is that this problem is solved** — `flags-canonical.md`'s four-status vocabulary (PRESENT / CRITICAL / ABSENT / NOT APPLICABLE, with absence a positive finding and NOT_APPLICABLE excluded from numerator *and* denominator) is a working answer to exactly this, already tested at 7,149-instrument scale. Reuse it; do not reinvent it.

### The Method (`method/`) — consolidating spec §IX.1 item 4

Now with Church Bells v3.0 as its backbone rather than as one input among several. The components and where they live:

| Component | Home |
|---|---|
| The brief protocol — sections, flags, layers, ratings, positive findings | `church-bells/church-bells-brief-methodology.md` v3.0 |
| Retrospective-brief protocol (the falsifiability test) | same |
| Differential diagnosis — full symptom set before candidate explanations | `book/chapter_02/DIAGNOSTIC_FRAME_NOTES.md` |
| Gap analysis — name the room, search for refutation, check prior art, say the disqualifying thing first | `governance-design-agency/context/GAP_ANALYSIS.md` |
| Epistemic labels | `VOCABULARY.md` §6, applied everywhere |
| Two-axis confidence taxonomy | Church Bells v3.0 |
| Unreliable instrument vs. inconclusive test | `DIAGNOSTIC_FRAME_NOTES.md` |
| Naive-answer analysis | spec §I.3 |

**Still true and still not written down anywhere:** every worked case runs the method *backwards*, on an enacted instrument. Voter Dollars is a proposal. Running it forwards is an **untested extension**, and the method document should say so rather than implying symmetry.

### The Practice note (`practice/`) — ✅ **sufficient as drafted in v1, plus two additions from v3**

1. **The frozen/living distinction** — see the section at the top. This is the substantive addition, and it is a field-level rule rather than housekeeping.
2. **Cross-repo enforcement.** The discipline holds beautifully *within* `statecraft-blueprint` and has no reach across a repo boundary. 0a and 0b are both instances, and 0a shows the specific cost: the correct copy lost because it was in another repository. Whatever the note says about "one fact, one home" should say what happens when the two homes are in different repos with different visibility — and that the public one is where the stale copies accumulate, because it is the one nobody is working in.

### The Catalogue (`patterns/`, `DSL/`, `reference-implementations/`)

Unchanged from v1, plus: **`eo-structural-weight/findings/` is a pattern library that doesn't know it is one.** Its own README says it is *"where a pattern gets named, defined, and tracked across every instance found — the kind of thing that's genuinely new knowledge."* The Zombie Emergency Trap continuation chain, quiet regression/strengthening pairs, the protective-seizure template, the no-private-right-of-action drafting convention. Those are patterns with *n* instances found by reading 7,149 primary texts, which is better evidence than any pattern currently in `governance-science/patterns/` has behind it.

Its README also says the extension streams' pattern logs are not yet synthesized. That backlog is `governance-science/patterns/` waiting to be written, and it is the one part of this proposal where the work is *harvest* rather than *authorship*.

### ✅ **Decision 2: publish `OBJECTIONS.md`**

Good — and it is consistent with everything else the project says about itself. Two mechanical notes, both about not being misread:

- **It needs a preamble explaining the tiers and statuses.** A reader who meets `○ open` with no gloss will read it as *refuted and conceded*. The register's own vocabulary makes sense to someone who knows it and is hostile-legible to someone who doesn't.
- **`IX.5` (the delegation objection) is explicitly noted as needing an answer "before it is needed in front of an audience that knows the literature."** Publishing puts it in front of that audience on day one. That is a consequence of the decision rather than an argument against it — but it moves IX.5 from "build it before the conference" to "build it before the register goes up," and that is a real reordering.

---

## Sequencing — rewritten for tertiary priority

✅ **Decision 1: this project is tertiary and publish-order doesn't matter.** That changes the recommendation substantially. v1's seven-step sequence assumed you were going to work on this. You are not, for a while. So:

**Do not attempt the rebuild.** Optimize instead for (a) stopping the things that get worse unattended, and (b) one extraction with a high value-to-hours ratio.

### Tier 0 — stop the bleeding. Hours, not days. Worth doing even though the project is tertiary, *because* it is tertiary

1. **Correct Church Bells v3.0 to eleven flags**, restoring Second/Third-Order Effects as a flag, with a version-history line saying the ten-flag merge diverged from the frozen set. **Do not touch `flags-canonical.md`.** ⚠️ This is the reverse of what v2 implied.
2. **Relabel the April methodology as a validation record** — one header block, and ideally a move under `mayer-price-validation/`. Not "superseded"; "the protocol as run."
3. **Dated note in `church-bells/CLAUDE.md`** that the bundling vocabulary is known-outdated pending the M/A/E extraction, so a fresh session doesn't propagate it into a new brief.
4. **Pull `essay-draft_structure-policy-separation.md`.**
5. **Fix the `governance-science` README** — dead links, counts, date, "certified."
6. *(One minute)* Confirm the `flags-canonical.md` v1.2.1 → v1.2.2 bump between the scoring scheme's citation and the file on disk, and record what changed.

These are cheap and they are the ones that cost real work later, in exactly the way the GDA spec's own corrected error did.

### Tier 1 — the high-leverage extraction, whenever you next have a session for this

5. **Move `flags-canonical.md` to `governance-science/`**, freeze intact, both projects cite it. One file, already written, already public, already the field-level object. This alone changes what the repo *is* more than anything else on the list.
6. **Write the conformance profile** and sort the flags onto it. Mostly assembly: §I.2 supplies the slots, `flags-canonical.md` supplies both the items and the status vocabulary.
7. **Write the Foxworth conversion guide** — now writable from the Church Bells abstraction-layer sections as worked examples rather than from scratch.

### Tier 2 — when this stops being tertiary

The decomposition render, the method consolidation, the comparative table (pin the NZ post-mortem, check the Nordic preparatory-works claim, resolve Art. 170), the DSL re-grounding, harvesting `findings/` into `patterns/`, the practice note.

---

## The Foxworth test (unchanged, one addition)

A five-page conversion guide taking someone with a policy proposal to a mandate/architecture/execution restatement.

Two things to lead with, offered as material rather than conclusions:

**Voter Dollars is an instance of the pattern §I.3 describes.** *Scan every ID. Build a taller fence. Give every voter dollars to give to candidates.* A proposed implementation arriving with its objective still unstated, held in the proposer's head as too obvious to need saying. §I.3 is explicit that this is the default and not a failing — which is what lets you say it to him without it landing as a criticism.

**The decomposition dissolves the argument you two had for months.** Per `relationships/mike-foxworth/context.md`, the thread ran on whether vouchers are *primary* or *complementary* to the coercion-loop diagnosis. In M/A/E terms: you were making a **mandate-layer** objection (the outcome vouchers pursue is not the outcome that needs pursuing); it was received as an **architecture-layer** one (vouchers are a poor way to achieve it). Different disagreements, different resolutions, and the bundled vocabulary is why neither of you could settle it.

**New with v2:** you now have a fair test of whether the guide works, and you have run this test before. The blind-coding protocol is the model — give the guide and Mike's own document to someone who has never spoken to you, and see whether their decomposition matches yours. You did exactly this for the flag set and got a number out of it. Doing it for the notation would tell you whether the notation transmits, which is the thing you actually said you don't know.

---

## Proposed repo shape

```
governance-science/
├── README.md                    # rewritten; the four layers, honestly stated
├── decomposition/               # LAYER 1 — the notation
│   ├── mandate-architecture-execution.md
│   ├── worked-example-utah-hb437.md
│   └── why-the-vocabulary-must-be-built.md
├── conformance/                 # the instrument that connects 1 to 3
│   ├── five-slot-profile.md
│   ├── scoring-rubric.md        # reuse flags-canonical's status vocabulary
│   └── flags-to-slots.md
├── method/                      # LAYER 2 — from Church Bells v3.0
│   ├── instrument-analysis-protocol.md
│   ├── retrospective-analysis.md    # the falsifiability protocol
│   ├── differential-diagnosis.md
│   ├── gap-analysis.md
│   └── epistemic-labels.md
├── measurement/                 # LAYER 3 — the field-level home
│   ├── flags-canonical.md       # MOVED from eo-structural-weight, freeze intact
│   ├── confidence-taxonomy.md
│   └── validation-standard.md   # pre-register, freeze, blind-code, report AUC
├── patterns/                    # LAYER 4 — re-read against the notation
│   └── external-error-signal-manufacture.md   # the Church Bells pattern
├── DSL/
│   ├── notation/                #   terms from the decomposition
│   └── properties/              #   degeneracy, cost routing, causal determinism…
├── reference-implementations/
│   ├── nz-building-act-1991.md          # the failure case: slots 1–2, no 3–5
│   ├── church-bells.md                  # the mirror: slot 4, no 5
│   ├── ch-const-art-170.md
│   ├── nordic-preparatory-works.md
│   └── us-eo-12866.md
├── objections/                  # published, with a tier/status preamble
├── practice/
├── foundations/                 # existing — causal emergence
└── guides/
    └── converting-a-proposal.md # the Foxworth artifact
```

---

## What this changes about the repo — worth stating explicitly

Three of your decisions across v2 and v3 point the same direction, and together they are a change of kind rather than of content:

- the conformance profile is a `governance-science` artifact, and TSB updates to reference it;
- the generalized method lives in `governance-science`, and both Church Bells and EO-SW reference it;
- `flags-canonical.md` moves to `governance-science`, and both projects cite it.

**That makes `governance-science` a substrate, not a downstream definitional repo.** Today `docs/tsb-work-structure.md` says *"Definitions flow down. `governance-science` defines the abstractions; `governance-design-agency/` builds the U.S. implementation."* After this, the method, the instrument and the conformance profile flow *up* into it, and the spec and Church Bells render *from* it.

That is coherent and I think it is right — it is what a field-level repo is for. But the arrow in `tsb-work-structure.md` would be wrong, and by your own repeatedly-documented failure mode, a fresh session would read the old arrow and put things back.

⏸️ **And it stays marked "intended, not yet executed" until the revised conformance profile has been run against all four comparative cases and demonstrably discriminates between them** (Jason, 2026-09-02; `DECISION_LOG.md` #39). Reversing early would have the spec — the document about to publish — citing an unpinned research artifact as load-bearing, out of the repo with the weakest corpus discipline into the one with the strongest. **§0a below is the proof that this happens.** And the profile itself was refuted as an existence test on the day it was written and re-drafted as an obligation test; **a re-drafted instrument that has not been run is not an instrument.**

✅ **Done 2026-09-02, uncommitted.** Both the `governance-science` repo description (§"The four repositories") and the flow bullet (§"How work flows between the pieces") now state the reversed direction, name the four layers, and are explicitly marked **"intended, not yet executed — nothing has moved as of 2026-09-02"** with a pointer here. The status marking is the load-bearing part: a document claiming a state that does not exist is the failure this whole proposal is about.

It also raises the priority of this repo above "tertiary" in one narrow respect: as long as it is a downstream catalogue, its staleness costs only credibility. Once it is a substrate, its staleness costs *work* — the same way v3.0's staleness cost work. That is an argument for doing Tier 0 now, not an argument for reprioritising the whole thing.

---

## Open decisions remaining

v1's five are resolved. v3's flag question is resolved by evidence rather than by choice. Bundling is resolved. Remaining:

1. **Whether `governance-science` is allowed to argue from Church Bells.** The slot-4-without-slot-5 finding is strong precisely because it is your own project's honest limit — but a field repo citing its maintainer's Substack project as evidence is a posture question, not just an evidence question. My read: fine and even good, *if* stated as a limitation discovered from inside rather than as a success story. Your call, and a hostile reader would go at it.
2. **Whether Church Bells v3.0 survives as a document at all**, or dissolves into the generalized protocol plus a thin US-instruments rendering. The second is cleaner and is what *render, don't rewrite* implies. The first is less work now and leaves two documents to keep in step — which is how this whole finding started.
3. ~~**The New Zealand / Westminster question.**~~ ✅ **CLOSED 2026-09-02 by May (2003) pp. 395–396**, and the answer is the awkward one. The failure was **local authorities and private certifiers unable to gauge performance**, with developers shopping between a council and a private certifier — *"a race to the bottom in building approval standards."* **A certification-layer failure.** The Act built the regulatory architecture; the Building Regulations 1992 carried the performance Code; the separation ran between **the Code and the means of compliance**, one layer below the legislature. It remains a real instance of mandate-versus-architecture. **It is not an instance of the GDA's own arrangement**, and spec §I.5's *"made this separation nationally in 1991"* is imprecise at exactly the point a New Zealand public-law scholar would press. Say the narrower thing.
4. **What the erratum convention is for frozen records.** The frozen/living rule says corrections cite the record rather than editing it. That needs a form — a sibling `ERRATA.md`, a dated appendix, something — decided once and applied everywhere, before the first correction has to be made under time pressure.

---

*Sources — `statecraft-blueprint`: `context/TSB_MISSION.md`, `context/CONCEPT_INDEX.md`, `docs/tsb-work-structure.md`, root `CLAUDE.md`, `governance-design-agency/` (`CLAUDE.md`, `GDA_SPECIFICATION_v4.0.md` Parts I / III.5 / IV.0 / IX, `context/ORIENTATION.md`, `GAP_ANALYSIS.md`, `RESEARCH_LEADS.md`, `MANDATE.md`, `EVIDENCE.md`, `conversations/2026-08-28-session-notes.md`), `book/CLAUDE.md`, `book/chapter_02/DIAGNOSTIC_FRAME_NOTES.md`, `church-bells/CLAUDE.md`, `church-bells/church-bells-brief-methodology.md` v3.0, `relationships/mike-foxworth/context.md`. `eo-structural-weight`: `README.md`, `methodology/flags-canonical.md` v1.2.2, `methodology/scoring-scheme.md` v1.4 **and its full version history (the basis for the v3 correction at 0a)**, `church-bells-brief-methodology.md` (the April copy), `findings/README.md`, `.gitignore`, `git ls-files`. `governance-science`: `README.md`, `CONTRIBUTING.md`, `DSL/`, `patterns/`, `essay-draft_structure-policy-separation.md`, `git log`.*
