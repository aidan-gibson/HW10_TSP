# Travelling Salesperson Project

Used Eitan solution for HW9; (I think mine is 100% fine but why play with fire?)

All build files end up in `cmake-build-debug/` (which is .gitignored), so `speed.tsv` and `shortest.tsv` were manually copied from there to root for submission. (Generated files which the assignment asks for must b manually copied to root).

***

### Chromosome Class

dw about `virtual` and `protected` keywords, they'll be important HW11.

chromosomes are represented as `permutation_t` types

`chromosome.h` may add members, but not modify existing members

`chromosome.cpp` only boilerplate written, gotta implement everything in header:

- [x] `is_valid()`checks that the my_order member actually represents a valid permutation (no repeats or gaps). tested, works.
- [x] `is_in_range()` tested, works.
- [x] `calculate_fitness()` 
- [x] augment constructor and destructor as necessary
- [x] `mutate()` pick 2 points at random and swap their values
- [x] `recombine()`



### Deme Class

- [x] Constructor: generate a completely random population of Chromosomes with pop_size individuals. 
- [x] Destructor: clean up any resources you allocated.
- [x] `get_best()`
- [x] `select_parent()`





- [X] Valgrind
  `/usr/bin/valgrind --tool=memcheck --xml=yes --xml-file=/tmp/clion-valgrind433dab77-8a68-4a35-9dd9-cd66df30bb3e/valgrind_output_%p --gen-suppressions=all --leak-check=full --show-leak-kinds=all --leak-resolution=high --show-reachable=yes --track-origins=yes --vgdb=no /home/parallels/CLionProjects/HW10_TSP/cmake-build-debug/HW10_TSP`
Came out clean!


`./HW10_TSP challenge.tsv 10000 0.2`

GA isn't much better than random ):

![](comparison.gif)