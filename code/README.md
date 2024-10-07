## Project Files Overview
Below are the files that are included in this project.

```
all.cfg                      - Collects all used Beluga source files
1_definitions.bel            - Contains encoding of syntax and semantics of the pi-calculus
2_input_rewriting.bel,       - Contain proofs of rewriting lemmas for specific transitions
3_free_output_rewriting.bel,
4_bound_output_rewriting.bel 
5_theorem1.bel               - Proof of the first theorem about semantics equivalence
6_stepcong_lemma.bel         - Contains proofs of a congruence-as-bisimilarity and a strengthening lemma 
7_reduction_rewriting.bel    - Contains proof of a rewriting lemma for reductions
8_theorem2.bel               - Proof of the second theorem about semantics equivalence

```

- `semantics-equivalence/` contains proofs of the equivalence of early/late LTS and Honsell/Miller & Tiu LTS encodings.
- `updates/` contains some later proof optimization for Beluga files.

## Paper to Code Table
The following table provides a comparison between definitions and proofs of the project [paper](http://www.arxiv.org/abs/2407.06624) (_A Beluga Formalization of the Harmony Lemma in the π-Calculus_) and the Beluga code.

| Definition/Proofs                             | Paper         | File                         | Definition Name                           |
|-----------------------------------------------|---------------|------------------------------|-------------------------------------------|
| Names, processes                              | Section 3.1   | 1_definitions.bel            | names, proc                               |
| Congruence, reduction                         | Section 3.2   | 1_definitions.bel            | cong, red                                 |
| Actions, transitions                          | Section 3.3   | 1_definitions.bel            | f_act, b_act, f_step, b_step              |
| Rewriting lemma for input transitions         | Section 3.4.1 | 2_input_rewriting.bel        | bs_in_rew                                 |
| Rewriting lemma for free output transitions   | Section 3.4.1 | 3_free_output_rewriting.bel  | fs_out_rew                                |
| Rewriting lemma for bound output transitions  | Section 3.4.1 | 4_bound_output_rewriting.bel | bs_out_rew                                |
| Theorem 1 (1st Harmony Lemma implication)     | Section 3.4.1 | 5_theorem1.bel               | fstep_impl_red                            |
| Strengthening lemma                           | Section 3.4.2 | 6_stepcong_lemma.bel         | strengthen_fstep, strengthen_bstep        |
| Congruence-as-bisimilarity lemma              | Section 3.4.2 | 6_stepcong_lemma.bel         | cong_fstepleft_impl_fstepright, cong_fstepright_impl_fstepleft, cong_bstepright_impl_bstepleft, cong_fstepleft_impl_fstepright |
| Rewriting lemma for reductions                | Section 3.4.2 | 7_reduction_rewriting.bel    | red_impl_red_rew                          |
| Theorem 2 (2nd Harmony Lemma implication)     | Section 3.4.2 | 8_theorem2.bel               | red_impl_fstepcong                        |
