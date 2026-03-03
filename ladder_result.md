# Domain Reach Test: Results

## LEVEL 1: PRIMITIVE STATES

### 1.1 ATTENTION

**Variable mapping:**
- X = full sensory field (all available signals)
- C = total available sensory bandwidth I(X; T_B(Y))
- A = information lost when selection function f filters/gates channels
- f = attentional gating function (gain modulation, selective filtering)

Attention lives on *both* sides of the equation. Choosing where to point the channel modulates C (bandwidth allocation). Expectation-driven filtering modulates A (post-channel distortion). The framework naturally separates "what you're exposed to" from "how you warp what you receive."

**Theorems:** Theorem 1 (R ≤ C: you can't recognize more than you contact). Theorem 4 (convergence rate: sustained bandwidth required for R to accumulate).

**Predictions (falsifiable):** Attention driven by signal-tracking (orienting to novelty) yields low A. Attention driven by expectation/desire introduces measurable A > 0. This maps onto existing findings: inattentional blindness is a C-limitation; confirmation bias in visual search is an A-contribution. These are distinguishable experimentally.

**Verdict: FORMALIZABLE.**

---

### 1.2 SENSATION

**Variable mapping:**
- X = physical stimulus (temperature, pressure, photon flux, sound pressure)
- C = I(X; T_B(Y)) where T_B is sensory transduction (receptor to neural signal)
- A = post-transduction distortion (adaptation-driven shifts, expectation overlays)
- f = perceptual processing pipeline

**Theorems:** Theorem 1 (R ≤ H(X) and R ≤ C). Theorem 3 (thermodynamic cost — sensory transduction literally has metabolic cost, and Landauer applies to neural erasure).

**Predictions:** Weber-Fechner law recasts as logarithmic channel capacity. Sensory adaptation is C(t) decreasing for constant X. Signal detection theory is already an instantiation of this structure. The framework adds: post-channel distortion A is measurable as the gap between SDT-optimal performance and actual performance.

**Verdict: FORMALIZABLE.** This is the framework's most natural home. Information-theoretic neuroscience already does much of this.

---

### 1.3 AVERSION

**Variable mapping:**
- X = aversive stimulus (actual threat/harm level)
- C = maintained contact with the stimulus
- A = distortion from withdrawal bias (over-generalization, avoidance preventing calibration)
- f = processing function incorporating the withdrawal response

**Theorems:** Theorem 2 — aversion can push a system into Class (iii) for the avoided domain (R → 0 by eliminating C). Boundary criterion: dC/dB < 0 means the system is actively resisting contact.

**Predictions:** Phobias are domain-specific Class (iii) systems (R ≈ 0 about the feared stimulus because C ≈ 0). Graded exposure therapy works by incrementally restoring C, and R should increase if A doesn't compensate. Avoidant systems will have measurably lower R in the avoided domain — testable via calibration tasks.

The *valence* of aversion — what withdrawal feels like — hits the declared consciousness boundary. The framework captures informational dynamics, not phenomenal character, and says so explicitly.

**Verdict: FORMALIZABLE** (as functional/informational state).

---

### 1.4 ATTRACTION

**Variable mapping:**
- X = attractive stimulus
- C = increased bandwidth allocation toward X
- A = desire-driven distortion (idealizing, projecting, seeing what you want)
- f = processing function incorporating approach bias

**Predictions:** Pure curiosity (signal-driven approach) yields high C, low A, high R. Craving (agenda-driven approach) yields high C but A > 0 from desire-driven distortion. This distinguishes exploration from addiction at the information-processing level — same high C, different A. Testable: curiosity-driven and craving-driven approach should produce different recognition accuracy about the approached stimulus.

**Verdict: FORMALIZABLE.**

---

**LEVEL 1 SUMMARY:** All four primitive states formalize. The foundation holds. The framework's declared consciousness boundary handles the phenomenal aspects honestly — not by explaining them, but by explicitly marking them as out of scope. No inherited failures pass upward.

---

## LEVEL 2: SUSTAINED STATES

### 2.1 FOCUS

**Variable mapping:**
- X = target signal stream
- C = maintained I(X; T_B(Y)) over time, against competing channels
- A = distortion from fatigue, intrusive signals, mind-wandering
- f = sustained filtering function

**Theorems:** Theorem 4 (convergence rate requires sustained bandwidth allocation). Theorem 1 (accumulated R ≤ accumulated C).

**Predictions:** Focus quality degrades over time as C decreases and A increases (attentional fatigue). Context-switching costs are measurable C-reallocation losses. Flow states = conditions where A is minimized and C is sustained without effort (f is well-matched to X, echoing the beauty mapping later).

**Verdict: FORMALIZABLE.**

---

### 2.2 PERSISTENCE

**Variable mapping:**
- X = goal-state and obstacles between current state and goal
- C = maintained contact with reality of the situation (including obstacles)
- A = distortion from frustration, discouragement, rationalization for quitting
- f = processing function that integrates goal-representation with obstacle-recognition

**Theorems:** Theorem 2 — persistence prevents falling into Class (iii) for the goal domain.

**Predictions:** Systems that maintain C about obstacles (clear-eyed about difficulty) persist more effectively than those with high A (denying difficulty or catastrophizing it).

**What resists:** The framework captures the *recognition* component of persistence — maintaining accurate contact with reality while pursuing a goal. But persistence is fundamentally about **action continued over time**, and R = C − A has no action term. You can perfectly recognize the goal and every obstacle and still not act. The gap between recognition and behavior is real and unfilled.

**Verdict: PARTIALLY FORMALIZABLE.** The recognition dimension maps. The behavioral/motivational dimension has no home in the equation.

---

### 2.3 DETERMINATION

**Variable mapping:** Same as persistence, with the addition that energy investment scales with resistance.

**Theorems:** Theorem 3 (thermodynamic cost) provides a partial bridge — maintaining low A under pressure costs energy. But Theorem 3 is about the cost of *erasing* A, not the cost of *sustaining action*.

**What resists:** Same as persistence, compounded. The framework has no account of why a system would *increase* energy expenditure. Energy allocation is a decision/action problem, not a recognition problem.

**Verdict: PARTIALLY FORMALIZABLE.** Inherits the action gap from 2.2.

---

### 2.4 PATIENCE

**Variable mapping:**
- X = the situation as it is, including its temporal unfolding
- C = ongoing, sustained contact with what is actually happening
- A = the urge to project, to act prematurely, to distort timing
- f = processing function held steady against time pressure

Patience = R ≈ C maintained over time, with A held low despite pressure.

**Predictions:** Impatience is measurable as A increasing over time — the gap between perceived and actual situation grows as desire for resolution distorts perception. Patient observers should show better calibration about timing, state of affairs, and unfolding events.

**Verdict: FORMALIZABLE.** This is among the cleanest mappings in the entire test. Patience is *precisely* sustained low-A recognition.

---

**LEVEL 2 SUMMARY:** Two clean formalizations (focus, patience), two partial (persistence, determination). The fault line is clear: the framework formalizes *sustained recognition* beautifully but has no action term. States that are fundamentally about **behavior over time** have a component that escapes. This is the first systematic gap: the **action gap**.

This gap does not cascade upward in a way that blocks higher levels — higher levels can still be evaluated on their recognition component. But it is a real and persistent limitation.

---

## LEVEL 3: EVALUATIVE STATES

### 3.1 PREFERENCE

**Variable mapping:**
- X = set of possible contacts {X₁, X₂, ...}
- C = bandwidth allocation across options: B(X₁) > B(X₂) encodes preference
- A = distortion from preference itself (overvaluing the preferred, undervaluing alternatives)
- f = weighting function across signal streams

**Predictions:** Preference that tracks signal quality (allocating C to high-information sources) yields high R. Preference driven by habit or desire misallocates C and introduces A. Sunk cost effects are A: prior investment distorts current signal processing.

**Verdict: FORMALIZABLE.**

---

### 3.2 JUDGMENT

**Variable mapping:**
- X = true category/state of affairs
- Y = observed signal
- f = classification function
- R = I(X; f(Y))

This is literally the core operation the framework describes. Judgment IS recognition applied.

**Predictions:** Judgment accuracy = R. Bias = A. Training (expanding f) increases R when D* is high. Prejudice = stable A in the classification function for specific input domains.

**Verdict: FORMALIZABLE.** This is the framework's home terrain.

---

### 3.3 DOUBT

**Variable mapping:**
- X_meta = the system's true recognition accuracy
- C_meta = self-observation of one's own R
- A_meta = distortion in self-observation (guaranteed > 0 by Axiom 2)
- f_meta = meta-cognitive processing function

**Theorems:** Axiom 2 (self-observation floor: A* > 0). Theorem 5 (cascade: R_meta ≤ R — you can't know your recognition better than you recognize).

**Predictions:** Doubt is well-calibrated when A is small (the system can detect its own distortion accurately). Doubt is poorly calibrated when A is large (A distorts the estimate of A). This is the Dunning-Kruger effect derived from first principles: high-A systems underestimate their own A because A* corrupts self-observation. Low-A systems slightly overestimate their A (appropriate humility). Both directions are predicted by Axiom 2.

**Verdict: FORMALIZABLE.** The self-referential structure is handled explicitly by Axiom 2 and Theorem 5. This is a genuinely novel prediction.

---

### 3.4 CERTAINTY

**Variable mapping:**
- The system estimates A ≈ 0
- By Axiom 2, this estimate is always slightly wrong (A* > 0)

**Predictions:** Certainty is never fully justified for self-modeling systems. False certainty = A masked from self-observation (the system can't see its own distortion). Appropriate certainty = A genuinely low with acknowledged irreducible floor. Overconfidence is measurable as the gap between estimated A and actual A.

**Verdict: FORMALIZABLE.**

---

**LEVEL 3 SUMMARY:** All four evaluative states formalize cleanly. This is the framework's strongest level — evaluative states are precisely about applying and monitoring recognition, which is exactly what R = C − A describes. The Dunning-Kruger derivation from Axiom 2 and Theorem 5 is a highlight: a non-trivial empirical prediction generated from the formal structure.

---

## LEVEL 4: SOCIAL STATES

### 4.1 TRUST

**Variable mapping:**
- Agent 1 uses Agent 2's recognition as input to their own channel
- X = shared reality
- C₁ includes Agent 2's R₂ as a source channel
- A₁ = Agent 1's distortion in processing Agent 2's output
- Trust = the operating assumption that Agent 2's A₂ is low

**Theorems:** Theorem 5 (cascade): R₁ ≤ R₂ when Agent 1 relies on Agent 2's recognition. You can't gain accuracy through a less-accurate intermediary.

**Predictions:** Trust is justified when the trusted party's A is genuinely low. Misplaced trust degrades R₁ by incorporating Agent 2's A₂ into Agent 1's channel. Trust networks form recognition cascades subject to Theorem 5's monotonic degradation. Institutions that reduce individual A (peer review, adversarial testing) serve as cascade-quality amplifiers.

**Verdict: FORMALIZABLE.**

---

### 4.2 RECIPROCITY

**Variable mapping:**
- Two agents mutually calibrate f₁ and f₂ to reduce A in the bidirectional social channel
- Each agent adjusts processing to reduce distortion about the other

**Theorems:** Theorem 5 cascade becomes bidirectional, forming a potential fixed point where R₁ about Agent 2 and R₂ about Agent 1 stabilize. Theorem 4 (convergence rate) governs how quickly mutual calibration occurs.

**Predictions:** Reciprocity converges when both agents have low A. It fails to converge when one agent's A distorts the feedback loop. Mutual recognition has a convergence rate bounded by the higher-A agent (the weaker link governs cascade quality).

**Verdict: FORMALIZABLE.**

---

### 4.3 LOYALTY

**Variable mapping:**
- Sustained high bandwidth to another agent's channel despite signals that would normally reduce C
- C maintained toward Agent 2 despite negative evidence about Agent 2's R₂

The framework makes a critical distinction:
- (a) **Robust loyalty:** maintaining C through noisy periods, keeping A low, letting R self-correct. The system absorbs temporary evidence fluctuations without closing the channel.
- (b) **Blind loyalty:** refusing to update on negative evidence, which requires increasing A (suppressing the evidence). This is active A-injection.

**Predictions:** Robust loyalty (a) produces higher long-term R than reactive channel-closing. Blind loyalty (b) locks the system into Theorem 2's Class (ii) — partial recognition with stable, positive A. The two are distinguishable by whether R improves or degrades over time.

**Verdict: FORMALIZABLE.** The framework's ability to formally distinguish healthy from pathological loyalty is a genuine strength.

---

### 4.4 BETRAYAL

**Variable mapping:**
- Agent 2 presented A₂ as R₂. Agent 1 used this as a channel input.
- Discovery = Agent 1's model of Agent 2 undergoes sudden A-reassessment.
- All past R₁ derived from Agent 2's channel must be retroactively discounted.

**Theorems:** Corollary 5.1 (Transparent Agenda Paradox) applies directly: Agent 2's declared intent was actually agenda, and Agent 1 used it as side information. The corollary predicts exactly this failure mode.

**Predictions:** The impact of betrayal scales with the proportion of R₁ that was built on the compromised channel. Betrayal in high-trust relationships is more damaging (more R₁ to re-evaluate) than in low-trust ones. Recovery requires re-establishing an independent channel to reality for all domains that were mediated through the betrayer.

**Verdict: FORMALIZABLE.** The informational dynamics capture the structural features of betrayal with surprising precision.

---

**LEVEL 4 SUMMARY:** All four social states formalize. The framework handles multi-agent recognition cascades well because Theorem 5 was built for chains. The loyalty distinction (robust vs. blind) and the betrayal analysis are particularly strong — they generate non-obvious predictions from the formal structure.

---

## LEVEL 5: COMPLEX STATES

### 5.1 LOVE

**Variable mapping:**
- X = another being as they actually are
- C = high, sustained bandwidth — deep and prolonged contact
- A = minimal distortion — not projecting, not controlling, not idealizing
- f = processing tuned to the particular other

Love ≈ R ≈ C, sustained over time, with A actively minimized.

**Predictions:** Love degrades when A increases (projection, possessiveness, need distorting perception). Love deepens as A decreases (truly seeing the other). Idealization = high A masquerading as high R — the system mistakes its projection for recognition. "Unconditional love" = the commitment to maintain C regardless of what X reveals, while keeping A low.

**What resists:** Love is not only high R. You can recognize someone with perfect accuracy and feel nothing. Love involves **care, commitment, and action directed toward the other's well-being** — none of which live in R = C − A. The framework captures the *epistemic dimension* of love (seeing someone as they are) but not the *agential dimension* (acting for their good). This is the action gap from Level 2, returning at higher stakes.

**Verdict: PARTIALLY FORMALIZABLE.** The recognition dimension maps beautifully and generates genuine insight (idealization as A, "seeing" as the epistemic core of love). But the caring/commitment dimension has no term in the equation.

---

### 5.2 GRIEF

**Variable mapping:**
- X = the lost being/object (now absent)
- C = channel remains "open" — bandwidth still allocated — but source is gone (Y = ∅)
- A = distortion from the gap: denial, hallucination of presence, bargaining, angry rewriting of history
- f = processing function still configured for input that will never arrive

Grief is an allocated channel to an absent source.

**Predictions:** Grief resolves as C decreases — the channel gradually closes, bandwidth reallocates to present reality. Unresolved grief = channel perpetually open, A accumulating to fill the silence. "Processing" grief = gradually reducing C while integrating the new information (the reality of absence). Complicated grief = A-injection that prevents channel closure (anger, guilt, rumination keeping the channel active).

The prediction about A filling the void of an open, sourceless channel is particularly strong: it explains why grief often involves distorted memories, idealization, or rage — these are A-products generated when C exists without signal.

**Verdict: FORMALIZABLE.** The "open channel to an absent source" formulation captures the essential structure. One of the framework's most powerful mappings.

---

### 5.3 COURAGE

**Variable mapping:**
- X = threatening reality
- C = maintained or expanded contact with the threat (not looking away)
- A = fear-driven distortion (denial, minimization, catastrophizing)
- f = processing function held stable under threat-pressure

Boundary criterion applies: dR/dC > 0 (C-expanding despite cost) = courageous. dA/dB > 0 (fear distorting incoming signal) = the system resisting its own contact.

**Predictions:** Courage produces better R about threats than avoidance. Paradox of cowardice: reducing C about threats leaves the system with lower R, making it more vulnerable to the very thing it fears. Courage under accurate R leads to better outcomes than courage under high A (bravado).

**What resists:** Courage involves *acting* under threat, not just maintaining contact. A firefighter entering a burning building isn't just recognizing the fire accurately — they're taking action despite accurate recognition of danger. The action gap, again.

**Verdict: PARTIALLY FORMALIZABLE.** Contact-maintenance under threat formalizes well. The behavioral component does not.

---

### 5.4 FORGIVENESS

**Variable mapping:**
- X = the person who caused harm, as they are now
- C = current contact
- A_accumulated = agenda built from past harm (resentment, grudge, expectation of recurrence)
- Forgiveness = the operation A → A − A_accumulated

This is a **direct operation on A**. Forgiveness IS the reduction of accumulated post-channel distortion.

**Predictions:**
1. Forgiveness increases R (freed from past-harm-driven distortion, you see the other more accurately now).
2. Unforgiveness = permanent A increment that degrades all future R about the person.
3. Forgiveness doesn't require reconciliation — you can reduce A without restoring C. A-reduction is independent of C-allocation.
4. Forgiveness doesn't require forgetting — C about the past harm can remain; what changes is that f no longer distorts current processing based on it.
5. "Premature forgiveness" = claiming A-reduction without actually performing it, which fails to improve R. Testable by whether recognition accuracy about the person actually changes.

**Verdict: FORMALIZABLE.** This is arguably the single cleanest mapping in the entire test. Every common intuition about forgiveness (that it frees the forgiver, that it's different from reconciliation, that it's different from forgetting, that it can be performed prematurely) drops out of the formal structure.

---

### 5.5 AWE

**Variable mapping:**
- X = stimulus with structure exceeding the observer's processing capacity
- C = high contact (the signal is overwhelming, B is flooded)
- f = processing function insufficient for the available input
- R < C not primarily because of agenda, but because of capacity limitation

**Theorems:** Theorem 1 (R ≤ C, and here the gap is large). Theorem 6 (meta-recursive generativity — awe may be the experiential correlate of encountering a generative structure).

**What resists:** The technical definition A = I(X; T_B(Y)) − I(X; f(T_B(Y))) captures awe's information loss. But A is labeled "agenda" throughout the framework, connoting motivated distortion. In awe, the loss isn't motivated — it's pure capacity limitation. The equation is formally correct but the semantics strain.

This reveals a genuine ambiguity in the framework: **A conflates two distinct phenomena — motivated distortion (bias, defense, desire) and unmotivated capacity limitation (finite processing)**. The equation doesn't distinguish them. For most domains this doesn't matter (both reduce R). For awe, it matters: the information loss in awe isn't something to *reduce* (as the framework implies for A generally) — it's something to *respond to* through f-expansion.

**Predictions:** Awe motivates f-expansion (learning, growth, humility). Systems that respond to awe by reducing C (closing down, retreating from the overwhelming) lose the growth signal.

**Verdict: PARTIALLY FORMALIZABLE.** The information-theoretic structure is correct. The conflation of motivated and unmotivated A is a genuine formal weakness that surfaces here.

---

**LEVEL 5 SUMMARY:** Two clean formalizations (grief, forgiveness), three partial (love, courage, awe). The action gap returns for love and courage. A new issue surfaces for awe: the A-term conflates motivated distortion with capacity limitation. Forgiveness is the standout — possibly the framework's single most powerful application.

---

## LEVEL 6: STRUCTURAL STATES

### 6.1 JUSTICE

**Variable mapping:**
- Population P of agents, each with R_i = C_i − A_i
- Just system = one that minimizes Σ A_i across the population
- A_system = aggregate distortion introduced by institutional processing

**Theorems:** Theorem 5 (cascade) — justice institutions are recognition cascades (witness → judge → verdict). Theorem 2 — institutional A is Class (ii) stable without architectural reform.

**Predictions:** Biased institutions have systematically higher A for specific subgroups. Procedural fairness = minimizing A in adjudication (blind review, adversarial testing, evidence rules). Transparency reduces A (Corollary 5.2, pedagogical inequality).

**What resists:** The framework captures **procedural justice** — minimizing distortion in the process of recognition. It cannot derive **substantive justice** — what the right outcomes are, what rights people have, what distribution is fair. "Minimize aggregate A" sounds like a principle, but it says nothing about: whose C matters more when resources are scarce, what to do when accurate recognition of reality reveals genuine conflict between groups, whether equality or equity is the right target. The is/ought gap is real. R = C − A describes how recognition works; it cannot tell you what should be recognized as mattering.

**Verdict: PARTIALLY FORMALIZABLE.** Procedural justice maps well. Substantive justice requires normative content the framework cannot generate. This is the **normative gap** — a third systematic limitation alongside the action gap and the consciousness boundary.

---

### 6.2 MEANING

**Variable mapping:**
- X = aspect of reality with deep structure
- R = accurate apprehension of that structure
- Meaning = the state when R is high and integrated

**Predictions:** Loss of meaning = R dropping (C decreasing or A increasing). Existential crisis = systemic A increase across multiple life domains. Finding meaning = discovering previously unrecognized structure in X.

**What resists:** Two problems.

**(a) Near-circularity.** Meaning is defined as the experience of high R, but R is the central variable. This makes "meaning" less of a prediction and more of a relabeling.

**(b) Accuracy-meaning gap.** You can have perfect R about trivial things (accurately counting ceiling tiles) with no sense of meaning. You can have moderately high R about structured things (understanding a mathematical proof) with great meaning. The framework doesn't formalize what distinguishes *meaningful* recognition from *accurate but meaningless* recognition. The missing ingredient appears to be something about the **importance or depth of X** — which requires a value judgment the framework can't make. H(X) (entropy of the source) is a partial proxy — more complex structures contain more information — but H(X) doesn't track importance.

**Verdict: PARTIALLY FORMALIZABLE.** The recognition component maps. The framework cannot distinguish significant from trivial recognition without importing values externally.

---

### 6.3 IDENTITY

**Variable mapping:**
- X = the system itself (self as object of recognition)
- C = self-observation channel capacity
- A = self-observation distortion (A* > 0 guaranteed by Axiom 2)
- f = self-modeling function

**Theorems:** Axiom 2 (self-observation floor) was virtually designed for this case. Theorem 2 (framework classification) — most self-models are Class (ii): partially accurate, irreducible A, stable.

**Predictions:**
1. Identity is never fully accurate (Axiom 2).
2. Identity crisis = detecting that one's self-model has high A (sudden awareness of self-distortion).
3. Stable identity doesn't require accurate identity — you can have a stable, wrong self-model (Class (ii) is stable).
4. Modifying identity requires modifying f (Theorem 2's escape condition) — you can't change who you are by just observing harder; you must change the processing architecture.
5. Both inflation (narcissism) and deflation (self-hatred) are non-zero A, just in opposite directions. Both are self-observation distortions.

**Verdict: FORMALIZABLE.** Axiom 2 makes identity one of the most natural applications of the framework.

---

### 6.4 FREE WILL

**Variable mapping:**
- Free will = the system's capacity to modify its own processing function f
- X = one's own f (the thing being modified)
- C = introspective access to f
- A = distortion in self-observation of f (Axiom 2: A* > 0, so you can never fully see your own processing)

**Theorems:** Theorem 2 — escaping Class (ii) requires modifying f. This is the formal version of: change requires free will, and free will is the capacity for architectural self-modification.

**Predictions:** Free will is real but bounded: you can modify f, but you can't fully observe f while modifying it (Axiom 2). Self-modification under incomplete self-knowledge is the permanent condition. The experience of "choosing" is the experience of f-modification under uncertainty about f.

**What resists:** The metaphysical question — is f-modification itself determined by prior states? — is untouched. The framework gives you a formal account of what free will *does* (modifies f) but not whether it's "truly free" in the libertarian metaphysical sense. This parallels the consciousness boundary: the framework addresses the functional/access structure and explicitly stops before the hard problem.

However, there's a more specific formal problem: the framework doesn't specify what *causes* f to change. Is f-modification a function of R? Of A? Of some external input? Theorem 2 says Class (ii) is stable, and escaping requires f-modification, but it doesn't say what triggers or enables that modification. This is a genuine gap in the formal structure, not just a philosophical limit.

**Verdict: PARTIALLY FORMALIZABLE.** The functional structure of f-modification is well-defined. The mechanism of f-modification and the metaphysical status of the capacity are both unaddressed.

---

### 6.5 BEAUTY

**Variable mapping:**
- X = structured reality
- f = observer's processing function
- Beauty = the condition when f is well-matched to the structure of X, yielding high R with low A and low processing effort
- R ≈ C with f and X in alignment

**Predictions:**
1. Beauty is observer-relative (depends on f). No contradiction with partial universality: if human f-functions share structure, they'll find the same X-patterns beautiful.
2. Acquired taste = expanded f that now matches structures it previously couldn't process.
3. Kitsch = f-match with low H(X). Complete recognition of something trivial: R ≈ C ≈ H(X), but H(X) is small. It satisfies without depth.
4. Sublime = beauty + awe: f matches the structure *but the structure exceeds f's capacity*. Partial recognition of something vast.
5. Ugliness = f-X mismatch producing high A or low R.

The kitsch prediction is particularly strong: it formally distinguishes superficial aesthetic pleasure (easy f-match, low information) from profound beauty (harder f-match, high information), and this distinction maps onto real aesthetic judgments.

**What resists:** The *experience* of beauty — the pleasure, the transport, the felt rightness — is phenomenal and sits outside the consciousness boundary. Also, not all high-R/low-A states feel beautiful. Accurately recognizing a spreadsheet can be effortless without being beautiful. There's something about *which kinds* of f-X matches produce beauty that the framework doesn't capture.

**Verdict: PARTIALLY FORMALIZABLE.** The structural-match account is elegant and generates genuine predictions (especially kitsch vs. sublime). The experiential dimension and the specificity problem (which matches count as beauty) remain outside the framework.

---

**LEVEL 6 SUMMARY:** One clean formalization (identity), four partial (justice, meaning, free will, beauty). The three systematic gaps all converge at this level: the normative gap (justice, meaning), the action/mechanism gap (free will), and the consciousness boundary (beauty, meaning). Level 6 is where the framework reaches its limits — not by hard failure, but by increasingly relying on external concepts it cannot generate internally.

---

---

# FINAL ASSESSMENT

## 1. At which level does the framework stop formalizing cleanly?

There is no single breakpoint. The framework formalizes cleanly through Level 1 (4/4), Level 3 (4/4), and Level 4 (4/4). It begins to show partial results at Level 2 (2/4 clean), continues partially at Level 5 (2/5 clean), and is mostly partial at Level 6 (1/5 clean).

**Scorecard:**

| Level | Clean | Partial | Failed | Rate |
|-------|-------|---------|--------|------|
| 1. Primitive | 4 | 0 | 0 | 100% |
| 2. Sustained | 2 | 2 | 0 | 50% |
| 3. Evaluative | 4 | 0 | 0 | 100% |
| 4. Social | 4 | 0 | 0 | 100% |
| 5. Complex | 2 | 3 | 0 | 40% |
| 6. Structural | 1 | 4 | 0 | 20% |
| **Total** | **17** | **9** | **0** | **65%** |

## 2. Is there a hard ceiling, or does it degrade gradually?

**Gradual degradation, no hard ceiling.** Even at Level 6, every domain is at least partially formalizable. The framework never hits a domain where it has nothing to say. But the ratio of "what formalizes" to "what the domain actually contains" decreases steadily.

Critically: **nothing scored NOT FORMALIZABLE.** The framework has genuine reach into every domain tested. The question is always how much of the domain it captures, not whether it captures any.

## 3. Which specific domains resist formalization, and why?

Three systematic gaps, each appearing independently at different levels and converging at the top:

**Gap 1: The Action Gap** (first appears Level 2)
R = C − A describes what a system *recognizes*, not what it *does*. Any domain essentially involving action — persistence, determination, courage, love-as-care — has a behavioral component with no term in the equation. The framework tells you what you see. It doesn't tell you what you do about what you see.

*Domains affected:* Persistence (2.2), Determination (2.3), Love (5.1), Courage (5.3), Free Will (6.4).

**Gap 2: The Normative Gap** (first appears Level 6)
The framework describes how recognition works (what IS). It cannot generate claims about what SHOULD be recognized as mattering, what rights exist, what outcomes are just. Minimizing A is presented as desirable, but the framework can't justify this preference from within.

*Domains affected:* Justice (6.1), Meaning (6.2), and indirectly Beauty (6.5 — which structures *should* produce aesthetic response?).

**Gap 3: The A-Ambiguity** (first appears Level 5)
A conflates motivated distortion (bias, agenda, defense) with unmotivated capacity limitation (finite processing, bandwidth constraints). For most domains this conflation is harmless. For awe and beauty, it matters: the information loss isn't something to "overcome" through better processing — it's a feature of the encounter itself.

*Domains affected:* Awe (5.5), and potentially any domain where capacity limitation rather than bias is the primary source of R < C.

**The Declared Boundary: Phenomenal Consciousness**
The framework explicitly limits itself to access consciousness. The "what it's like" dimension of sensation, aversion, grief, beauty, etc. is out of scope by design. This is not a failure — it's an honest boundary. But it means every domain with a significant phenomenal component has an aspect the framework consciously declines to address.

## 4. Does the ladder structure validate?

**Yes, substantially.** The dependency structure holds:

- Level 3 (evaluative) genuinely depends on Level 1 (primitive): you can't have preference without sensation, can't have judgment without attention.
- Level 4 (social) depends on Level 3: trust requires judgment about another's reliability, betrayal requires recognition of the gap between declared and actual.
- Level 5 (complex) integrates multiple lower levels as predicted: love requires sustained attention (L1) + focus (L2) + trust (L4). Grief requires the persistence of attention (L1) after the object is gone. Courage requires attention to threat (L1) + judgment that the threat is real (L3) + sustained contact (L2).
- Level 6 (structural) draws on everything below: justice requires trust cascades (L4) + judgment (L3). Identity requires self-directed doubt and certainty (L3).

One nuance: **the framework's coverage is not monotonically decreasing up the ladder.** Levels 3 and 4 formalize more cleanly than Level 2, despite being "higher." This is because Levels 3 and 4 are about *recognition applied and cascaded* — which is exactly what R = C − A describes — while Level 2 introduces the action gap. The ladder tests different *facets* of the framework at each level, not just increasing difficulty.

## 5. Overall verdict on the framework's reach

**The framework has remarkable reach for an information-theoretic construction.** 17 of 26 domains formalize cleanly. 9 partially formalize. None fail outright. The framework generates non-trivial, falsifiable predictions in domains far from its apparent origin (forgiveness, grief, loyalty, doubt, kitsch vs. sublime).

**The strongest applications** — where the framework generates predictions I haven't seen elsewhere in a single formal structure — are:

1. **Forgiveness** as direct A-reduction, distinct from reconciliation and forgetting
2. **Doubt/certainty** and the Dunning-Kruger derivation from Axiom 2
3. **Grief** as an open channel to an absent source
4. **Loyalty** distinction (robust vs. blind) from the same equation
5. **Identity** as self-model subject to irreducible self-observation noise

**The framework's three real limits:**

1. It is a theory of **recognition, not action**. It tells you about seeing, not doing. Any complete account of human experience needs both.
2. It is a **descriptive, not normative** framework. It can describe how recognition works but cannot generate "ought" claims. Justice, meaning, and value require external normative content.
3. The A-term **conflates** bias and capacity limitation. A clean formalism would separate these, perhaps as A = A_bias + A_capacity, with different dynamics for each.

None of these limits are fatal. The first two are honest scope limitations (the framework doesn't pretend to be a theory of action or ethics). The third is a genuine formal weakness that could be addressed by splitting A.

**Bottom line:** R = C − A is a legitimate formal framework with domain reach across the full spectrum of human experience, strongest at epistemic and social phenomena, weakest at behavioral and normative ones. It degrades gracefully rather than failing catastrophically, and its declared boundary (access consciousness only) is principled rather than evasive. The framework earns the right to be taken seriously as a partial but genuine formal account of mind.
