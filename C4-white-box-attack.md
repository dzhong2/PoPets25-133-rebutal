## C4: attack under white-box setting

We adapt TIMIA to white-box setting. In particular, white-box access allows the attacker to measure the loss of the target model and the reference models
on the target sample. Thus, we construct influence feature by

$$
x_I = |\mathcal{L}(S(T)) - \mathcal{L}(S^{-R_1}(T))| ||...|||\mathcal{L}(S(T)) - \mathcal{L}(S^{-R_m}(T))| 
$$