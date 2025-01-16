## C4: attack under white-box setting

We adapt TIMIA to white-box setting. In particular, white-box access allows the attacker to measure the loss of the target model and the reference models
on the target sample. Thus, we construct influence feature by

$$
x_I = abs(\mathcal{L}(\mathcal{M}(T)) - \mathcal{L}(\mathcal{M}^{-R_1}(T))) \parallel...\parallel abs(\mathcal{L}(\mathcal{M}(T)) - \mathcal{L}(\mathcal{M}^{-R_m}(T))) 
$$
where $\mathcal{L}(\mathcal{M}(T))$ denotes the loss of target model $\mathcal{M}$ on target sample $T$, $\mathcal{M}^{-R_i}$ denotes the model with reference model $R_i$ removed.
In this table we present the result of TIMIA under black-box setting and white-box setting. The results are measured on Character dataset when the target model is ResNet

|                   | Blackbox | Whitebox |
|-------------------|----------|---------|
| Attack accuracy   | 0.90     | 0.93    |
| TPR@1%FPR         | 42.2%    | 57.4%   |


From the table we observe that TIMIA under white-box setting achieves a higher attack accuracy and TPR@1%FPR. This is expected as the loss on the target sample better reflect the influence of removing reference samples,
and further provids more information for the attacker to infer the membership of the target.