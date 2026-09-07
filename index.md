---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest 2026-W37

**Covered period:** 2026-08-31 to 2026-09-07 UTC  
**Total scanned:** 656 | **Kept:** 20

---

## Causal Discovery & Structure Learning

### Beyond Stationarity in Time Series: Discovering Causal Structures and Latent Regimes via Markov Blankets
**Lei Zan, Charles K. Assaad, Emilie Devijver, Eric Gaussier**  
[arXiv:2609.05150](https://arxiv.org/abs/2609.05150) | `cs.LG`, `cs.AI`

Introduces RCBNB-MB, a constraint-and-noise-based causal discovery algorithm for time series that simultaneously identifies latent *regimes* (contiguous intervals with a stable causal structure) and the within-regime causal graphs, using Markov blanket selection to keep the search tractable.

*Why relevant: Directly combines Markov boundary selection with causal discovery under regime changes — touches non-stationary causal structure learning, a natural extension of constraint-based methods.*

---

### Federated Causal Discovery via Regression-Directed Cumulants
**Pablo Torrijos, Fabio Stella, José A. Gámez, José M. Puerta**  
[arXiv:2609.03705](https://arxiv.org/abs/2609.03705) | `cs.LG`

Adapts DirectLiNGAM to federated settings by showing that the higher-order cumulant tensors required for direction identification can be aggregated across clients without sharing raw data, enabling causal discovery beyond Markov equivalence under GDPR-style constraints.

*Why relevant: LiNGAM / additive-noise-model causal discovery; goes beyond Markov equivalence classes in a privacy-preserving way — intersects structure learning and non-Gaussian methods.*

---

### Guide, Not Bind: Why Defeasible Priors Fail in Augmented Lagrangian Causal Discovery
**Sairam Sundararaman, Sara Girdhar, Manit Narasimha Murthy, Samrudh N.**  
[arXiv:2609.03442](https://arxiv.org/abs/2609.03442) | `cs.LG`

Diagnoses two fundamental failure modes of differentiable causal discovery (e.g. NOTEARS-style) when expert-knowledge forbidden-edge priors are encoded via Augmented Lagrangian penalties: sequential penalty ramping suppresses true edges before they can be checked, and the counterfactual correction remains incomplete even after repair.

*Why relevant: Core differentiable structure learning; the paper's formal analysis directly concerns DAG-constrained optimisation and the interplay between data evidence and expert priors in causal graph estimation.*

---

### Genetic Algorithms for Tractable Bayesian Network Fusion via Pre-Fusion Edge Pruning
**Pablo Torrijos, José A. Gámez, José M. Puerta, Juan A. Aledo**  
[arXiv:2609.03724](https://arxiv.org/abs/2609.03724) | `cs.NE`, `cs.LG`

Proposes a GA-based framework for merging multiple Bayesian networks into a single tractable structure; a pre-fusion edge-pruning step prioritises edges shared across input BNs, controlling treewidth while preserving statistically agreed-upon dependencies.

*Why relevant: Bayesian network structure learning and fusion; relevant to combining multiple causal/graphical model sources while maintaining a parsimonious DAG.*

---

### Replicating TRACE: A Practitioner's Guide to Its Threshold and Particle Budget
**Alex Chadyuk, Alicia Zhang, Roy Kucukates**  
[arXiv:2609.01108](https://arxiv.org/abs/2609.01108) | `cs.LG`

Independent replication of TRACE, a method that reads causal event-type graphs out of a pretrained autoregressive language model by thresholding per-position conditional mutual information. The replication confirms headline F1 numbers but shows the optimal threshold is pinned to the truth margin rather than a universal constant.

*Why relevant: Causal graph extraction / CI-testing from learned models; uses CMI thresholding, linking to CI-test-based structure learning methodology.*

---

## Interventions, Identifiability & Experimental Design

### Symmetries and Causality: Causal Effect Identification Beyond IID Data
**Martin Rabel, Jakob Runge**  
[arXiv:2609.03697](https://arxiv.org/abs/2609.03697) | `math.ST`, `cs.AI`

Develops a formal language for causal reasoning grounded in symmetries that leave causal mechanisms invariant, enabling identifiability analysis in settings beyond IID (time series, spatial data, dynamical systems) without bespoke causal models per case.

*Why relevant: Causal identification theory beyond IID; formal symmetry-based extension connects to FCI/PAG-style reasoning under non-standard data-generating regimes.*

---

### Resolution-Aware Experimental Design under Partial Identifiability
**Sofianos Panagiotis Fotias**  
[arXiv:2609.03686](https://arxiv.org/abs/2609.03686) | `cs.LG`

Introduces RAED, which selects experiments by minimising the expected *structural candidate set* size under a false-exclusion constraint rather than maximising information gain. Proves an exact aliasing-separation theorem showing structural and latent-information objectives can diverge under partial identifiability.

*Why relevant: Optimal experimental design for causal structure learning under partial identifiability — directly relevant to active learning for causal discovery with latent variables.*

---

### Off-Policy Causal Estimation in Networks
**Sahil Loomba, Dean Eckles**  
[arXiv:2609.02756](https://arxiv.org/abs/2609.02756) | `stat.ME`, `econ.EM`

Studies off-policy estimation of causal effects under network interference, representing exposure-weighted potential outcomes in a biased-coin design and deriving estimators for heterogeneous Bernoulli policies with associated variance bounds.

*Why relevant: Causal estimation under interference / non-standard interventional distributions; connects to transportability and policy-shift identification in networked settings.*

---

### COSTA: Covariance-Optimized Design and Causal Inference under Network-Temporal Interference
**Qianyi Chen, Bo Li, Yongli Qin, Jinyong Ma**  
[arXiv:2609.02032](https://arxiv.org/abs/2609.02032) | `stat.ME`

Proposes COSTA, a joint Bernoulli spatiotemporal treatment-assignment design for network experiments with both spillovers and carryover. The Horvitz–Thompson bias equals the negative expected weight of an assignment cut; a covariance-level MSE bound is directly optimised.

*Why relevant: Experimental design under network/temporal interference — addresses identifiability of interventional effects in complex observational/experimental structures.*

---

### Causal Foundation Models
**Christopher Stith, Hossein Rahmani, Jesse C. Cresswell**  
[arXiv:2609.03003](https://arxiv.org/abs/2609.03003) | `cs.LG`, `stat.ML`

Introduces the *causal foundation model* (CFM) paradigm: a neural network pretrained once at scale on diverse causal problems that estimates treatment effects, identifies causal quantities, and performs policy evaluation without per-task bespoke pipelines or fine-tuning.

*Why relevant: A new architecture for causal inference estimation; bridges meta-learning with classical causal identification, potentially impacting how causal discovery and estimation are unified.*

---

## Conditional Independence Testing & Methodology

### Embedded Conditional Independence Tests for Large Language Model Generated Text
**Marco Simnacher, Georg Keilbar, Benjamin König, Christoph Lippert**  
[arXiv:2609.00946](https://arxiv.org/abs/2609.00946) | `stat.ML`, `cs.AI`, `cs.LG`, `math.ST`

Proposes eCITs (embedded conditional independence tests) that embed high-dimensional / multimodal objects (text, embeddings) before applying a standard CI test, enabling tests of whether an LLM's output carries attribute-related information beyond its source text, with theoretical guarantees. Applied to detecting political bias in German parliamentary speeches.

*Why relevant: Core CI testing methodology for high-dimensional and non-Euclidean objects — directly relevant to kernel/distance-covariance CI tests in causal discovery pipelines.*

---

### Exploring Sparse Autoencoders in Text-Based Causal Confounding Adjustment
**Mian Zhong, Katherine A. Keith, Anjalie Field**  
[arXiv:2609.01322](https://arxiv.org/abs/2609.01322) | `cs.CL`, `cs.LG`

Uses sparse autoencoders to extract a minimal, interpretable set of text features for confounding adjustment, iteratively selecting SAE features via conditional independence checks to balance richness (covering all confounders) against sparsity (finite-sample overlap).

*Why relevant: CI-test-guided covariate selection for high-dimensional text confounding — applies CI testing as a principled model-selection criterion in the adjustment pipeline.*

---

### Confounding-Valid Conformal Inference for Counterfactual KPIs in Wireless Networks
**Abdessamed Qchohi, Jessica Moysen Cortes, Matteo Zecchin**  
[arXiv:2609.05073](https://arxiv.org/abs/2609.05073) | `cs.LG`, `cs.NI`, `eess.SP`, `stat.ML`

Extends conformal counterfactual inference to settings with hidden confounding from omitted logged variables, using randomized nudges to recover valid coverage guarantees for counterfactual KPI prediction sets under latent confounders.

*Why relevant: Counterfactual inference under latent confounding with finite-sample validity guarantees — directly touches identifiability under hidden confounders and propensity-based correction.*

---

## Treatment Effects & Observational Studies

### Treatment Persistence Drives Estimator Performance in Longitudinal Causal Inference
**Sergio Gaiotti, Sara Poletto, Enrico Longato, Erica Tavazzi**  
[arXiv:2609.04940](https://arxiv.org/abs/2609.04940) | `stat.ME`

Simulation study using an SCM with time-varying confounding comparing longitudinal estimators (TMLE, G-formula, IPW, etc.) across nine scenarios. Finds that treatment persistence — correlation between consecutive treatment decisions — is the primary driver of performance gaps between baseline and longitudinal estimators.

*Why relevant: SCM-grounded evaluation of longitudinal causal estimators under time-varying confounding — of direct relevance to structure learning with time-varying interventions.*

---

### Causal Inference for Heterogeneous Extreme Quantiles with Heavy-Tailed Outcomes
**Xiaorui Wang, Juan-Juan Cai, Huixia Judy Wang, Jian Qing Shi**  
[arXiv:2609.03933](https://arxiv.org/abs/2609.03933) | `stat.ME`

Proposes a framework for conditional extreme quantile treatment effects (CEQTEs) in observational studies with heavy-tailed outcomes: IPW quantile regression estimates intermediate quantiles which are extrapolated via extreme value theory, exploiting that conditional and marginal potential outcome distributions share a common extreme value index.

*Why relevant: Nonparametric/semiparametric causal effect estimation under confounding with propensity score-based adjustment — extends IPW methodology to the heavy-tailed regime.*

---

### A Location-Invariant Estimator of Extremal Quantile Treatment Effects for Heavy-Tailed Distributions
**Xin Yu, Shuwei Huang, Jicheng Liu, Jielin Tang**  
[arXiv:2609.04018](https://arxiv.org/abs/2609.04018) | `cs.LG`, `stat.AP`, `stat.ME`

Addresses a location-invariance gap in existing extremal QTE estimators and proposes a corrected causal extreme value index estimator and paired extrapolation procedure that respects the invariance of the population QTE to common location shifts.

*Why relevant: Causal treatment effect estimation with propensity scores at extreme quantile levels — methodological extension of IPW-based estimation under heavy tails.*

---

## Graphical Models

### A Computational Approach to Maximum Likelihood Thresholds for Colored Gaussian Graphical Models
**Roser Homs, Olga Kuznetsova, Bernadette J. Stolz**  
[arXiv:2609.02382](https://arxiv.org/abs/2609.02382) | `stat.ML`, `cs.LG`, `math.AG`, `math.ST`

Studies the *maximum likelihood threshold* — the minimum sample size for the MLE to exist almost surely — for colored GGMs, which impose symmetry constraints via graph coloring to reduce effective dimension. Develops algebraic-geometry-based algorithms to compute MLTs for CGGMs.

*Why relevant: Fundamental structure-learning question in Gaussian graphical models: when does identifiable estimation become possible? Extends classical GGM theory to structured/symmetric models.*

---

### Deterministic LOCO Cross-Validation for Multilevel Bayesian Structural Equation Models
**Mohammad Alhyari, Haziq Jamil, Hans Montcho, Håvard Rue**  
[arXiv:2609.00670](https://arxiv.org/abs/2609.00670) | `stat.ME`

Derives a closed-form leave-one-cluster-out cross-validation procedure for multilevel Gaussian Bayesian SEMs via INLA, exploiting conditional independence of clusters given parameters to express the cluster-deleted posterior analytically and enable tractable SEM model selection.

*Why relevant: SEMs with Markov-type conditional independence structure; the CI-based factorisation is central to the derivation, linking SEM model selection to graphical model methodology.*

---

## Other Relevant

### Portable Causal Fairness Across Synthetic Data Generator Families
**Steven Golob, Sikha Pentyala, Martine De Cock**  
[arXiv:2609.03180](https://arxiv.org/abs/2609.03180) | `cs.LG`

Tests whether DECAF-style causal fairness constraints (defined as edge cuts on the generator's causal graph) transfer across nine generators from three unrelated families. Finds the fairness constraints hold across families, confirming they arise from causal factorisation rather than GAN-specific artefacts.

*Why relevant: Applies causal graph structure (edge removal = soft intervention) to synthetic data generation — relevant to interventional causal discovery and data-driven causal fairness.*

---

### Spurious Quantum Correlations
**Shashaank Khanna, Matthew F. Pusey, Roger Colbeck**  
[arXiv:2609.04157](https://arxiv.org/abs/2609.04157) | `quant-ph`, `math.ST`, `physics.class-ph`

Extends Bell's theorem to show that any classical causal structure that recovers all quantum correlations must permit *spurious* correlations — classically impossible correlations arising purely from the causal structure, not physical signals.

*Why relevant: Uses causal structures and ancestral graphs in a fundamental way; results about achievable correlations under causal structures are directly relevant to graphical model identifiability theory.*

---

## Previous Digests

- [2026-W35](archive/2026-W35.md) — August 24 – 31, 2026
- [2026-W34](archive/2026-W34.md) — August 10 – 17, 2026
- [2026-W33](archive/2026-W33.md) — August 3 – 10, 2026
- [2026-W32](archive/2026-W32.md) — July 27 – August 3, 2026
- [2026-W31](archive/2026-W31.md) — July 20 – 27, 2026
- [2026-W29](archive/2026-W29.md) — July 13 – 20, 2026
- [2026-W28](archive/2026-W28.md) — June 29 – July 6, 2026
- [2026-W27](archive/2026-W27.md) — June 22 – 29, 2026
- [2026-W26](archive/2026-W26.md) — June 15 – 22, 2026
- [2026-W25](archive/2026-W25.md) — June 8 – 15, 2026
