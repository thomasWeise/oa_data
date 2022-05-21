# Experimental Data of the Book "Optimization Algorithms" 

Here we provide the data of the experiments conducted for the electronic book "[Optimization Algorithms](https://thomasweise.github.io/oa)".


## Job Shop Scheduling Problem (JSSP)

### Random Sampling-Related Algorithms

These algorithms make random search moves without using information from the objective function.

- [`jssp_1rs.zip`](jssp/jssp_1rs.zip): The results of the single random sampling algorithm.
  813&nbsp;kB zipped, 1.8&nbsp;MB unzipped.
- [`jssp_rs.zip`](jssp/jssp_rs.zip): The results of the (multiple) random sampling algorithm.
  828&nbsp;kB zipped, 1.8&nbsp;MB unzipped.
- [`jssp_rw_swap2.zip`](jssp/jssp_rw_swap2.zip): The results of a random walks using the operator `swap2` that swaps two (different) job IDs.
  846&nbsp;kB zipped, 1.9&nbsp;MB unzipped.


### Hill Climbers (HC)

These algorithms are simple local searches that accept only *strictly improving* moves.

- [`jssp_hc_swap2.zip`](jssp/jssp_hc_swap2.zip): The results of a hill climber using the operator `swap2` that swaps two (different) job IDs.
  992&nbsp;kB zipped, 2.2&nbsp;MB unzipped.
- [`jssp_hcr_swap2.zip`](jssp/jssp_hcr_swap2.zip): The results of the hill climber with restarts using the operator `swap2` that swaps two (different) job IDs, for different restart settings.
  14.5&nbsp;MB zipped, 31.6&nbsp;MB unzipped.
- [`jssp_hc_swapn.zip`](jssp/jssp_hc_swapn.zip): The results of a hill climber using the operator `swapn` that swaps a randomly chosen number (different) of job IDs.
  1&nbsp;MB zipped, 2.2&nbsp;MB unzipped.
- [`jssp_hcr_swapn.zip`](jssp/jssp_hcr_swapn.zip): The results of the hill climber with restarts using the operator `swapn` that swaps a randomly chosen number of (different) job IDs, for different restart settings.
  14.4&nbsp;MB zipped, 31.2&nbsp;MB unzipped.
  
  
### Random Local Search (RLS)

These algorithms are simple local searches that accept all moves that are either improving or lead to the same objective values, i.e., all non-worsening moves.

- [`jssp_rls_swap2.zip`](jssp/jssp_rls_swap2.zip): The results of a Random Local Search (RLS) using the operator `swap2` that swaps two (different) job IDs.
  1.3&nbsp;MB zipped, 2.9&nbsp;MB unzipped.
- [`jssp_rls_swapn.zip`](jssp/jssp_rls_swapn.zip): The results of a Random Local Search (RLS) using the operator `swapn` that swaps a randomly chosen number of (different) job IDs.
  1.3&nbsp;MB zipped, 2.8&nbsp;MB unzipped.


## License

This dataset is released under the Attribution-NonCommercial-ShareAlike 4.0 International license (CC&nbsp;BY&#8209;NC&#8209;SA&nbsp;4.0), see [http://creativecommons.org/licenses/by-nc-sa/4.0/](http://creativecommons.org/licenses/by-nc-sa/4.0/) for a summary.
