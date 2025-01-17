## Reviewer B3: number of reference model

In the following table we present the number of shadow models and number of reference models of TIMIA and the baseline attacks presented .

| Attack                                      | Number of shadow models | Number of reference models   | Total number of shadow models and reference models |
|---------------------------------------------|-------------------------|------------------------------|----------------------------------------------------|
| GMIA [1]                                    | 0                       | N                            | N                                                  |
| MIA [2]                                     | 1                       | 0                            | 1                                                  |
| RAM (Baseline with random reference sample) | 1                       | $\vert\mathcal{R}\vert$      | $\vert\mathcal{R}\vert + 1$                        |
| TIMIA (Our Method)                          | 1                       | $\vert\mathcal{R}\vert$      | $\vert\mathcal{R}\vert + 1$                        |

$N$ denotes the number of reference models or shadow models used by GMIA, 
while $|\mathcal{R}|$ denotes the number of reference samples in TIMIA, which can be as small as 2 in our experiment. 
When $|\mathcal{R}| \approx N$, the number of reference models in TIMIA is comparable to the number of shadow models in GMIA.

[1] Long, Yunhui, Lei Wang, Diyue Bu, Vincent Bindschaedler, Xiaofeng Wang, Haixu Tang, Carl A. Gunter, and Kai Chen. "A pragmatic approach to membership inferences on machine learning models." In 2020 IEEE European Symposium on Security and Privacy (EuroS&P), pp. 521-534. IEEE, 2020.

[2] Shokri, Reza, Marco Stronati, Congzheng Song, and Vitaly Shmatikov. "Membership inference attacks against machine learning models." In 2017 IEEE symposium on security and privacy (SP), pp. 3-18. IEEE, 2017.
