# Melissa Ellison / MonongahelaHellbender

I build refusal-first verification infrastructure for AI-assisted science.

The through-line across my public work is simple: AI and code can generate
substantial outputs quickly; the critical part is knowing what is actually
proven, what is only demonstrated, and what should be refused. My projects make
that boundary runnable.

## Portfolio

| Project | What it is | Trusted base / boundary |
|---|---|---|
| [Barrier Atlas](https://github.com/MonongahelaHellbender/barrier-atlas) | A certified, composable map of impossibilities: each entry names a claim, a certificate, a checker, and a trust rung. | Checkers are one-directional: they can refuse, but they cannot silently promote. Current barriers include SAT/LRAT, independent RUP, Lean axiom audits, composed min-trust barriers, and a finite hybrid Schur/vdW result certified at R2 and R3. |
| [Lean Verification Journey](https://github.com/MonongahelaHellbender/lean-verification-journey) | Lean 4 proofs and small verified checkers across SAT certificates, bounded neural-network robustness, and AI-generated proofs. | The Lean kernel checks the artifact; `#print axioms` records exactly what was trusted. |
| [Certified Combinatorics Verification](https://github.com/MonongahelaHellbender/certified-combinatorics-verification) | A reproducible SAT/RUP pipeline for known Schur and van der Waerden values. | Known finite results, rechecked through explicit certificate pipelines. Not new mathematics. |
| [Chaos Universality Paper](https://github.com/MonongahelaHellbender/chaos-universality-paper) | A public manuscript package and reproducibility bundle for chaos/universality experiments. | Empirical/scientific evidence with seeded artifacts and explicit claim boundaries. Not a formal proof. |
| [Claim Stress Tester](https://github.com/MonongahelaHellbender/claim-stress-tester) | A small tool for routing scientific claims into evidence-quality stress tests. | It does not verify claims; it asks what would support, weaken, or falsify them. |

## The thesis

Most impressive demos answer an **existence** question: *can the system do this
once?* The harder and more durable question is often universal or negative:

- no certificate line is accepted unless the checker verifies it;
- no composed claim earns a stronger trust rung than its weakest part;
- no AI-generated proof is trusted because an AI sounds confident;
- no experimental result becomes a broad claim without its falsifiers.

That is the shape I am interested in: **AI systems can propose artifacts; a
small named trusted base checks them; failed gates stay visible.**

## Safety and risk angle

My safety/risk work focuses on claim boundaries, coverage gaps, misuse-aware
release discipline, privacy-preserving review, and fail-closed gates. I am
especially interested in the gap between existence demos and universal safety
claims: formal verification where specs exist, empirical evaluation where they
do not, and clear refusal where the evidence does not earn the claim.

## Current highlights

- Barrier Atlas now has 9 barriers across 5 checker kinds, with 7 certified, 0
  refused, and 2 honestly deferred in the current public run.
- Its hybrid Schur/van der Waerden finite result is certified two ways: R2 by a
  CNF/RUP certificate accepted by a Lean-proved checker, and R3 by exhaustive
  Python recomputation.
- The R3 independent Python RUP checker is differential-fuzzed against
  `lratcheck` on generated valid and invalid small certificates when the Lean
  binary is available.
- Lean Verification Journey demonstrates the same trust pattern in three
  domains: SAT certificates, bounded neural-network robustness, and AI-generated
  proof checking.
- Chaos Universality Paper keeps empirical claims separate from formal ones;
  its public package is reproducibility evidence, not a theorem certificate.

## What I am looking for

I am interested in collaborations around:

- formal verification and proof-carrying artifacts;
- AI safety assurance, especially claim-boundary, coverage, and evidence-gate design;
- independent checker implementations and differential testing;
- scientific workflows that preserve nulls, refusals, and negative results;
- risk-aware release and documentation practices that avoid guarantee-style overclaims.

If you are evaluating this work, the strongest reading is not “new theorem
factory.” It is: **a working portfolio for building systems that know when not to
believe themselves.**

Public contact route for now: GitHub.
