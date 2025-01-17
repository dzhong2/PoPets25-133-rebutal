## Reviewer B3: number of reference model

In the following table we present the number of shadow models and number of reference models of TIMIA and the baseline attacks.

| Attack                                  | MIA  | GMIA | RAM/TIMIA |
|-----------------------------------------|------|------|-----------|
| Number of shadow models (1 target)      | N    | 0    | 1         |
| Number of shadow models (K targets)     | N    | 0    | 1         |
| Number of reference models (1 target)   | 0    | N    | $\vert\mathcal{R}\vert$   |
| Number of reference models (K targets)  | 0    | N*K  | K*$\vert\mathcal{R}\vert$ |

$N$ denotes the number of reference models or shadow models used by the baselines, 
while $|\mathcal{R}|$ denotes the number of reference samples in TIMIA.
When $|\mathcal{R}| \approx N$, the number of reference models in TIMIA is comparable to the number of shadow models in the baselines.


