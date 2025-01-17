## Common Review 2: Additional defenses (Reviewer A)

In this table, we present the attack accuracy and model accuracy when the target model is protected by MemGuard [1],
which will be added to the paper in the revision as a baseline defense.
The results are measured on the Character dataset, with the target model being ResNet.

| Confidence Score Distortion Budget | 0    | 0.20 | 0.40 | 0.60 | 0.80 |
|------------------------------------|------|------|------|------|------|
| Attack accuracy                   | 0.90 | 0.89 | 0.87 | 0.86 | 0.85 |
| Model accuracy                    | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 |

Note that the model accuracy is not affected by the defense, as the label with the highest probability in the model output remains unchanged,
thereby keeping the model accuracy unchanged.

In the implementation, since the defender lacks knowledge of the attacker's strategy,
we follow the setting in [1] and use an MLP as the surrogate attack model. The MLP takes the target model's output vector as input.
Our results demonstrate that MemGuard fails to defend against TIMIA due to its lack of knowledge about the attack features and strategy.
[1] JIA, Jinyuan, et al. Memguard: Defending against black-box membership inference attacks via adversarial examples. In Proceedings of the 2019 ACM SIGSAC conference on computer and communications security.