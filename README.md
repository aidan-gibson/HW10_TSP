# Travelling Salesperson Project

Used Eitan solution for HW9; (I think mine is 100% fine but why play with fire?)

All build files end up in `cmake-build-debug/` (which is .gitignored), so `speed.tsv` and `shortest.tsv` were manually copied from there to root for submission. (Generated files which the assignment asks for must b manually copied to root).

***

### Chromosome Class

dw about `virtual` and `protected` keywords

chromosomes are represented as `permutation_t` types

`chromosome.h` may add members, but not modify existing members

`chromosome.cpp` only boilerplate written, write all



- [x] `is_valid()`checks that the my_order member actually represents a valid permutation (no repeats or gaps). tested, works.
- [x] `is_in_range()` tested, works.











- [ ] Valgrind
