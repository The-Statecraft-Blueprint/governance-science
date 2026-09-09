# The Conditions of Consent: Dissent Price as a Procedural Criterion

**Status**: Draft  
**Document Type**: Theoretical Foundation  
**Version**: 1.1  
**Last Updated**: September 2026

---

## Overview

This document works out the standing of two DSL terms—**Dissent Pricing** and **Consent Degeneracy**—as instruments for evaluating governance systems, and draws the boundary around what they can and cannot establish.

The short version: the price a system charges for dissent is a measurable structural property that determines whether the system's consent signal carries information. Where it does not, no claim resting on that consent is checkable, including the system's claims about itself. This is a **procedural criterion**, not a moral one. It requires no imported values, applies across cultures without appealing to any of them, and is necessary but nowhere near sufficient for a system being any good.

That last sentence is the whole of the discipline this document exists to enforce. There is a tempting stronger claim in the vicinity, it is the one most people reach for first, and it fails. Section 3 sets it out and takes it apart, because getting this wrong reopens exactly the relativism problem the criterion was reached for in order to close.

---

## 1. The Question This Answers

The question arrives, in practice, in something like this form: *any system must be ethical—how?*

It is a real question and it stalls for a real reason. The instinct that systems cannot be ethical is half right, and the half that is right makes the other half hard to see. Systems have no intentions and no character, so the virtue vocabulary—honest, courageous, decent—does not apply to them. A system does what it does, whether or not anyone designed it to.

But systems are proper objects of moral evaluation even so. Rawls opens *A Theory of Justice* with "justice is the first virtue of social institutions," and his subject is the basic structure itself rather than the people staffing it. An unjust arrangement is unjust regardless of the personal decency of anyone administering it. So the question is not a category error; it is a design question asked in virtue vocabulary, because virtue vocabulary is usually the only vocabulary available for it.

The framework's own answer to the "but people are mostly decent" objection is older than the framework. Hume's knavery principle holds that in designing institutions "every man ought to be supposed a knave"—and Hume immediately adds that this is *false* about most people individually. It is a design assumption, not an empirical claim. Federalist 51 states the same premise in the American case: "If men were angels, no government would be necessary." The design premise and the empirical fact about people are not in tension, and the personnel frame is a departure from the founders' stated method rather than an expression of it.

But this only relocates the difficulty. Granting that systems can be evaluated, evaluated *against what*? Every candidate standard looks culturally situated. The designer's own philosophy is the obvious contaminant, and the worry that one is simply encoding it is well founded.

---

## 2. Why the Usual Escape Routes Do Not Work

**Appeal to the participants' endorsement.** The natural move is to let the people inside a system say whether it serves them. It runs into a loop: where a system controls the goods its participants depend on, and rewards or penalizes them according to what they say about it, the endorsement it collects is partly an output of the thing being evaluated. When senior members defend the seniority system, that is weak evidence that seniority is good and strong evidence that the system selects for and rewards people who defend it.

The objection has to be stated in that conditional form. Stated generally—systems shape behavior, preferences are behavior, therefore no endorsement from inside any system is independent evidence—it defeats all testimony everywhere, including the analyst's own, and an argument that proves that much has proved nothing. What the criterion below addresses is the specific, mechanically produced version: endorsement collected under a price the collector sets. It does not address, and does not claim to address, the general problem that people's preferences are formed by their circumstances. See Limit 2 in Section 7, which concedes precisely this and leaves it open.

**Appeal to the participants' true interests.** The move that usually follows—the endorsers are mistaken about what is good for them—is worse. It is condescending, unfalsifiable in practice, and frequently wrong. It also cannot be operated by anyone who does not already hold the standard being defended, which returns the problem unchanged.

**Appeal to the system's stated purpose.** This one works and is the framework's primary tool: here is what the institution says it exists to do, here is what its rules actually produce, here is the gap and the mechanism that makes it. It imports no external moral standard and works on a reader who shares none of the analyst's values. It is worth guarding as a property, because almost every competing reform argument requires the listener to already want a particular outcome.

The criterion developed below is a special case of that third move—applied to the one claim nearly every governance system makes about itself.

---

## 3. The Claim That Fails

Here is the tempting formulation, and it is worth stating in its strongest form because it is genuinely attractive:

> *The cost of dissent is an absolute measure of how ethical a system is. The first rule for creating an ethical system: low cost of dissent.*

The appeal is obvious. It appears to escape relativism entirely, it is measurable, it corresponds to something real about the First Amendment's underlying purpose, and it converts a philosophical impasse into an engineering variable.

It does not survive.

**A system can charge nothing for dissent and still be monstrous.** Free objection is compatible with an arrangement that hears every complaint, records it faithfully, and proceeds to do terrible things. This is the same structure as the caution that applies to mechanism design generally: a perfectly incentive-compatible arrangement can be efficiently monstrous, because the design question tells you how to produce behavior and never whether the resulting outcome is worth having. Low dissent price purchases legible preferences. It purchases nothing about what is done with them.

**"Absolute measure" is the phrase that draws the fire.** A measure of ethics that a monstrous system can score perfectly on is not a measure of ethics. Stated as an absolute, the claim invites exactly one response, and it is fatal. Stated as *necessary but not sufficient*, it survives—but "necessary but not sufficient" is a much weaker claim than "absolute measure," and the gap between them is where the argument is lost.

**And the upgrade reopens the door it was meant to close.** The original insight was epistemic: a high dissent price makes endorsement uninformative, which is a statement about what an observation can distinguish. Recasting it as *ethical* smuggles a normative standard back in—now one is claiming that low dissent price is a good thing rather than a readable thing, which is a value commitment requiring its own defense, in the same relativist weather the epistemic version had already escaped.

The instinct behind the claim is sound. The formulation gives away the property that made it worth having.

---

## 4. The Version That Survives

The bridge is a property this project names **evaluability**—that a designed system is a checkable object, because it can be tested against a stated objective. (The term is currently defined in the companion Governance Design Agency vocabulary rather than in this repository's DSL; promoting it here, so that this note does not depend on a document outside the public library, is an outstanding task.) Evaluability is conditional, and the condition usually is not met.

Restated through it:

> **Cheap dissent is not the good thing. It is the precondition for the system being checkable at all.**

If a system cannot distinguish consent from compliance, then no claim about that system's performance is evaluable—including every claim the system makes about itself. Its support figures do not report support. Its unity measures do not report agreement. Its assertion that the people it governs accept its arrangement is an assertion about an instrument that has been disconnected from what it purports to read.

This is a procedural criterion. It states a condition that must hold before evidence of a certain kind can be admitted, exactly as rules of evidence do, and it says nothing whatever about what the evidence will turn out to show. It needs no imported values. It applies identically in every culture because it concerns signal rather than substance: the question is not what people should want but whether the system can find out what they do want.

And it does not require a new normative commitment, because it slots under a term the framework has already defined for a different purpose.

---

## 5. The Formalization

The precise version is a likelihood ratio, and it is worth carrying because it is what makes the criterion survive a technical reading.

> Λ = P(endorse | actually supports) ÷ P(endorse | does not support)

An observed endorsement discriminates between the two underlying states to the degree that Λ departs from 1. As the price of dissent rises, both probabilities are driven toward 1 and Λ degrades toward 1 with them.

Three qualifications, each of which the loose version of this argument gets wrong:

**It is a matter of degree.** Λ equals 1 only where refusal is impossible. The working claim is that discriminating power falls as the price rises, and can fall far enough that decisions resting on the observation are not supportable—not that a threshold is crossed at which the signal becomes literally empty.

**The two channels move in opposite directions.** The same price rise that degrades Λ for endorsement concentrates it for refusal. Under a high price, assent is the uninformative channel and defection is the strong one, which is why such a body is read by its defections rather than by its majorities. This is not in tension with the above; it is the same fact seen from the other message.

**Lowering the price buys less than it appears to.** Driving the price toward zero removes an engineered distortion. It does not manufacture a credible signal, because the informativeness of a costless message then turns on preference alignment between speaker and listener rather than on cost (Crawford and Sobel, 1982). The common slogan—a costless message is cheap talk and therefore carries no information—is false as stated, and if it were true it would defeat this programme rather than support it, since at zero price both messages are costless. What actually destroys discrimination is *asymmetry* in the price across the available messages. That is the property dissent pricing names, and it is why the design target is the differential between what yes costs and what no costs.

On the relation to the parent term: the claim that **Consent Degeneracy** is a species of `degeneracy` rather than a borrowing rests on the general information-theoretic form—given an effect, how many causes could have produced it—rather than on the accountability reading in `DSL/degeneracy.md`, whose mapping runs decision → consequence-for-the-decision-maker and does not fit. The inheritance is from the formal definition. The entry itself makes this argument at length.

A second voider operates independently and must be stated alongside the first: a rich **reward for endorsement** destroys the signal just as thoroughly as a high price on dissent. Coerced praise and bought praise are uninformative for different reasons and by different mechanisms. Both must be low for an endorsement to be admissible—and at present only the first has a term and a pattern in this library.

---

## 6. Why This Is Internal Critique

The criterion has a property worth making explicit, because it is what gives it reach.

Nearly every modern governance system claims consent-based legitimacy. This is not a Western or liberal peculiarity—it is close to universal in the modern era, and it is precisely why authoritarian systems hold elections, stage referenda, publish approval figures, and invoke the will of the people. They are not obliged to make that claim. They make it because legitimacy is load-bearing.

Having made it, they have supplied the standard. The criterion asks only whether the evidence they offer for their own central claim is capable of supporting it. That requires the analyst to hold no position on what the good society looks like, and it does not depend on the analyst and the system sharing any values at all.

The honest limit, and it is larger than it first appears: a body that grounds its authority somewhere other than consent—divine mandate, inheritance, ownership, professional expertise, or an explicitly asserted claim to know better—is outside this criterion's reach. It is not being evaluated against its own claim, because it did not make this one.

Among *states* the exclusion is now narrow, which is what gives the criterion its reach in governance. But the terms this note supports are not restricted to states, and among the other bodies that price dissent the exclusion is wide rather than rare. A religious community, a family, a firm, a professional association: these price dissent heavily and most of them make no consent-legitimacy claim of the kind this argument turns on. The religious-exit case that motivates the **Dissent Pricing** entry is in the excluded class. For those bodies the terms remain useful as *measurement*—the consent signal is degenerate or it is not, and that is a fact about the signal either way—but the internal-critique move in this section is unavailable, and evaluating them requires standards from somewhere else. This is a real boundary and should not be papered over by counting states only.

---

## 7. The Honest Floor

Four limits, all of which should be stated whenever the criterion is used, because each is the objection a competent critic will raise:

**1. Necessary, not sufficient.** Low dissent price makes a system's consent claims checkable. It does not make the system good, and a system can satisfy this criterion completely and fail every other test that matters.

**2. Admissible, not true.** Where dissent is cheap, endorsement becomes admissible evidence—not correct evidence. Preferences can be shaped upstream, before anyone had to speak. Adaptive preference formation and system justification are well documented, including the finding that members of disadvantaged groups sometimes defend an arrangement more than the advantaged do. This criterion governs whether the evidence counts. It does not establish what the evidence proves.

**3. Silent on outcomes.** The criterion evaluates a system's capacity to read itself. It says nothing about whether what the system does is worth doing. Those are separable questions and both are required.

**4. A floor, not a ranking—and not yet an operational one.** It rules systems out; it does not order the ones that remain. Two systems that both price dissent near zero are not thereby comparable on this measure, and the interesting evaluative work in most real cases begins above this floor rather than at it.

The stronger caveat: applying a floor requires a scalar and a threshold, and dissent price is a distribution across participants rather than a scalar (see **Dissent Pricing**). No summary of that distribution has been justified here—mean, median, or the price faced by the most dependent participant would give different answers, and the choice among them is itself a value judgment. Until that is settled, the criterion identifies a direction and supports case-by-case argument; it does not yet rule any system out by computation. Anyone using it as though it did is claiming more than the apparatus delivers.

Underneath all four sits a further honesty: somewhere at the bottom there is a normative commitment that cannot be derived from facts, and anyone claiming otherwise is smuggling one in. Here that commitment is thin—roughly, that a system's own account of why it is entitled to govern should be checkable. It is far thinner than the relativism worry suggests, and nearly every argument in institutional design happens well above it.

---

## 8. A Related Correction: Selection, Not Difficulty

A neighboring reformulation is worth recording here, with a warning attached, because it is usually reached at the same moment and it is *not* a version of the criterion above.

Faced with the awkwardness of "ethical system," the natural repair is *a system that makes it easy for humans to be ethical*. Better, but *easy* is not the operative variable. Conduct of any given kind can be entirely easy and still fail to persist—if the person who engages in it is primaried, eased out, or passed over, difficulty was never the constraint.

The correction is descriptive and holds regardless of anyone's values: **systems are not difficulty dials, they are selection machines.** Whoever the system rewards is who accumulates in it. This is why replacing every member of a body changes little—the material passing through the filter is swapped and the filter is untouched—and it is the observation the whole structural programme rests on.

**Survivability** is the design question that follows: does a participant who does X remain in the system and advance within it? Note carefully what this is. It is a *schema* with a blank in it, and the blank has to be filled from outside. "Does someone who acts in the public interest survive here?" is a perfectly good question and it is not a procedural one—"the public interest" is exactly the contested, imported standard that Sections 1 through 4 established the consent criterion does not require. Anyone who fills the blank has taken on the burden of defending what they put there.

So survivability is not a sharper version of the criterion in Section 4. It is a different instrument with a different cost: more powerful, because it evaluates what a system produces rather than only whether the system is readable, and correspondingly not available to an analyst who wants to hold no position. Both are worth having. Conflating them, or presenting survivability as the procedural criterion's stronger form, throws away the property that made the procedural version worth reaching for.

Dissent pricing is a special case of the *selection* observation, which is the descriptive half: a sustained price on dissent does not primarily change what participants do, it changes which participants remain. It is not a special case of survivability-with-the-blank-filled, and nothing in Sections 3 through 7 depends on filling it.

---

## 9. Precedents

The criterion is not invented here. It exists, fully formed, inside half a dozen domains, and in every one of them it is locked to that domain:

- **Contract law** voids consent obtained under duress. An agreement signed under threat is not a weaker agreement; it is not evidence of agreement at all.
- **Research ethics** requires voluntariness. The Nuremberg Code's first principle demands that the subject "be able to exercise free power of choice, without the intervention of any element of force, fraud, deceit, duress, over-reaching, or other ulterior form of constraint or coercion."
- **International election observation** asks whether opposition parties could campaign and voters could choose without intimidation—that is, it treats the price of dissent as the precondition for reading the result, rather than reading the result on its face.
- **Labor law** protects concerted activity, on the reasoning that a workforce that cannot object without penalty cannot bargain.
- **Signaling theory** supplies the general form: a costless message is cheap talk and carries no information about the sender's type.
- **Kuran's preference falsification** supplies the empirical mechanism and the characteristic signature—falsified endorsement produces arrangements that appear stable until they collapse very fast, because no one, the regime included, can observe how thin the support has become.

Every one of these is the same criterion. None of them generalizes it into an instrument that can be pointed at an institution. That generalization—from a rule of admissibility in a particular domain to a structural property an architect sets—is the contribution the DSL terms are attempting.

---

## 10. Relation to the DSL

| Concept | Role |
|---------|------|
| **Dissent Pricing** | The independent variable. A structural property: what the architecture charges for withholding assent, through which instrument, held by whom. |
| **Consent Degeneracy** | The dependent variable. The failure state: assent and compliance become observationally identical and the consent signal carries no information. |
| **Degeneracy** | The parent. Consent degeneracy instantiates its formal definition rather than resembling it. |
| **Cost Routing** | The complement to dissent pricing. Where the consequences of a decision land, as against what is charged for refusing one. |
| **Observer Dependency** | A system sustained by falsified endorsement is maximally observer-dependent while appearing maximally stable—including to itself. |
| **Protected Dissent Channel** | The design pattern that lowers the price deliberately, and its four anti-patterns. |

---

## 11. A Note on Usage

Two cautions for anyone applying this in public-facing work.

**Avoid the word "ethical."** It is personnel-frame-coded: the moment it appears, readers slide into character talk, which is the ditch the structural argument exists to steer them out of. "Evaluable," "checkable," "survivable," or Madison's own framing does the same work without opening that door.

**Never state the criterion without its limit.** "The cost of dissent is a measure of a system" invites the objection in Section 3 and deserves it. "The cost of dissent determines whether a system's claims about itself can be checked—necessary, not sufficient" is barely longer and cannot be taken apart the same way.

---

## Open Questions

- **The endogeneity boundary.** Distinguishing mechanism-imposed cost from cost that emerges from genuine consensus is stated here as a discipline (name the instrument, name the holder) rather than as a test. Is there a sharper criterion?
- **Aggregating an unequal price.** Dissent price is a property of the relationship between a participant and a system, so it is a distribution rather than a number. What summary of that distribution is the right one for evaluating a system as a whole—the mean, the price faced by the most dependent, or something else?
- **Systems that make no consent claim.** Section 6 sets these outside the criterion's reach. Is there an analogous internal critique for a system grounding authority elsewhere, or does that case genuinely require external standards?
- **Upstream preference formation.** Limit 2 concedes that cheap dissent establishes admissibility only. How much can be said about the upstream question without collapsing into the false-consciousness move rejected in Section 2?

---

## Contributors

- Jason Edwards - Initial development - September 2026

---

## References

1. Rawls, John (1971). *A Theory of Justice*. Harvard University Press.

2. Hume, David (1742). "Of the Independency of Parliament," in *Essays, Moral, Political, and Literary*.

3. Madison, James (1788). *Federalist* No. 51.

4. Kuran, Timur (1995). *Private Truths, Public Lies: The Social Consequences of Preference Falsification*. Harvard University Press.

5. Kuran, Timur (1991). "Now Out of Never: The Element of Surprise in the East European Revolution of 1989." *World Politics*, 44(1): 7-48.

6. Hirschman, Albert O. (1970). *Exit, Voice, and Loyalty*. Harvard University Press.

7. Hoel, Erik (2017). "When the Map Is Better Than the Territory." *Entropy*, 19(5): 188.

8. Crawford, Vincent P., and Joel Sobel (1982). "Strategic Information Transmission." *Econometrica*, 50(6): 1431-1451.

9. "The Nuremberg Code" (1947), Principle 1, from the judgment in *United States v. Karl Brandt et al.* United States Holocaust Memorial Museum, Holocaust Encyclopedia.

10. Elster, Jon (1983). *Sour Grapes: Studies in the Subversion of Rationality*. Cambridge University Press.

11. Jost, John T., and Mahzarin R. Banaji (1994). "The Role of Stereotyping in System-Justification and the Production of False Consciousness." *British Journal of Social Psychology*, 33(1): 1-27.

12. Hurwicz, Leonid (2008). "But Who Will Guard the Guardians?" *American Economic Review*, 98(3): 577-585.

---

## Revision History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | September 2026 | Initial development | Jason Edwards |
| 1.1 | September 2026 | Rewrote §8: survivability is a schema requiring an imported standard, not a sharper form of the procedural criterion — the first draft smuggled "the public interest" back in, which is the exact failure this note exists to prevent. Restated §5's likelihood ratio as a ratio and as a matter of degree, and corrected the cheap-talk claim. Narrowed §2's endogeneity argument, which as written defeated all testimony. Widened §6's excluded class, which is not rare and contains the terms' own motivating case. Marked the §7 floor as not yet operational | Jason Edwards |

---

**Document Version**: 1.0
