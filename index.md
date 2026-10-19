---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest — 2026-W43

**Period covered:** 2026-10-12 to 2026-10-19  
**Categories scanned:** stat.ME, math.ST, stat.ML, cs.LG  
**Papers scanned:** ~1000 (top results by recency)  
**Papers kept:** 20

---

## Causal Discovery & Structure Learning

### 1. Causal Discovery beyond Conditional Independence: Identifiability, Algorithms, and Statistical Inference for Directed Acyclic and Cyclic Graphs
**Yang Ni** | stat.ME | 2026-10-16  
[https://arxiv.org/abs/2610.23543](https://arxiv.org/abs/2610.23543)

A comprehensive review of modern causal discovery methods that exploit distributional properties beyond conditional independence—covering functional model constraints (ANMs, LiNGAM), score-based identifiability, interventional data, and cyclic graphs, with a unified treatment of algorithms and inference.  
*Why relevant:* Directly covers the full scope of the research profile—ANMs, identifiability beyond CI, interventional discovery, DAG and cyclic structure learning.

---

### 2. Using Heteroscedasticity for Causal Discovery under Hidden Confounding
**Jing Zou, Wei Li, Wei Lin** | stat.ME | 2026-10-15  
[https://arxiv.org/abs/2610.21219](https://arxiv.org/abs/2610.21219)

Exploits non-constant residual variance (heteroscedasticity) as a signal for orienting edges in DAGs even when unmeasured confounders are present, bypassing the need for valid instruments. Provides identification conditions and a practical algorithm.  
*Why relevant:* Directly addresses the core challenge of causal discovery under latent confounding; connects to the JCI/soft-intervention identification literature.

---

### 3. Generalizing Identifiability Results in Causal Discovery from Complete Data to Missing Data Settings
**Matteo Ceriscioli, Shohei Shimizu, Mallika Gupta, Karthika Mohan** | stat.ML | 2026-10-13  
[https://arxiv.org/abs/2610.19211](https://arxiv.org/abs/2610.19211)

Establishes general sufficient conditions under which causal graphs remain identifiable from data with missing values (including MNAR), and provides a framework to transfer correctness guarantees from complete-data algorithms to the missing-data regime.  
*Why relevant:* Extends identifiability theory central to causal discovery—addresses a practical gap when applying structure learning to real-world incomplete datasets.

---

### 4. Graph Dirichlet Energy for Fitting-Free Bivariate Causal Inference
**Povilas Daniušis** | cs.LG | 2026-10-15  
[https://arxiv.org/abs/2610.21892](https://arxiv.org/abs/2610.21892)

Proposes a new score for bivariate cause-effect identification based on the Dirichlet energy of the outcome signal on a kernel similarity graph of the putative cause, requiring no model fitting. Achieves competitive accuracy on benchmark pairs.  
*Why relevant:* New kernel-based, fitting-free causal direction test—connects to kernel CI testing and nonparametric structure learning.

---

### 5. Benchmarking and Enhancing Agentic Causal Discovery
**Pingchuan Ma, Rui Ding, Shuai Wang** | cs.LG | 2026-10-16  
[https://arxiv.org/abs/2610.22846](https://arxiv.org/abs/2610.22846)

Introduces a benchmark specifically designed to evaluate whether LLM agents can go beyond running stock algorithms—catching algorithmic failures, issuing follow-up conditional independence tests, and correcting outputs—rather than just exploiting variable-name semantics.  
*Why relevant:* Addresses how agentic approaches can incorporate principled CI testing and iterative structure correction, relevant to automated causal discovery pipelines.

---

## Confounding, Proximal Methods & Identification

### 6. Proximal Causal Inference for Time Series from N-of-1 Mobile Device Data
**Fanyu Cui, Charlotte Fowler, Xiaoxuan Cai et al.** | stat.ME | 2026-10-15  
[https://arxiv.org/abs/2610.22647](https://arxiv.org/abs/2610.22647)

Extends the proximal causal inference (PCI) framework to intensive longitudinal (N-of-1) time series with time-varying hidden confounders, using negative control outcomes from mobile device data. Derives identification conditions and semiparametric estimators.  
*Why relevant:* PCI directly addresses latent confounding via proxy variables—extends to the time-series/dynamic setting relevant for root-cause analysis in sequential data.

---

### 7. Flexible Doubly Robust Proximal Causal Inference for Censored Outcomes
**Dhanajit Brahma, Ruolin Meng, Lawrence Carin, Ricardo Henao** | stat.ML | 2026-10-14  
[https://arxiv.org/abs/2610.20893](https://arxiv.org/abs/2610.20893)

Develops doubly robust proximal survival estimators (PSB) that relax the parametric bridge-function assumptions of prior proximal survival methods, using flexible nonparametric bridge estimation with formal semiparametric efficiency guarantees.  
*Why relevant:* Advances the proximal causal inference toolkit for settings with hidden confounding; the doubly-robust and nonparametric aspects connect to semiparametric theory central to the profile.

---

### 8. Sharp Instrumental Variable Bounds under the Marginal Sensitivity Model
**Antonio Olivas-Martinez, Eric Tchetgen Tchetgen** | stat.ME | 2026-10-15  
[https://arxiv.org/abs/2610.22513](https://arxiv.org/abs/2610.22513)

Combines partial identification via a marginal sensitivity model (bounding unmeasured confounding) with instrumental variable restrictions to sharpen inference on treatment effects, without requiring monotonicity or homogeneity.  
*Why relevant:* Identification under latent confounding; IV + sensitivity analysis is directly adjacent to JCI and soft-intervention target identification.

---

### 9. DeDiCa: A Scalable Deconfounding Discrete Causal Generative Model
**Kunchangtai Liang, Adrián Javaloy, Antonio Vergari, Isabel Valera** | cs.LG | 2026-10-16  
[https://arxiv.org/abs/2610.23272](https://arxiv.org/abs/2610.23272)

Introduces DeDiCa, a tractable causal Bayesian network framework for discrete variables with hidden confounders, using tensorized parameterization and exact marginalization over latents. Trained once on observational data and supports efficient interventional queries.  
*Why relevant:* Directly combines discrete causal structure with hidden confounding, and enables interventional inference—connects to JCI and identification under latent variables.

---

### 10. On Local Inference for Functionals of Ill-Posed Inverse Problems
**Ellen Graham, Andrea Rotnitzky** | math.ST | 2026-10-14  
[https://arxiv.org/abs/2610.19350](https://arxiv.org/abs/2610.19350)

Studies local (uniform) inference for linear functionals in ill-posed inverse problems, covering nonparametric IV, proximal causal inference, and shadow-variable models. Shows that standard pointwise root-n inference can fail locally and provides adaptive procedures.  
*Why relevant:* Core semiparametric theory for proximal causal inference and NP-IV—addresses a fundamental reliability gap in confidence intervals for latent-confounding methods.

---

## Treatment Effects & Experimental Design

### 11. Causal Mediation Analysis for Panel Data with Double/Debiased Machine Learning
**Peikai Wu, Zhiguo Xiao** | stat.ME | 2026-10-15  
[https://arxiv.org/abs/2610.21339](https://arxiv.org/abs/2610.21339)

Develops a DML framework for history-specific direct, indirect, and total effects in panel data with two-way fixed effects, using partially linear potential-outcome models and sequential identification under no-unmeasured-mediator-confounding assumptions.  
*Why relevant:* Mediation under panel/longitudinal data with high-dimensional nuisances; DML connects to nonparametric methods relevant to structure learning and causal effect estimation.

---

### 12. Difference-in-Differences for Heterogeneous Effects of General Treatment Strategies Accounting for Time-Varying Covariates
**Oliver Dukes, Zach Shahn, James Robins, Andrea Rotnitzky** | stat.ME | 2026-10-15  
[https://arxiv.org/abs/2610.22113](https://arxiv.org/abs/2610.22113)

Extends DiD to marginal structural nested mean models (mSNMMs) capturing time-varying effect modification, with identification under conditional parallel trends and robust semiparametric estimation.  
*Why relevant:* Time-varying treatment strategies and heterogeneous effect estimation; the mSNMM/Robins framework is closely related to interventional graph-based causal reasoning.

---

### 13. Learning Who Benefits Most: Multi-Treatment Causal Ranking for Population Health Stratification
**Rocco Zaccagnino, Martina Girolamo, Alberto Lombardi et al.** | cs.LG | 2026-10-14  
[https://arxiv.org/abs/2610.19782](https://arxiv.org/abs/2610.19782)

Formulates population health stratification as a multi-treatment CATE estimation problem, ranking which treatment benefits each patient subgroup most under resource constraints, using uplift modeling.  
*Why relevant:* Multi-treatment CATE estimation relates to heterogeneous intervention effects; connects to experimental design and optimal treatment allocation.

---

### 14. Minimax Rates for Pointwise CATE Estimation: The Role of Design Smoothness
**Yuxuan Hou, Zhenghan Li** | math.ST | 2026-10-13  
[https://arxiv.org/abs/2610.18623](https://arxiv.org/abs/2610.18623)

Derives matching upper and lower minimax risk bounds for pointwise CATE estimation, showing that the convergence rate depends critically on the smoothness of the design density (covariate distribution), not just the outcome regression smoothness.  
*Why relevant:* Sharp theoretical results for nonparametric CATE; the role of design conditions mirrors issues in nonparametric CI testing and neighborhood selection in high-dimensional settings.

---

### 15. Unit-Level Aggregation Breaks Coverage in Causal Foundation Models
**Gabe Schulman, Lucius E. J. Bynum, Yoav Wald** | stat.ML | 2026-10-16  
[https://arxiv.org/abs/2610.22770](https://arxiv.org/abs/2610.22770)

Shows that causal foundation models (CFMs) producing well-calibrated unit-level credible intervals lose valid coverage when these are aggregated to population-level ATEs or subgroup effects, due to interval non-exchangeability. Proposes a correction procedure.  
*Why relevant:* Exposes a fundamental reliability gap in modern neural causal estimators; directly relevant for anyone using CFMs to estimate interventional effects.

---

### 16. Calibrated Bayesian Inference for Overall and Subgroup-Specific Causal Effects in Stepped-Wedge Cluster-Randomized Trials
**Ruyi Liu, Yuki Ohnishi, Xi Fang et al.** | stat.ME | 2026-10-14  
[https://arxiv.org/abs/2610.20858](https://arxiv.org/abs/2610.20858)

Proposes a calibrated Bayesian approach for stepped-wedge CRTs that targets well-defined causal estimands (ATE, subgroup effects) rather than working model coefficients, providing valid uncertainty quantification under model misspecification.  
*Why relevant:* Causal estimands from randomized designs; connects to experimental design and transportability of causal estimates across subpopulations.

---

## CI Testing & Semiparametric Methodology

### 17. Testing Conditional Distribution Equality Using Generative Models
**Zekai Jin, Yi Zhang, Yun Yang, Xiaofeng Shao** | stat.ME | 2026-10-14  
[https://arxiv.org/abs/2610.20447](https://arxiv.org/abs/2610.20447)

Proposes a conditional distribution equality test that augments real data with generative model samples to boost power when the conditioning variable is high-dimensional. Provides a sample-splitting and studentization procedure with provable Type-I error control.  
*Why relevant:* High-dimensional conditional distribution testing is fundamental to CI testing (a core component of constraint-based causal discovery like FCI/PC).

---

### 18. A Bayesian Model Averaging Approach for Estimating Longitudinal Treatment Effects
**David Adenyo, Mireille E. Schnitzer, Jason R. Guertin, Denis Talbot** | stat.ME | 2026-10-16  
[https://arxiv.org/abs/2610.23578](https://arxiv.org/abs/2610.23578)

Adapts Bayesian model averaging to variable selection for longitudinal treatment effect estimation, combining propensity score and outcome regression model uncertainty to reduce covariate selection bias.  
*Why relevant:* Variable selection for causal effect estimation under longitudinal confounding; relevant to high-dimensional graphical model selection in observational studies.

---

## Graphical Models

### 19. Student Copula Markov Networks
**Salha Mamane, Cheikh Tidiane Seck** | stat.ML | 2026-10-13  
[https://arxiv.org/abs/2610.19135](https://arxiv.org/abs/2610.19135)

Characterizes the pairwise Markov property in undirected graphical models via copula densities, then derives a necessary condition for the pairwise Markov property in Student copula networks, enabling non-Gaussian graphical modeling via an ECM algorithm.  
*Why relevant:* Extends Markov property characterization to heavy-tailed (Student) copulas—directly relevant to high-dimensional graphical models and neighborhood selection under non-Gaussian distributions.

---

### 20. Maximum Likelihood Degrees via One-Edge Chordal Completion
**Nilava Metya** | math.AG | 2026-10-14  
[https://arxiv.org/abs/2610.19669](https://arxiv.org/abs/2610.19669)

Computes the maximum likelihood degrees of Gaussian graphical models for graphs that become chordal after adding a single missing edge, expressing the MLD in terms of clique and separator sizes in the chordal completion.  
*Why relevant:* Algebraic complexity of Gaussian graphical model inference—informs understanding of identifiability and estimation in structured Gaussian models.

---

*Generated automatically by the arXiv digest agent.*

---

## Past Digests

- [2026-W43](archive/2026-W43.md) — 2026-10-12 to 2026-10-19
- [2026-W40](archive/2026-W40.md) — 2026-09-21 to 2026-09-28
- [2026-W39](archive/2026-W39.md)
- [2026-W38](archive/2026-W38.md)
- [2026-W37](archive/2026-W37.md)
- [2026-W36](archive/2026-W36.md)
- [2026-W35](archive/2026-W35.md)
- [2026-W34](archive/2026-W34.md)
- [2026-W33](archive/2026-W33.md)
- [2026-W32](archive/2026-W32.md)
- [2026-W31](archive/2026-W31.md)
- [2026-W29](archive/2026-W29.md)
- [2026-W28](archive/2026-W28.md)
- [2026-W27](archive/2026-W27.md)
- [2026-W26](archive/2026-W26.md)
- [2026-W25](archive/2026-W25.md)
