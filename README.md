Added a simple element to DIAYN which increases coverage across different environments.
DIAYN code was taken from the original paper repo.
for the experiments continuous z's skills were used.

further experiments required -
comparison to more recent skill discovery methods.
comparison in more envs, specifically ones used in literature.
can this element be added to other skill discovery methods and improve them as well.
does this element make it easier later for high level policy to control the low level policy through the skills. 
if it is better for higher level policies is it because increased coverage or is it because it encourages some structure in the skills which makes it easier to learn to use for the higher lvl policy.

currently the idea is the bare bones implementations. (simple and elegant and works)
but exploring other implementations and how they effect the all of the results, and why.

initial results -

## Initial Results

| Environment | Point | ObstaclePoint | Reacher | MountainCarContinuous |
|---|---:|---:|---:|---:|
| DIAYN | 72.7% | 38.1% | 61.8% | 49.3% |
| **Ours** | **81.2%** | **74.2%** | **69.3%** | **60.1%** |

