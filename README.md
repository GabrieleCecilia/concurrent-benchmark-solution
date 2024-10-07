# Overview
The [Concurrent Calculi Formalisation Benchmark](https://concurrentbenchmark.github.io/) is a set of challenges focused on the mechanization of models for concurrent and distributed programming languages. In particular, the key problem addressed in the second challenge is reasoning about _scope extrusion_, which occurs when a process transmits a restricted name to another process, expanding its scope to include the receiver.

This repository contains the [Beluga](https://complogic.cs.mcgill.ca/beluga/) source code for a solution to the second challenge in this benchmark, authored by Alberto Momigliano and Gabriele Cecilia. You can read the associated paper, _A Beluga Formalization of the Harmony Lemma in the π-Calculus_, [here](http://www.arxiv.org/abs/2407.06624).
- The `code/` directory contains the Beluga source files.
- The `thesis` file includes Gabriele Cecilia's MS thesis, which offers a detailed discussion of this work.

## Install and usage instructions
This mechanization is compatible with Beluga version 1.1.1.

For installation, please refer to the [installation guide](https://github.com/Beluga-lang/Beluga/blob/master/INSTALL) in the GitHub repository of Beluga.

Once Beluga is installed, you can type-check the project by running it on the file `all.cfg`. The following is the expected output:

```
>> beluga all.cfg
## Type Reconstruction begin: ./1_definitions.bel ##
## Type Reconstruction done:  ./1_definitions.bel ##
## Type Reconstruction begin: ./2_input_rewriting.bel ##
## Type Reconstruction done:  ./2_input_rewriting.bel ##
## Type Reconstruction begin: ./3_free_output_rewriting.bel ##
## Type Reconstruction done:  ./3_free_output_rewriting.bel ##
## Type Reconstruction begin: ./4_bound_output_rewriting.bel ##
## Type Reconstruction done:  ./4_bound_output_rewriting.bel ##
## Type Reconstruction begin: ./5_theorem1.bel ##
## Type Reconstruction done:  ./5_theorem1.bel ##
## Type Reconstruction begin: ./6_stepcong_lemma.bel ##
## Type Reconstruction done:  ./6_stepcong_lemma.bel ##
## Type Reconstruction begin: ./7_reduction_rewriting.bel ##
## Type Reconstruction done:  ./7_reduction_rewriting.bel ##
## Type Reconstruction begin: ./8_theorem2.bel ##
## Type Reconstruction done:  ./8_theorem2.bel ##
```
