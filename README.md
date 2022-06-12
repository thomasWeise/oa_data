# Experimental Data of the Book "Optimization Algorithms" 

Here we provide the data of the experiments conducted for the electronic book "[Optimization Algorithms](https://thomasweise.github.io/oa)".
These experiments have been done using the *The Metaheuristic Optimization in Python*, [`moptipy`](https://thomasweise.github.io/moptipy/index.html) for short.


## Job Shop Scheduling Problem (JSSP)

### Random Sampling-Related Algorithms

These algorithms make random search moves without using information from the objective function.

- [`jssp_1rs.zip`](jssp/jssp_1rs.zip): The results of the [single random sampling](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.single_random_sample) algorithm.
  813&nbsp;kB zipped, 1.8&nbsp;MB unzipped.
- [`jssp_rs.zip`](jssp/jssp_rs.zip): The results of the (multiple) [random sampling](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.random_sampling) algorithm.
  828&nbsp;kB zipped, 1.8&nbsp;MB unzipped.
- [`jssp_rw_swap2.zip`](jssp/jssp_rw_swap2.zip): The results of a [random walks](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.random_walk) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  846&nbsp;kB zipped, 1.9&nbsp;MB unzipped.


### Hill Climbers (HC)

[Hill climbers](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.hill_climber) are algorithms are simple local searches that accept only *strictly improving* moves.

- [`jssp_hc_swap2.zip`](jssp/jssp_hc_swap2.zip): The results of a [hill climber](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.hill_climber) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  992&nbsp;kB zipped, 2.2&nbsp;MB unzipped.
- [`jssp_hcr_swap2.zip`](jssp/jssp_hcr_swap2.zip): The results of the [hill climber with restarts](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.hill_climber_with_restarts) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs, for different restart settings.
  14.5&nbsp;MB zipped, 31.6&nbsp;MB unzipped.
- [`jssp_hc_swapn.zip`](jssp/jssp_hc_swapn.zip): The results of a [hill climber](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.hill_climber) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number (different) of job IDs.
  1&nbsp;MB zipped, 2.2&nbsp;MB unzipped.
- [`jssp_hcr_swapn.zip`](jssp/jssp_hcr_swapn.zip): The results of the [hill climber with restarts](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.hill_climber_with_restarts) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number of (different) job IDs, for different restart settings.
  14.4&nbsp;MB zipped, 31.2&nbsp;MB unzipped.
  
  
### Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.rls))

Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.rls))-style algorithms are simple local searches that accept all moves that are either improving or lead to the same objective values, i.e., all non-worsening moves.
Depending on the field and representation used, they are also known under different names, such as, for example, `(1+1) EA` if the search space are bit strings and the search operator flips each bit with the same probability.

- [`jssp_rls_swap2.zip`](jssp/jssp_rls_swap2.zip): The results of a Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.rls)) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  1.3&nbsp;MB zipped, 2.9&nbsp;MB unzipped.
- [`jssp_rls_swapn.zip`](jssp/jssp_rls_swapn.zip): The results of a Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.rls)) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number of (different) job IDs.
  1.3&nbsp;MB zipped, 2.8&nbsp;MB unzipped.


### Evolutionary Algorithms (EAs)

Evolutionary Algorithms (EAs) maintain a population of solutions.
They start with a population of `mu` random solutions.
In each iteration, they keep the `mu` best solutions in the population.
Then they create `lambda` new solutions by applying search operators to them and add them to the population.

- [`jssp_eanocr_swap2`(jssp/jssp_eanocr_swap2.zip): The results of an [EA without binary operator](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#moptipy.algorithms.ea_without_crossover.EAnoCR)using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  44.5&nbsp;MB zipped, 93.7&nbsp;MB unzipped.


## License

This dataset is released under the Attribution-NonCommercial-ShareAlike 4.0 International license (CC&nbsp;BY&#8209;NC&#8209;SA&nbsp;4.0), see [http://creativecommons.org/licenses/by-nc-sa/4.0/](http://creativecommons.org/licenses/by-nc-sa/4.0/) for a summary.
