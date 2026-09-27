30th & 5th

Quantitative Research – Take-Home Assessment (v2)

Pure Lambda Calculus · Research Questions

Duration: 24 hours · Difficulty: Hard · Focus: Syntax, Semantics, Types, Observational Theory



NOTICE: This is a fictional practice assessment created for educational purposes. “30th & 5th” is not a real firm. The problems are original research-style questions intended to approximate the depth expected in a demanding quant research take-home centered on the foundations of the λ-calculus.



Instructions

You have 24 hours from the moment you begin. Submit a written solutions document (Markdown or PDF). Optional supporting code (OCaml/Haskell) is welcome but secondary to mathematical content.





Prefer rigorous proofs. When citing standard results, state them precisely and supply the critical inductive or constructive steps for the syntax you use.



Open-book for standard references (Barendregt, Hindley–Seldin, Pierce, Girard, Abramsky–Jung, etc.). Solutions must be your own.



Partial answers that show genuine insight rank higher than complete but shallow ones.



State any extra assumptions clearly.



Problem 1 — Reduction Theory & Head Normal Forms

(a) Residual theory.
Define residuals of a redex with respect to a reduction sequence. Prove that residuals of a single redex under a reduction are pairwise disjoint (non-overlapping). Use this to give a clean proof that β-reduction is weakly Church-Rosser (local confluence).

(b) Head reduction.
Define head reduction and head normal form (HNF). Prove that a term has an HNF if and only if the head-reduction strategy terminates on it. Show that solvability is equivalent to possession of an HNF.

(c) Perpetual reductions.
Construct, for any term that has no normal form, an infinite reduction sequence that never reaches a normal form (a perpetual reduction). Contrast this with the fact that leftmost reduction is normalizing whenever a normal form exists.

(d) Conservation theorem.
State and prove the Conservation Theorem: if M is solvable and M →β N, then N is solvable. Deduce that unsolvability is preserved under reduction.



Problem 2 — Typed Systems & Computational Content

(a) Strong normalization via reducibility.
Prove strong normalization of the simply-typed λ-calculus using Girard’s reducibility candidates (or Tait’s saturated sets). Explicitly verify the key “CR3 / saturation” properties for arrow types.

(b) η-long normal forms.
Define η-long normal forms for STLC. Prove that every typable term has a unique η-long β-normal form. Explain the relevance of uniqueness for decision procedures and for the correspondence with natural deduction normal proofs.

(c) System F and impredicativity.
Show how to encode pairs, sums, and natural numbers in System F. Prove that the polymorphic fixed-point combinator is not typable in System F, and explain why this is consistent with strong normalization.

(d) Inhabitation & classical principles.
Which of the following types are inhabited in STLC? In System F? In λμ-calculus (or classical natural deduction)?





((A → B) → A) → A



¬¬A → A



((A → B) → A) → ((A → B) → B) → B

Give inhabitants or proofs of non-inhabitation, and comment on the computational interpretation of the classical principles involved.



Problem 3 — Denotational & Operational Models

(a) Term models.
Construct both the closed term model and the open term model of the untyped λ-calculus. Determine precisely which equations each validates (β, η, or neither). Show an explicit counter-example to η in the open term model.

(b) Filter models / intersection-type models.
Outline the construction of a filter model based on intersection types. Explain how the interpretation of a term is the set of types that can be assigned to it, and why this yields a λ-model that characterises solvability.

(c) Sequentiality & full abstraction (outline).
What is sequentiality in the sense of Berry–Curien or Kahn–Plotkin? Why do continuous function models (such as D∞) fail to be fully abstract for PCF? Sketch the idea behind game semantics or sequential algorithms as a route to full abstraction.

(d) Observational vs denotational equivalence.
Prove that if two terms have the same denotation in a sensible model (e.g., a model that is adequate), then they are observationally equivalent. Give a concrete example of two observationally equivalent terms that are distinguished by a non-fully-abstract model.



Problem 4 — Choose Two Advanced Directions

Develop substantial answers for exactly two of the following.

(A) Böhm’s theorem & separability.
State Böhm’s theorem on the separability of distinct βη-normal forms. Prove the finite case (or give a detailed proof sketch). Discuss the consequences for the lattice of λ-theories.

(B) Realizability.
Present a simple realizability interpretation (e.g., Kleene realizability or a typed variant). Show how it validates the axiom of choice for finite types or a form of Markov’s principle, and discuss the computational content extracted from a proof.

(C) Quantitative / resource-sensitive calculi.
Define a simple resource λ-calculus (or the differential λ-calculus fragment). Explain how coefficients or multiplicities track usage. Give an example where ordinary β-reduction loses information that the resource calculus retains.

(D) Abstract machines.
Describe the Krivine abstract machine (or the SECD machine) for weak-head reduction. Prove correctness with respect to the operational semantics of head reduction. Discuss the relationship between environment machines and the categorical notion of a closed Freyd category or a sequential algorithm.



Problem 5 — Original Research Question

Formulate one precise research question suggested by the material above, then give a non-trivial partial answer.

Acceptable directions include (but are not limited to):





Complexity of deciding observational equivalence for restricted classes of terms (linear terms, affine terms, terms of bounded order, typable terms of bounded rank).



Characterisation of the λ-theories induced by particular models (e.g., which equations hold in all continuous models, or in all stable models).



Extraction of computational content from classical proofs via CPS or λμ, and analysis of the resulting programs’ complexity or observational behaviour.



Relationships between intersection-type characterisations of normalization and modern quantitative type systems (e.g., non-idempotent intersection types, graded types).

Your submission for this problem must contain:





A clear statement of the question.



Necessary definitions.



At least one genuine partial result, construction, counter-example, or reduction.



A short discussion of significance and possible routes to a full solution.



Evaluation Criteria





Rigor — correctness and completeness of definitions and proofs.



Depth — ability to move fluently between syntax, operational semantics, denotational models, and logic.



Clarity — precise, well-organised exposition.



Insight — recognition of subtle points, limitations, or interesting special cases.



Originality — especially in the choice of advanced topics and the research question.



— End of Assessment —

Good luck. Prefer depth over breadth.
