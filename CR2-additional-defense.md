## Common Review 2: Additional defenses (Reviewer A)

In this table we present the attack accuracy and model accuracy when the target model is protected by MemGuard [1], which will be added to the paper in the revision as a baseline defense.
The results are measured on Character dataset when the target model is ResNet

| Confidence Score Distortion Budget | 0    | 0.20  | 0.40  | 0.60  | 0.80  |
|------------------------------------|------|-------|-------|-------|-------|
| Attack accuracy                   | 0.9  | 0.89  | 0.87  | 0.86  | 0.85  |
| Model accuracy                    | 0.97 | 0.970 | 0.970 | 0.970 | 0.970 |

Note that the model accuracy is not affected by the defense, as the label with the highest probability in the model output will not be changed, thus making the prediction unchanged.
In the implement, as the defender lacks knowledge of the attacker's strategy, we follow the setting in [1] to use a MLP, which takes the target model output vector as the input, as the surrogate
attack model. Our results present that MemGuard fails to defense against TIMIA because of lackness of the knwoledge about the attack feature and the strategy.

