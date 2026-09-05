Added a simple element to DIAYN which increases coverage across different environments.
DIAYN code was taken from the original paper repo.
for the experiments continuous z's skills were used.


## Initial Results

| Environment | Point | ObstaclePoint | Reacher | MountainCarContinuous |
|---|---:|---:|---:|---:|
| DIAYN | 72.7% | 38.1% | 61.8% | 49.3% |
| **My** | **81.2%** | **74.2%** | **69.3%** | **60.1%** |



## Further Experiments Required

### Baselines
- Comparison to more recent skill discovery methods.

### Environments
- Comparison in more environments, specifically ones used in the literature.

### agnostic to intrinsic exploration methods?
- Can this element be added to other intrinsic reward based exploration methods and improve them as well? (initially mostly across unsupervised skill discovery methods as a start)

### High-Level Policy
- Does this element make it easier for a high-level policy to control the low-level policy through the skills?
- If it is better for higher-level policies, is it because of:
  - Increased coverage, or
  - Some structure in the skills which makes it easier for the higher-level policy to learn to use them?

### Implementation
- Currently the idea is the bare-bones implementation: simple, elegant, and works.
- Explore other implementations and how they affect all of the results, and why.

### Statistical significance testing
- In general more Robust experimentation with multi seed runs for each environment and test statistical significance.

currently the idea is the bare bones implementations. (simple and elegant and works)
but exploring other implementations and how they effect the all of the results, and why.

initial results -
each is a single run, but no hyper parem optimization was done of any kind. simply drop in DIAYN from their repo, and added my element where params for it were kept consistent across the envs and were chosen arbitrarily (I was surprised myself that it works like that off the gate) 



code will be released after publication.
or after doing further experiments and deciding that the results so far were all accidental haha and there is nothing interesting here. (so far not looking like that is the case)

