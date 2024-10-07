## Updates

- We optimized the proof of the main lemma in each of the files `2_input_rewriting.bel`, `3_free_output_rewriting.bel` and `4_bound_output_rewriting.bel`: now they are proved by induction on the derivation of the given transition, rather than on the structure of the process involved. Since these lemmas now take one less argument, `5_theorem1.bel` has been adjusted accordingly.