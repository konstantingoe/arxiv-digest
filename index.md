---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest 2026-W31

**Week of July 20 -- 27, 2026**

Categories scanned: `stat.ME`, `math.ST`, `stat.ML`, `cs.LG`
Papers scanned: 400 of ~689 in window | Papers selected: 13

---

## Causal Discovery & Structure Learning

### Local Causal Structure Learning in the Presence of Latent Variables and Selection Bias
**Zheng Li, Hao Zhang, Ruxin Wang, Ruichu Cai, Kun Zhang**
[arXiv:2607.19866](https://arxiv.org/abs/2607.19866) | `cs.LG`

Proposes a local causal discovery algorithm that recovers the direct causes and effects of a target variable without reconstructing the full global graph, under both latent confounders and selection bias. The key contribution is a characterisation of a local ancestral region that supports target-specific discovery, plus a theoretical bridge connecting causal information in this region to identifiable structures under FCI-style assumptions.

*Why relevant:* Directly addresses local causal discovery under unmeasured confounders and selection bias — the exact setting of local JCI and Markov boundary identification with latent variables.

---

### Learning Bidirectional Causal Interactions with Heteroscedastic Neural Networks
**Masahiro Tanaka**
[arXiv:2607.22313](https://arxiv.org/abs/2607.22313) | `stat.ML`, `cs.LG`, `stat.ME`

Introduces SEM-DNN, a simultaneous-equation neural network estimator for reciprocal structural interactions between endogenous variables. Identification is achieved without instruments by exploiting conditional covariance diagonalization: when structural shocks are conditionally uncorrelated with nonproportional conditional variances given covariates, only the true structural coefficients diagonalize the conditional residual covariance across the feature space.

*Why relevant:* Extends heteroscedasticity-based identification to bidirectional/cyclic non-linear SEMs without instruments; relevant to discovery in systems with feedback and unknown confounders.

---

### CEDAR: Causal Edge Discovery for Autoregressive Processes
**Mohammad Fesanghary**
[arXiv:2607.20696](https://arxiv.org/abs/2607.20696) | `cs.LG`, `stat.ME`

A constraint-based method for lagged causal edge discovery in sparse multivariate time series. CEDAR pre-screens candidate lags using AR(1)-residualized, U-centred distance covariance, then applies two targeted conditional independence tests per surviving candidate lag, followed by an MCI-inspired pruning step to remove indirect edges.

*Why relevant:* Directly uses distance covariance as a CI screening statistic in a constraint-based structure learning pipeline — bridges dcov-based testing with practical time-series causal discovery.

---

### Reconstruction of Enhanced Causal Omnidirectional Network (RECON)
**Praveen Niranda, Peter T. McKenney, Guifang Fu**
[arXiv:2607.21833](https://arxiv.org/abs/2607.21833) | `stat.ME`, `stat.ML`

Proposes an integral-based nonparametric additive ODE model for reconstructing regulatory/causal networks from multiple discrete-time trajectory observations. Incorporates data-driven edge selection, stability-constrained estimation, and time-varying extensions; outperforms existing ODE-based approaches on synthetic and real gene-expression benchmarks.

*Why relevant:* Nonparametric additive structure for causal graph recovery from time-course data; the integral formulation and edge-selection procedure connect to sparse additive methods for causal discovery.

---

## Interventional Methods & Identification

### Interventional Score Geometry for Causal Inference
**Mojtaba Eslami**
[arXiv:2607.21914](https://arxiv.org/abs/2607.21914) | `stat.ME`, `cs.AI`, `econ.EM`

Develops an interventional analogue of score geometry: a hard intervention do(*X*_k = ξ) restricts the distribution to the submanifold {*x*_k = ξ}, so the relevant score is defined on the remaining *d*−1 free coordinates. Causal influence *X*_k ↝ *X*_j is then defined as variation of the conditional score ∂_j log *p*(*x*_{−k} | *x*_k) with respect to the intervention value ξ, yielding a geometry that distinguishes causal direction where purely observational score geometry cannot.

*Why relevant:* Offers a new geometric characterisation of interventional distributions and causal direction; directly applicable to score-function-based causal discovery and identifiability under hard interventions.

---

### Identification and Robust Inference for Multiple Treatment Effects with Possibly Invalid Instruments
**Ziwei Mei, Qingliang Fan, Zijian Guo**
[arXiv:2607.21481](https://arxiv.org/abs/2607.21481) | `stat.ME`

Studies linear IV models with multiple endogenous treatments when some instruments may be invalid. Shows that the multi-treatment identification problem is fundamentally harder than the scalar case (each valid instrument identifies a hyperplane in effect space), derives sharp identification conditions, and proposes robust inference procedures controlling type-I error under partial instrument invalidity.

*Why relevant:* Advances identification theory for causal effects under unmeasured confounders with multiple treatments; the hyperplane geometry of multi-treatment IV is relevant to settings with multiple unknown soft-intervention targets.

---

### Equilibrium Causal Digital Twins: Validation, Transport, and Identification Limits
**Faraz Dadgostari, Neda Nazemi**
[arXiv:2607.21667](https://arxiv.org/abs/2607.21667) | `stat.ME`, `cs.MA`, `eess.SY`

Studies when causal predictions from digital twins trained in one context can be validated and transported to another. For equilibrium causal games with feedback, derives conditions on mechanisms, equilibrium selection, and intervention design under which agreement with experimental distributions identifies the target counterfactual. Shows that moment agreement is insufficient for distributional queries, and characterises identification limits via selection diagrams.

*Why relevant:* Transportability and identification limits for equilibrium/feedback causal systems; uses selection diagrams and links to the do-calculus transportability framework.

---

## Conditional Independence Testing

### Local Permutation Tests for Conditional Independence: An Adaptive Binning Perspective
**David Chen, Rohan Hore, Rina Foygel Barber**
[arXiv:2607.20751](https://arxiv.org/abs/2607.20751) | `stat.ME`, `math.ST`

Extends the local permutation test (LPT) for conditional independence *X* ⊥ *Y* | *Z* by replacing pre-fixed *Z*-space partitions with data-adaptive binning strategies that balance bin sizes. Establishes finite-sample validity for the adaptively-binned LPT and demonstrates improved power over fixed-partition tests, particularly in high dimensions where a fixed grid creates highly imbalanced bins.

*Why relevant:* Direct advance in CI testing methodology; the adaptive binning strategy addresses a practical limitation of LPT relevant to constraint-based causal discovery pipelines.

---

## Causal Inference & Semiparametric Methods

### Optimal Use of a Black-Box Learner in Semiparametric Estimation
**Yihong Gu**
[arXiv:2607.21541](https://arxiv.org/abs/2607.21541) | `math.ST`, `stat.ME`, `stat.ML`

In the partial linear model *Y* = μ₀(*X*) + β₀·*T* + ε with black-box nuisance estimation, derives a novel estimator achieving the optimal rate n^{−1/2} + δ_{a,μ}·δ_{a,π} + δ_s², with a matching lower bound. The product term for approximation errors matches DML, but the squared excess-risk term δ_s² strictly improves on DML when the hypothesis class has excess risk above n^{−1/4}.

*Why relevant:* Establishes minimax-optimal causal effect estimation rates under black-box nuisance learning; the tighter bound informs when nonparametric causal effect estimators can achieve root-n efficiency.

---

### GAUGER: Generalized Regression Adjustment via Graph-Weighted Exposure-Level Residualization for Causal Inference Under Interference
**Lei Shi, Rita Lyu, Sizhu Lu**
[arXiv:2607.19627](https://arxiv.org/abs/2607.19627) | `stat.ME`

Reveals a "mismatch between accuracy and efficiency" in network causal inference: model adjustments minimising prediction error do not maximise variance reduction in treatment-effect estimators under interference. Proposes GAUGER, a graph-weighted regression adjustment that targets variance reduction directly via graph-structured exposure-level residualisation, with design-based validity and formal efficiency guarantees.

*Why relevant:* Advances design-based causal inference under network interference; the graph-weighted residualisation directly exploits causal graph structure for efficiency.

---

### Bounding the Causal Impact of ML-Assisted Decision-Making via Counterfactual Correctness
**Jonathan Zhang, Erik Skalnes, Jacob Chen, Michael Oberst**
[arXiv:2607.21806](https://arxiv.org/abs/2607.21806) | `cs.LG`

Proposes "counterfactual correctness" — a property of ML predictions that, when satisfied, bounds the causal impact of deploying a model on downstream outcomes without running a new RCT after each model update. Derives sharp partial identification bounds on causal effects from observational deployment data when counterfactual correctness holds approximately.

*Why relevant:* Uses partial identification and counterfactual reasoning to bound causal effects of deployment interventions; methodologically connects to identifiability under latent confounders.

---

### Information Criteria Exploiting Latent Structure for Model Selection in Structural Equation Models
**Marion Naveau, Magalie Houée-Bigot, Matthieu Marbac, Anouk Zancarini, Mathieu Emily**
[arXiv:2607.21053](https://arxiv.org/abs/2607.21053) | `stat.ME`

Proposes two information criteria for SEM model selection derived from the integrated *complete*-data likelihood, explicitly accounting for the latent variable structure rather than marginalising it away. The first adapts ICL to Gaussian SEMs; the second approximates the integrated observed-data log-likelihood via importance sampling that incorporates latent structural information.

*Why relevant:* Addresses model selection in SEMs with latent variables using criteria that respect the latent structure — relevant to graphical model and causal SEM selection where the number of latent confounders must be chosen.

---

### Weighted Extensions of the Kolmogorov-Smirnov, Cramer-von Mises, and Anderson-Darling Tests for Assessing Covariate Balance
**Ariel Linden**
[arXiv:2607.21782](https://arxiv.org/abs/2607.21782) | `stat.ME`

Extends three classical distributional tests (KS, CvM, AD) to accommodate case weights of any origin (propensity scores, IPTW, matching weights) via a shared label-permutation inference procedure requiring no assumptions about weight generation. Simulation confirms type-I error control at nominal levels across substantial weight variability.

*Why relevant:* Principled distributional balance diagnostics for weighted observational causal inference; the permutation-based inference is assumption-free and applicable with any weighting scheme from propensity or causal models.

---

*Digest generated automatically on 2026-07-27. 400 of ~689 papers scanned via the arXiv API. Only papers actually returned by the API are included — no fabricated entries.*

---

## Archive

- [2026-W31](archive/2026-W31.md) -- July 20 -- 27, 2026 (13 papers)
- [2026-W29](archive/2026-W29.md) -- July 13 -- 20, 2026 (15 papers)
- [2026-W28](archive/2026-W28.md) -- June 29 -- July 6, 2026 (14 papers)
- [2026-W27](archive/2026-W27.md) -- June 22 -- 29, 2026 (19 papers)
- [2026-W26](archive/2026-W26.md) -- June 15 -- 22, 2026 (15 papers)
- [2026-W25](archive/2026-W25.md) -- June 10 -- 17, 2026 (19 papers)
