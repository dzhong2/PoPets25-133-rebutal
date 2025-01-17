## Common Review 1: Additional attacks (Reviewer A & B & C)

In this table, we present the attack accuracy and TPR@1%FPR of the baseline attacks to be added in the revision.
The results are measured on the Character dataset, with the target model being ResNet.

| Attacks applied in paper | TIMIA | ML-leak [1] | Mentr [2]      |  LiRA [3]  |  RMIA [4]  |
|--------------------------|-------|------------|------------|------------|------------|
| ACC                      | 0.90  | 0.59       | 0.61       | 0.65       | 0.71       |
| TPR@1%FPR                | 42.2% | 3.7%       | 6.2%       | 16.5%      | 19.4%      |
| Suggested reviewer             |  -    | Reviewer A | Reviewer A | Reviewer B | Reviewer C |

From the results, we observe that TIMIA achieves higher attack accuracy than the four attacks in terms of both ACC and TPR@1%FPR.




[1] SALEM, Ahmed, et al. Ml-leaks: Model and data independent membership inference attacks and defenses on machine learning models. arXiv preprint arXiv:1806.01246, 2018. (Accepted by NDSS 2019)

[2] SONG, Liwei; MITTAL, Prateek. Systematic evaluation of privacy risks of machine learning models. In: 30th USENIX Security Symposium (USENIX Security 21). 2021. p. 2615-2632.

[3] Carlini, Nicholas, Steve Chien, Milad Nasr, Shuang Song, Andreas Terzis, and Florian Tramer. "Membership inference attacks from first principles." In 2022 IEEE Symposium on Security and Privacy (SP), pp. 1897-1914. IEEE, 2022.

[4] Zarifzadeh, Sajjad, Philippe Liu, and Reza Shokri. "Low-Cost High-Power Membership Inference Attacks." In Forty-first International Conference on Machine Learning. 2024. 