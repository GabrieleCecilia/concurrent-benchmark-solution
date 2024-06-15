# Nats
In this version of the formalization we present a slight modification of the set of names, so that it includes an explicit copy of the natural numbers (the "names" type also retains the possibility of having any number of distinct variables added at need, as in the original formalization). Since we added some explicit closed terms to the type "names", a subcase of the "cong_fstepright_impl_fstepleft" lemma, which performs a case analysis on a contextual name, needs to be slightly adjusted to account for these new names. Aside from this modification, the rest of the code type-checks without any further changes.

Refer to the main branch for the explanation of the content of each Beluga file.
