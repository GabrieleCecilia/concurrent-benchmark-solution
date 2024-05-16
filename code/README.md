# concurrent-benchmark-solution/code
The solution consists of the following files:

- [1_definitions.bel](1_definitions.bel):
formalization of syntax and semantics (reduction, LTS) of the pi-calculus

- [2_input_rewriting.bel](2_input_rewriting.bel), [3_free_output_rewriting.bel](3_free_output_rewriting.bel), [4_bound_output_rewriting.bel](4_bound_output_rewriting.bel):
lemmas about rewriting (up to structural congruence) of processes involved in input/free output/bound output transitions

- [5_theorem1.bel](5_theorem1.bel):
proof of the first theorem about semantics equivalence (tau-transition implies reduction)

- [6_stepcong_lemma.bel](6_stepcong_lemma.bel):
lemma stating that, given two congruent processes P and Q and a transition from P to P', then Q makes a transition through the same action to some process Q' congruent to P'. This file also contains a technical strengthening lemma necessary for this proof.

- [7_reduction_rewriting.bel](7_reduction_rewriting.bel):
lemma about rewriting (up to structural congruence) of processes involved in a reduction

- [8_theorem2.bel](8_theorem2.bel):
proof of the second theorem about semantics equivalence (reduction implies tau-transition, up to congruence)

- [all.cfg](all.cfg):
cfg file containing all the previous Beluga files

The directory [semantics-equivalence](semantics-equivalence) contains proofs of the equivalence of early/late LTS and Honsell/Miller & Tiu LTS encodings.
The directory [updates](updates) contains some later proof optimization for few Beluga files.
