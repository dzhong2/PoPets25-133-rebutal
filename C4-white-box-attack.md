## C4: attack under white-box setting

We adapt TIMIA to white-box setting. In particular, white-box access allows the attacker to measure the loss of the target model and the reference models
on the target sample. Thus, we construct influence feature by

$$
x_I = abs(\mathcal{L}(S(T)) - \mathcal{L}(S^{-R_1}(T))) \parallel...\parallel abs(\mathcal{L}(S(T)) - \mathcal{L}(S^{-R_m}(T))) 
$$

In this table we present the result of TIMIA under black-box setting and white-box setting. The results are measured on Character dataset when the target model is ResNet

|                   | Blackbox | Whitebox |
|-------------------|----------|----------|
| Attack accuracy   | 0.90     | 0.93     |
| TPR@1%FPR         | 42.2%    | 57.40%   |


From the table we observe that TIMIA under white-box setting achieves a higher attack accuracy and TPR@1%FPR. This is expected as the loss on the target sample better reflect the influence of removing reference samples,
and further provids more information for the attacker to infer the membership of the target.