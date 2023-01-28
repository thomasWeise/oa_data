# Experimental Data of the Book "Optimization Algorithms" 

Here we provide the data of the experiments conducted for the electronic book "[Optimization Algorithms](https://thomasweise.github.io/oa)".
These experiments have been done using the *The Metaheuristic Optimization in Python*, [`moptipy`](https://thomasweise.github.io/moptipy/) for short.
All datasets are provided in the `tar.xz` format, which can be unpacked by the default archive manager of several Linux distributions as well as [WinRAR](https://www.rarlab.com/download.htm).


## Job Shop Scheduling Problem (JSSP)

The Job Shop Scheduling Problem ([JSSP](https://thomasweise.github.io/moptipy/moptipy.examples.jssp.html#module-moptipy.examples.jssp)) is a classical NP-hard optimization problem where the goal is to find schedules (assignments of jobs to machines) that complete as fast as possible.
Each of the `n` jobs of a JSSP instance must be processed by `m` machines in a job-specific sequence, requiring a specific runtime on each machine.

### Random Sampling-Related Algorithms

These algorithms make random search moves without using information from the objective function.

- [`jssp_1rs.tar.xz`](jssp/jssp_1rs.tar.xz): The results of the [single random sampling](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.single_random_sample) algorithm.
  514&nbsp;kB packed, 2.3&nbsp;MB unpacked.
- [`jssp_rs.tar.xz`](jssp/jssp_rs.tar.xz): The results of the (multiple) [random sampling](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.random_sampling) algorithm.
  550&nbsp;kB packed, 2.5&nbsp;MB unpacked.
- [`jssp_rw_swap2.tar.xz`](jssp/jssp_rw_swap2.tar.xz): The results of a [random walks](https://thomasweise.github.io/moptipy/moptipy.algorithms.html#module-moptipy.algorithms.random_walk) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  483&nbsp;kB packed, 1.9&nbsp;MB unpacked.


### Hill Climbers ([HC](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber))

[Hill climbers](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber) are algorithms are simple local searches that accept only *strictly improving* moves.

- [`jssp_hc_swap2.tar.xz`](jssp/jssp_hc_swap2.tar.xz): The results of a [hill climber](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  680&nbsp;kB packed, 3.0&nbsp;MB unpacked.
- [`jssp_hcr_swap2.tar.xz`](jssp/jssp_hcr_swap2.tar.xz): The results of the [hill climber with restarts](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber_with_restarts) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs, for different restart settings.
  6.7&nbsp;MB packed, 32.4&nbsp;MB unpacked.
- [`jssp_hc_swapn.tar.xz`](jssp/jssp_hc_swapn.tar.xz): The results of a [hill climber](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number (different) of job IDs.
  714&nbsp;kB packed, 2.9&nbsp;MB unpacked.
- [`jssp_hcr_swapn.tar.xz`](jssp/jssp_hcr_swapn.tar.xz): The results of the [hill climber with restarts](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.hill_climber_with_restarts) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number of (different) job IDs, for different restart settings.
  6.7&nbsp;MB packed, 31.7&nbsp;MB unpacked.
  
  
### Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.rls))

Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.rls))-style algorithms are simple local searches that accept all moves that are either improving or lead to the same objective values, i.e., all non-worsening moves.
Depending on the field and representation used, they are also known under different names, such as, for example, `(1+1) EA` if the search space are bit strings and the search operator flips each bit with the same probability.

- [`jssp_rls_swap2.tar.xz`](jssp/jssp_rls_swap2.tar.xz): The results of a Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.rls)) using the [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  910&nbsp;kB packed, 3.9&nbsp;MB unpacked.
- [`jssp_rls_swapn.tar.xz`](jssp/jssp_rls_swapn.tar.xz): The results of a Random Local Search ([RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.rls)) using the [operator `swapn`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swapn) that swaps a randomly chosen number of (different) job IDs.
  840&nbsp;kB packed, 3.3&nbsp;MB unpacked.


### Evolutionary Algorithms (EAs)

Evolutionary Algorithms ([EAs](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.ea)) maintain a population of solutions.
They start with a population of `mu` random solutions.
In each iteration, they keep the `mu` best solutions in the population.
Then they create `lambda` new solutions by applying search operators to them and add them to the population.

- [`jssp_ea_no_binary_swap2.tar.xz`](jssp/jssp_ea_no_binary_swap2.tar.xz): The results of an Evolutionary Algorithm ([EA](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.ea)) using the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs and no binary operator.
  56.2&nbsp;MB packed, 239.9&nbsp;MB unpacked.
- [`jssp_ea_gap_swap2.tar.xz`](jssp/jssp_ea_gap_swap2.tar.xz): The results of an Evolutionary Algorithm ([EA](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.ea)) using the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs and the binary generalized alternating position [operator `gap`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#moptipy.operators.permutations.op2_gap.Op2GeneralizedAlternatingPosition).
  54.3&nbsp;MB packed, 238.9&nbsp;MB unpacked.
- [`jssp_generalEa.tar.xz`](jssp/jssp_generalEa.tar.xz): The results of a general [Evolutionary Algorithm](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#moptipy.algorithms.so.general_ea.GeneralEA) with configurable fitness assignment process, survival selection, and mating selection.
  As fitness assignment process, we use either the objective values [directly](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.fitnesses.html#module-moptipy.algorithms.so.fitnesses.direct), their [ranks](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.fitnesses.html#module-moptipy.algorithms.so.fitnesses.rank), or their [ranks combined with the iteration indices](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.fitnesses.html#module-moptipy.algorithms.so.fitnesses.rank_and_iteration).
  As selection algorithms, we test [fitness proportionate selection](https://thomasweise.github.io/moptipy/moptipy.algorithms.modules.selections.html#module-moptipy.algorithms.modules.selections.fitness_proportionate_sus), tournament selection [with](https://thomasweise.github.io/moptipy/moptipy.algorithms.modules.selections.html#module-moptipy.algorithms.modules.selections.tournament_with_repl) and [without](https://thomasweise.github.io/moptipy/moptipy.algorithms.modules.selections.html#module-moptipy.algorithms.modules.selections.tournament_without_repl) replacements, [best](https://thomasweise.github.io/moptipy/moptipy.algorithms.modules.selections.html#module-moptipy.algorithms.modules.selections.best) selection, and [random selection](https://thomasweise.github.io/moptipy/moptipy.algorithms.modules.selections.html#module-moptipy.algorithms.modules.selections.random_without_repl).
  All setups use the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs and the binary generalized alternating position [operator `gap`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#moptipy.operators.permutations.op2_gap.Op2GeneralizedAlternatingPosition) at a rate of 0.125 as well as &#x3BC;=&#x3BB;&#x2208;{4,32}.
  10.0&nbsp;MB packed, 43.7&nbsp;MB unpacked.


### Simulated Annealing (SA)

Simulated Annealing ([SA](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.simulated_annealing)) is similar to RLS in that it is a local search that always accepts any non-worsening move.
However, different from RLS, it also sometimes accepts a move to a solution worse than the current one.
The probability to accept such a move is the higher the higher the current "[temperature](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#moptipy.algorithms.so.temperature_schedule.TemperatureSchedule.temperature)" is and the lower the worse the move is.
The "temperature" is controlled by a [temperature schedule](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.temperature_schedule).

- [`jssp_sa_swap2.tar.xz`](jssp/jssp_sa_swap2.tar.xz): The results of a Simulated Annealing ([SA](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.simulated_annealing)) algorithm with [exponential](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#moptipy.algorithms.so.temperature_schedule.ExponentialSchedule) temperature schedule and the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) that swaps two (different) job IDs.
  32.2&nbsp;MB packed, 150.7&nbsp;MB unpacked.
 

### Memetic Algorithms (MA)

Memetic Algorithms (MAs) are basically Evolutionary Algorithms where each solution is refined by another algorithm, usually a local search, for a pre-defined number of `ls_fes`&nbsp;FEs.
We can implement this concept in several different ways, e.g., as a [MA with hard-wired RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.marls), or as a [MA where arbitrary algorithms can be plugged in](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.ma).
Here we provide the results of the former (MA+RLS) and the latter (MA+Simulated Annealing).

- [`jssp_marls_gap_swap2.tar.xz`](jssp/jssp_marls_gap_swap2.tar.xz): The results of an [MA with hard-wired RLS](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.marls) using our binary [operator `gap`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#moptipy.operators.permutations.op2_gap.Op2GeneralizedAlternatingPosition) and the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) in the RLS for different values of `ls_fes` and `mu=lambda`.
  34.2&nbsp;MB packed, 185.7&nbsp;MB unpacked. 
- [`jssp_masa_gap_swap2.tar.xz`](jssp/jssp_masa_gap_swap2.tar.xz): The results of an [MA](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.ma) with [Simulated Annealing](https://thomasweise.github.io/moptipy/moptipy.algorithms.so.html#module-moptipy.algorithms.so.simulated_annealing) (SA) plugged it, using our binary [operator `gap`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#moptipy.operators.permutations.op2_gap.Op2GeneralizedAlternatingPosition) and the unary [operator `swap2`](https://thomasweise.github.io/moptipy/moptipy.operators.permutations.html#module-moptipy.operators.permutations.op1_swap2) in the SA for different values of `ls_fes` and &#x3BC;=&#x3BB.
  The SA is configured to have a starting temperature&nbsp;`T_0` of&nbsp;16 and has &#x3B5; set such that after 80% of `ls_fes` has been consumed, the temperature will be approximately&nbsp;0.22.
  38.8&nbsp;MB packed, 185.6&nbsp;MB unpacked.


## License

This dataset is released under the Attribution-NonCommercial-ShareAlike 4.0 International license (CC&nbsp;BY&#8209;NC&#8209;SA&nbsp;4.0), see [http://creativecommons.org/licenses/by-nc-sa/4.0/](http://creativecommons.org/licenses/by-nc-sa/4.0/) for a summary.


## Contact

If you have any questions or suggestions, please contact
Prof. Dr. [Thomas Weise](http://iao.hfuu.edu.cn/5) (汤卫思教授) of the 
Institute of Applied Optimization (应用优化研究所, [IAO](http://iao.hfuu.edu.cn)) of the
School of Artificial Intelligence and Big Data ([人工智能与大数据学院](http://www.hfuu.edu.cn/aibd/)) at
[Hefei University](http://www.hfuu.edu.cn/english/) ([合肥学院](http://www.hfuu.edu.cn/)) in
Hefei, Anhui, China (中国安徽省合肥市) via
email to [tweise@hfuu.edu.cn](mailto:tweise@hfuu.edu.cn) with CC to [tweise@ustc.edu.cn](mailto:tweise@ustc.edu.cn).
