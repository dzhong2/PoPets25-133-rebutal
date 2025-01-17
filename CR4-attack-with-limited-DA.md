## Common-Review-4: Attack with limited DA (Reviewer B & C)

In this table, we present the attack accuracy and TPR@1%FPR of TIMIA when the size of $D_A$ is small.
Specifically, we ensure that $\|D_A\| / \|D_T\| \in [1%, 2%, 3%]$, with $|D_A|$ being smaller than 30.
For each target, we select 6 reference samples, which constitute 20% of $|D_A|$. 
The results are measured on the Character dataset, with the target model being ResNet.

| $\|D_A\|/\|D_T\|$ | 1%    | 2%    | 3%    |
|-------------------|-------|-------|-------|
| Attack accuracy   | 0.86  | 0.88  | 0.89  |
| TPR@1%FPR         | 29.60% | 32.20% | 36.70% |


From the results, we observe that TIMIA still achieves high performance when the size of $D_A$ is small,
with attack accuracy no lower than 0.86 and TPR@1%FPR no lower than 29.6%.