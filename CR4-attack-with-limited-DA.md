## Common-Review-4: Attack with limited DA (Reviewer B & C)

In this table we present the attack accuracy and TPR@1%FPR of TIMIA when the size of $D_A$ is small. In particular, we assure that
 $|DA|/|D_T|\in$ [1%, 2%, 3%],
assuring that $|D_A|$ is smaller than 30. For each target we pick 6 reference samples,
which takes 20% of $|D_A|$. The results are measured on Character dataset when the target model is ResNet

| $\|D_A\|\|D_T\|$ | 1%    | 2%    | 3%    |
|------------------|-------|-------|-------|
| Attack accuracy  | 0.86  | 0.88  | 0.89  |
| TPR@1%FPR        | 29.60% | 32.20% | 36.70% |


From the results we observe that TIMIA still achieves a high performance when the size of $D_A$ is small, which is no lower than 0.86 and 29.6\% 
in terms of attack accuracy and TPR@1\%FPR
