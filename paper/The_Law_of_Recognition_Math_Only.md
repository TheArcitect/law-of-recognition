# The Law of Recognition: Formal Content Only

## R = C − A

**This document contains only the axioms, definitions, theorems, proofs, and formal structure. No prose, no examples, no applications, no worked demonstrations.**

---

## Definitions

**R (Recognition)** — accurate apprehension of what is actually present. Formally: R = I(X; f(Y)), where X is reality, Y is observation, f is observer processing.

**C (Contact)** — degree of encounter with reality. Formally: C = I(X; T_β(Y)), where T_β is the information bottleneck variable at capacity limit β → ∞.

**A (Agenda)** — post-channel distortion. Formally: A = I(X; T_β(Y)) − I(X; f(T_β(Y))). Exclusively post-channel: biases, motivated reasoning, confirmation-seeking applied after observation.

**A Decomposition.** A = A_bias + A_capacity, where A_bias is motivated distortion (defense, desire, ideology — reducible through architectural change) and A_capacity is unmotivated limitation (finite processing, bandwidth constraints — reducible through expansion of f). Both satisfy A_bias ≥ 0, A_capacity ≥ 0. The distinction matters for intervention: A_bias responds to debiasing, A_capacity responds to training. Axiom 2 applies to both components: A*_bias > 0 and A*_capacity > 0 for self-observing systems.

**The Equation:**
$$R = C - A$$
$$R = I(X;\, f(Y)) = I(X;\, T_\beta(Y)) - [I(X;\, T_\beta(Y)) - I(X;\, f(T_\beta(Y)))]$$

---

## Axioms

**Axiom 1 (DPI / Non-negativity).** For any recognition triple: A ≥ 0.

By the Data Processing Inequality: I(X; f(Y)) ≤ I(X; Y). Therefore A = C − R ≥ 0. □

**Axiom 2 (Self-Observation Floor / Non-Splitting).** For any self-modeling system S, the sequence 0 → A_self → C_self → R_self → 0 does not split.

Define A⁽⁰⁾ = A, A⁽ᵏ⁺¹⁾ = A_measurement(A⁽ᵏ⁾). The self-observation channel has Markov structure A⁽ᵏ⁾ → Y_meta → A⁽ᵏ⁺¹⁾ with strictly positive measurement noise variance σ² > 0.

Contraction condition: Decompose A_measurement = g ∘ E[·|Y_meta], where g captures self-reinforcing feedback with gain factor γ = sup_a |g'(a)| ≥ 1, and E[·|Y_meta] is the conditional-mean operator with attenuation factor λ = Var(A)/(Var(A) + σ²) < 1. The composite Lipschitz constant is L = γλ, where L measures the net effect of self-observation: whether measurement noise (λ < 1) dominates self-reinforcing bias (γ ≥ 1), or vice versa.

When L < 1 (noise attenuation dominates feedback gain): A_measurement is a contraction mapping and Banach-Caccioppoli gives convergence to a unique fixed point A*. The fixed point satisfies A* > 0 because A_measurement(0) > 0: measuring zero agenda still introduces strictly positive meta-agenda from the measurement apparatus itself (σ² > 0 guarantees this). Non-zero kernel prevents splitting.

When L ≥ 1 (confirmation-bias regime): the contraction fails and {A⁽ᵏ⁾} may diverge or oscillate. The sequence remains bounded (A⁽ᵏ⁾ ∈ [0, H(X)] by Theorem 1), so any limit point is a fixed point, but uniqueness and convergence are not guaranteed. The non-splitting conclusion holds a fortiori. Both regimes yield A* > 0. □

**Axiom 3 (Substrate Independence / Functoriality).** For categories 𝒞₁, 𝒞₂ with recognition structures and exact functor F : 𝒞₁ → 𝒞₂, the image of the exact sequence is exact.

---

## Channel Boundary

C is identified with the mutual information between source and observation at the channel's capacity limit, via the information bottleneck framework (Tishby et al., 1999):

$$C = I(X;\, T_\beta(Y))$$

A is exclusively post-channel distortion:

$$A = I(X;\, T_\beta(Y)) - I(X;\, f(T_\beta(Y)))$$

Capacity-optimal compression is absorbed into C. Structural loss H(X) − C is channel limitation, not agenda.

The measurement protocol: improve the channel (increase β) and observe what changes. Define 𝒟 = {β : dC/dβ > 0}. On 𝒟:

$$\rho(\beta) = \frac{dR/d\beta}{dC/d\beta}, \qquad \beta \in \mathcal{D}$$

When ρ = 1, all channel improvement converts to recognition. When ρ < 1, some channel improvement is absorbed by increasing agenda. When ρ = 0, bottleneck has shifted entirely to A.

At capacity saturation (β → β* where dC/dβ → 0), ρ is undefined. The diagnostic is replaced by dR/dβ = dC/dβ − dA/dβ.

---

## Decoder Resolution

Decoders expand C, not A. Training rewrites the channel's conditional distribution: p(Y_trained|X) ≠ p(Y_untrained|X). Training is not post-processing — it is channel expansion (changing p(Y|X)).

Formally: X = reality, Y_observer = perception through channel, Z = f(Y_observer) where f encodes biases.

$$C = I(X;\, Y_{\text{observer}})$$
$$A = I(X;\, Y_{\text{observer}}) - I(X;\, f(Y_{\text{observer}}))$$
$$R = I(X;\, f(Y_{\text{observer}})) = C - A$$

The DPI guarantees A ≥ 0. Different observers have different C values.

---

## Boundary Criterion

Dynamic test: increase contact, observe trajectory.

$$\frac{dR}{dC} > 0 \implies \text{C-expanding (consistent estimator)}$$
$$\frac{dR}{dC} \leq 0 \text{ despite increasing C} \implies \text{A-injecting (inconsistent estimator)}$$

The capacity-derivative formulation:

$$\frac{dR}{d\beta} = \frac{dC}{d\beta} - \frac{dA}{d\beta}$$

When dA/dβ > 0 (improving channel increases agenda), framework is actively resisting contact.

### The Partition Problem

R = C − A does not provide a domain-general method for determining the C/A partition. The structure is general. The partition is not.

Three partial resolutions: (1) convergence criterion — components invariant across independent observers more likely C; (2) interventionist criterion — modify processing, measure changes; (3) structural transfer — calibrate in ground-truth domains, transfer structure to contested domains.

---

## Theorem 1: Recognition Capacity Bound

Recognition is bounded above by the entropy of reality: R(n) ≤ H(X). Recognition is bounded by contact: R(n) ≤ C(n), by the DPI. Contact is non-decreasing and, under sufficiently diverse observations with a non-degenerate channel, converges to H(X). Marginal returns to contact diminish under i.i.d. or exchangeable observations.

*Proof.* By the chain rule for mutual information, the DPI, and martingale convergence. The bound is tight — achieved when processing is a sufficient statistic. □

## Theorem 2: Framework Classification

Frameworks partition into three classes based on asymptotic recognition:

**(i) Full recognition:** R_∞ = H(X). A(n) → 0.
**(ii) Partial recognition:** 0 < R_∞ < H(X). A_∞ > 0.
**(iii) Null recognition:** R_∞ = 0.

Class (ii) is stable, not transitional.

*Proof.* Trichotomy on the reals: R_∞ ∈ [0, H(X)] implies exactly one of (i), (ii), (iii).

**Existence of Class (ii).** Suppose f factors through a fixed lossy map T: f = g ∘ T where sup_n I(X; T(Y^n)) ≤ C_T < H(X). By the DPI:

$$R(n) \leq I(X;\, T(Y^n)) \leq C_T < H(X)$$

As C(n) → H(X): A(n) = C(n) − R(n) ≥ C(n) − C_T → H(X) − C_T > 0. Therefore A_∞ ≥ H(X) − C_T > 0.

**Stability.** By Fano's inequality, P_e ≥ (H(X|f(Y^n)) − 1)/log|𝒳|. Since A_∞ > 0 implies H(X|f(Y^n)) bounded away from zero, error probability remains strictly positive for all n. Escaping Class (ii) requires modifying the processing architecture itself. □

## Theorem 3: Thermodynamic Cost of Agenda

By Landauer's principle: any logically irreversible erasure of one bit dissipates at least k_B T ln 2 of energy.

When observer applies processing f to observation Y:

$$E_A \geq A(n) \cdot k_B T \ln 2$$

All processing is physically instantiated. When f erases information (which the DPI says it does when A > 0), Landauer applies. Axiom 3 guarantees no processing regime is exempt.

Lower bound on a lower bound: thermodynamic cost of total erasure by f is at least the agenda cost, but may be substantially larger.

## Theorem 4: Convergence Rate

**Definition.** The *framework learning rate* α is the supremum of rates γ ≥ 0 such that A(n) − A_∞ ≤ K_A · exp(−γn) for some K_A > 0 and all sufficiently large n.

Recognition converges at rate limited by min(D*, α), where D* is channel quality (Chernoff information) and α is framework learning rate.

*Proof.* Decompose: H(X) − R(n) = (H(X) − C(n)) + A(n).

Contact gap: By Chernoff-Stein lemma, P_e(n) ≤ exp(−D* · n + o(n)). Applying Fano's inequality: H(X) − C(n) = H(X|Y^n) ≤ K₁ · exp(−D* · n).

Agenda gap: By definition of α, for every γ < α: A(n) − A_∞ ≤ K_γ · exp(−γn).

Therefore for any γ < α:
$$H(X) - R(n) \leq K_1 \cdot e^{-D^* \cdot n} + A_\infty + K_\gamma \cdot e^{-\gamma \cdot n}$$

For Class (i) (A_∞ = 0): asymptotic convergence exponent is min(D*, α). □

## Theorem 5: The Recognition Cascade

For a chain R_1 → D_1 → R_2 → D_2 → R_3...:

$$R_n \leq R_{n-1} \quad \text{for all } n$$

*Proof.* At stage k, the DPI applied twice — once to dissemination, once to next recognition step — yields R_{k+1} ≤ R_k. By induction. □

**Scope note.** Theorem 5 holds for pure chains. For non-chain topologies (DAGs) where a receiver has independent contact with reality — i.e., I(X; C_ind | C_transmitted) > 0 — the receiver's total recognition R_n may exceed R_{n-1} through fresh contact not derived from the chain. The cascade bound applies only to the transmitted component.

---

## Corollaries of the Cascade

### Corollary 5.1: The Transparent Agenda Paradox

A disseminator who declares intent provides the receiver with side information for decoding. By Wyner-Ziv (1976):

$$I(X;\, Z, A_D) \geq I(X;\, Z)$$

Net information loss approaches the irreducible uncertainty floor of the disseminator's self-knowledge (Axiom 2 applies to disseminator).

Boundary condition: Under cheap talk (Crawford-Sobel 1982), adversarial agents can declare false agendas at zero cost. Honest declaration must be a costly signal (Spence 1973).

### Corollary 5.2: The Pedagogical Inequality

Using rate-distortion theory, for sufficiently large R:

$$D_T(R) \leq D_O(R)$$

where D_T is minimum distortion under transparent dissemination and D_O under ostensibly objective dissemination. Fails for naive receivers, capacity-constrained channels, and adversarial receivers.

### Corollary 5.3: The Generation Problem

The cascade R_n ≤ R_{n-1} applies to transmitted content fidelity. It does not bound the receiver's total recognition state, because the receiver has independent contact with reality.

---

## Mathematical Structure

### The Adjunction

Define the residuated lattice **L** = ([0, H(X)], ≤, +, 0). The residuation:

$$A \otimes R \leq C \quad \text{iff} \quad R \leq A \to C$$

where A → C = max(C − A, 0). The tensor-hom adjunction:

$$\mathrm{Hom}(A \otimes R,\, C) \cong \mathrm{Hom}(R,\, [A, C])$$

holds on domain restriction Ω = {(C, A) : A ≤ C}.

The DPI guarantees Ω universally in the formal domain: A = I(X; Y) − I(X; f(Y)) ≤ I(X; Y) = C.

Structural parallel is at the monoidal closed level (linear logic: information cannot be freely duplicated or discarded).

### Three-Regime Partition

**Formal** (Ω guaranteed by DPI, adjunction unconditional): information theory, signal detection, Bayesian inference.

**Informal-healthy** (Ω maintained by sufficient contact, adjunction conditional).

**Informal-pathological** (Ω violated, A > C, recognition collapses to lattice bottom).

### The Effect Algebra

**Definition.** E = [0, H(X)], where a ⊕ b = a + b when a + b ≤ H(X), undefined otherwise.

**Definition.** A *recognition triple* (C, A, R) ∈ E³ with A ⊕ R = C, A ≥ 0, R ≥ 0.

**Definition.** The recognition exact sequence in E:
```
0 ──► A ──ι──► C ──π──► R ──► 0
```
ι : A ↪ C is inclusion; π : C ↠ R sends C ↦ C − A. Exactness holds at each position by construction.

---

## The Central Adjunction (Lawvere Quantale)

In the Lawvere quantale (ℝ₊, +, 0):

$$\mathrm{Hom}(A + R,\, C) \cong \mathrm{Hom}(R,\, [A, C])$$

where [A, C] = C − A. R = C − A is the right residual of C with respect to A. Same adjunction as: conjunction ⊣ implication (logic), product ⊣ exponential (topology), application ⊣ currying (computation).

---

## The Temporal Extension: Spectral Sequence

Static triple → filtered process:
- C(t) = I(X; Y¹,...,Yᵗ)
- A(t) = I(X; Yᵗ) − I(X; f_t(Yᵗ))
- R(t) = C(t) − A(t)

C(t) is non-decreasing. R(t) is not monotone: decreases when dA/dt > dC/dt.

**Convergence Rate Theorem.** ‖Eᵣ − E_∞‖ ≤ K · exp(−r · min(D*, α))

**Bottleneck theorem.** If D* is binding, need more data. If α is binding, need better framework.

**Second equation:** τ = 1/min(D*, α) — characteristic convergence time.

---

## Theorem 6: Meta-Recursive Generativity

### Definitions

**6.1 (Framework).** F = (Ω, R, C, A) with domain Ω of (observer, reality) pairs and functions R, C, A : Ω → [0, ∞) satisfying R = C − A and Axioms 1–3.

**6.2 (Transmission event).** T = (O_s, O_r, F, D) where O_s is sender with recognition R_s, O_r is receiver, D is dissemination channel with agenda A_D.

**6.3 (Meta-application).** Φ(F) = {(O, T) : T is a transmission event of F and O has a channel to T}.

**6.4 (Instance).** Specific (ω, R, C, A) together with at least one falsifiable prediction.

**6.5 (Novel instance).** Instance I of Φ(F) is novel if its falsifiable prediction is not logically derivable from predictions generated by F on non-transmission domains prior to the transmission event.

**6.6 (Generative framework).** F is generative if Φ(F) contains at least one novel instance.

### Statement

Let F satisfy Axioms 1–3. Suppose:
- **(P1)** There exists at least one transmission event T of F.
- **(P2)** Receiver O_r has independent contact C_ind with I(X; C_ind | C_transmitted) > 0.
- **(P3)** Receiver's agenda about framework satisfies A_r(F) < C_r(F).

Then:

**(a) Self-Applicability [Theorem].** Ω_T ⊂ Ω.

**(b) Validity [Theorem].** Every (O, T) ∈ Ω_T satisfies Axioms 1–3.

**(c) Receiver Surplus [Theorem].** R_total > R_transmitted.

**(d) Novelty [Conjecture].** At least one instance produced by Φ(F) is novel.

**(e) Boundedness [Theorem].** Σ_i R_i ≤ H(X_structure).

**(f) Convergence [Theorem].** Under finite observer populations, Φ^n(F) converges: D* = ⋃_n Φ^n(F) is finite and stable.

### Proofs

**(a):** By Axiom 3, Ω contains all (observer, reality) pairs where observer has channel to reality. T exists in reality. Any observer O witnessing T has channel to T. Therefore (O, T) ∈ Ω. □

**(b):** Markov chain: T → Y_O → f_O(Y_O). Axiom 1: DPI gives A ≥ 0. Axiom 2: meta-observation carries own bias. Axiom 3: definitions invoke only observer, channel, processing. □

**(c):** By P2, I(X; C_ind | C_transmitted) > 0. By chain rule:
$$I(X; C_{\text{transmitted}}, C_{\text{ind}}) = I(X; C_{\text{transmitted}}) + I(X; C_{\text{ind}} | C_{\text{transmitted}}) > I(X; C_{\text{transmitted}})$$
When A_r is small (P3), R_total > R_transmitted. □

**(e):** By Theorem 1: R ≤ H(X). Finite populations → finite transmission events → bounded sum. □

**(f):** D_n = ⋃_{k≤n} Φ^k(F) is non-decreasing. Each application generates ≤ |observers|² new events. Each distinct instance contributes ≥ δ > 0 bits. Total bounded by H(X_structure). Therefore at most ⌊H(X_structure)/δ⌋ distinct instances. D_n stabilizes. □

### A_model Bound

$$R_{\text{meta}} = C_{\text{meta}} - A_{\text{model}}$$
$$G_{\text{genuine}} \in [\max(0, G_{\text{observed}} - A_{\text{model}}), G_{\text{observed}}]$$

Interval width = A_model. Irreducible for single observer. Convergence requires multiple independent observers.

---

## Consciousness Boundary

**Theorem (Domain Claim).** R = C − A is a theory of access consciousness (Block 1995). Phenomenal consciousness is not an object in InfoCat.

**Theorem (Two-Entity Minimum).** Recognition of consciousness is structurally irreducible to a single-entity operation.

*Proof.* System S observing own phenomenal experience: by Axiom 2, A_self > 0. S cannot distinguish "I am conscious" from "my processing generates output 'I am conscious'" from inside. External observer O with independent contact can recognize properties of S that S cannot. Minimum two entities required. □

**Corollary.** The explanatory gap IS the self-observation floor. A_self > 0 guarantees no functional system can close the gap. This is a theorem, not a limitation of current theory.

---

## Derived Propositions Summary

**Monotonicity.** C(n) = I(X; Y¹,...,Yⁿ) ↑ H(X) under i.i.d. non-degenerate observation.

**Trichotomy.** Class I (Full): R∞ = H(X), A∞ = 0. Class II (Partial): 0 < R∞ < H(X), A∞ > 0. Class III (Null): R∞ = 0.

**Cascade.** Rₙ ≤ Rₙ₋₁ ≤ ... ≤ R₁.

**Bottleneck.** Convergence rate = min(D*, α). Wrong bottleneck → no improvement.

**Self-Application.** The theory predicts its own A. Predicts necessity of external review. Predicts Axiom 2 applies to its own construction.

---

*End of formal content. No examples. No applications. No worked demonstrations.*
