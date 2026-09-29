---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest 2026-W40

**Covered period:** 2026-09-21 to 2026-09-28 UTC  
**Total scanned:** ~450 (cat:stat.ME, math.ST, stat.ML, cs.LG) | **Kept:** 12

---

## Causal Discovery & Structure Learning

### Statistical Inference for Causal Discovery under Selection and Latent Variables via Single-Target Interventions
**Xiaotian Hou, Kwangmoon Park, Hongzhe Li**  
[arXiv:2609.28856](https://arxiv.org/abs/2609.28856) | `stat.ME` — 2026-09-23

Addresses causal discovery when both latent confounders and selection bias are present, a setting where DAGs over observed variables are insufficient. The authors introduce *system-induced subgraphs* and establish identifiability via maximal ancestral graphs (MAGs) using single-target interventions on observed variables; they show such interventions are both sufficient and necessary, requiring at most 5/2d²_X tests for d_X observed variables — optimal up to a constant. The framework accommodates soft interventions, makes no parametric assumptions, and is validated on Perturb-seq lung-cancer data.

*Why relevant: Directly targets JCI-style interventional causal discovery under latent confounding; the MAG/PAG identifiability result and soft-intervention treatment are core to the research agenda on localized root cause analysis.*

---

### MARCEDES: Score-based Causal Discovery under Non-Gaussianity with Continuous Optimization
**Anamitra Chaudhuri, Anirban Bhattacharya, Yang Ni**  
[arXiv:2609.30643](https://arxiv.org/abs/2609.30643) | `stat.ML`, `cs.LG`, `stat.CO`, `stat.ME` — 2026-09-25

Proposes a continuous score-based method for learning DAGs from non-Gaussian structural equation models. The key contribution is a *mean absolute residual risk* score with row-specific sparsity penalties and a soft DAG constraint, enabling unconstrained gradient-based optimization. A generalized Bayes framework handles the non-smooth objective and penalty tuning; simulation studies confirm improved performance over existing approaches in finite-sample high-dimensional settings.

*Why relevant: Non-Gaussian SEM + continuous DAG optimization is a direct contribution to structure learning; the score function and sparsity formulation connect to the sparse-additive nonparametric setting in the research profile.*

---

### LUCID: Learning Under Confounding for Inference and Discovery in Time Series
**Mohammad Fesanghary**  
[arXiv:2609.31315](https://arxiv.org/abs/2609.31315) | `cs.LG`, `stat.ML` — 2026-09-25

Proposes LUCID, a method for causal discovery in time series data with unobserved common causes that induce spurious associations. The approach explicitly models latent confounders within a structural causal framework and recovers causal structure despite their presence. LUCID achieves an F1 score of 0.60 on synthetic benchmarks.

*Why relevant: Causal discovery under latent confounding in the time-series setting; aligns with identifying unknown intervention targets and latent variable challenges in the research profile.*

---

## Interventions & Experimental Design

### Optimal Sequential Decision-Making with Initiation Regimes
**Laurendeau, Sarvet, Stensrud**  
[arXiv:2609.29844](https://arxiv.org/abs/2609.29844) | `stat.ME` — 2026-09-25

Develops the theory of *initiation regimes* — dynamic treatment rules that also govern when treatment begins — and proves they strictly generalize superoptimal regimes identified from large experiments. The paper derives identification and optimality results for this broader class of sequential decision rules.

*Why relevant: Extends the theory of optimal dynamic treatment regimes (interventional causal inference) and has direct implications for experimental design with intervention timing.*

---

### Factorial Multivariate Bayesian Causal Forests
**Danilo A. Sarti**  
[arXiv:2609.31332](https://arxiv.org/abs/2609.31332) | `stat.ME`, `stat.AP`, `stat.CO` — 2026-09-25

Introduces a Bayesian nonparametric model for heterogeneous treatment effects when units receive several binary treatments and outcomes are correlated. Factorial Multivariate Bayesian Causal Forests (F-MBCF) uses a tree ensemble that jointly captures treatment–outcome interactions and within-outcome dependence, providing posterior uncertainty quantification for factorial causal contrasts.

*Why relevant: Multi-treatment causal inference with nonparametric methods; the factorial / joint intervention framing is closely related to Joint Causal Inference and experimental settings with multiple simultaneous interventions.*

---

### An End-to-End Pipeline for Causal ML with Continuous Treatments
**Moral Hernández, Higuera-Cabañes, Ibraín**  
[arXiv:2609.30396](https://arxiv.org/abs/2609.30396) | `stat.ME`, `cs.LG`, `stat.AP`, `stat.ML` — 2026-09-25

Presents a practical end-to-end causal machine learning pipeline for settings with continuous treatment variables. Contributions include a modular architecture for high-dimensional confounding adjustment, dose-response function estimation, and sensitivity analysis, validated on real-world datasets.

*Why relevant: Practical causal ML for continuous interventions; addresses high-dimensional confounding in line with the sparse/nonparametric methods strand of the research profile.*

---

### Sample-Efficient Multiple Testing with Adaptive Data Collection
**Zhanran Lin, Wanteng Ma, Zhimei Ren**  
[arXiv:2609.26651](https://arxiv.org/abs/2609.26651) | `stat.ME` — 2026-09-22

Studies how to allocate sampling effort across hypotheses in an adaptive experiment while maintaining FDR control. The method uses e-value-based posterior sampling under the e-BH procedure, adapting data collection to the evidence accumulated so far. Proven to be more sample-efficient than non-adaptive designs while preserving finite-sample FDR guarantees.

*Why relevant: Adaptive experimental design with FDR control; directly addresses the intersection of interventional causal discovery and optimal experimental design that is central to the research profile.*

---

## Mediation Analysis & Counterfactuals

### Formulating Cross-World Mediation Estimands Through Single-World Mixtures
**Razieh Nabi, David Benkeser**  
[arXiv:2609.27075](https://arxiv.org/abs/2609.27075) | `stat.ME` — 2026-09-22

Natural direct and indirect effects are traditionally defined via nested counterfactuals crossing potential worlds. This paper shows that under *susceptibility marker* assumptions, these cross-world estimands can be expressed as mixtures of controlled (single-world) direct effects, yielding identification from observed data without cross-world independence. Provides a path toward more credible nonparametric identification of mediation estimands.

*Why relevant: Counterfactual identification under latent confounding for mediation analysis; the single-world mixture representation is a new identifiability result connecting nested counterfactuals to estimable quantities, directly relevant to causal reasoning with latent variables.*

---

## Graphical Models & Conditional Independence Testing

### High-Dimensional Gaussian Graphical Model Testing for Long-Memory Time Series
**Zhai, Zhong, Wu**  
[arXiv:2609.30565](https://arxiv.org/abs/2609.30565) | `stat.ME`, `math.ST`, `stat.ML` — 2026-09-25

Develops a data-adaptive conditional independence test for high-dimensional Gaussian graphical models (GGMs) when observations exhibit long-range dependence. The test accounts for the inflated covariance of sample correlations under long memory, providing valid inference for GGM edge selection where standard independence tests fail. Asymptotic theory and simulations on both synthetic and financial time-series data are provided.

*Why relevant: Conditional independence testing for graphical model structure under non-i.i.d. (long-memory) observations; directly extends the CI testing methodology in the research profile to dependent settings.*

---

## Causal Perspectives on Distribution Shift & Epidemiology

### Concept Drift from a Causal Perspective
**Eduardo V. L. Barboza, Jean Paul Barddal, Robert Sabourin**  
[arXiv:2609.25340](https://arxiv.org/abs/2609.25340) | `cs.LG`, `stat.ME` — 2026-09-21

Proposes a Structural Causal Model taxonomy for concept drift, categorising shifts by causal origin: changes in exogenous noise, changes in mechanism functions, or changes in the causal graph topology itself. This causal decomposition separates types of drift that are conflated in distribution-centric accounts and suggests targeted adaptation strategies for each drift type.

*Why relevant: SCM-based framework for distribution shift connects to transportability and invariant prediction; the mechanism-level decomposition is directly relevant to understanding when causal models transfer across environments.*

---

### Design-Ignoring versus Design-Respecting World Models for Epidemiology
**Xiangyu Yu, Weiyu Liu**  
[arXiv:2609.30679](https://arxiv.org/abs/2609.30679) | `stat.ME`, `stat.AP`, `stat.ML` — 2026-09-25

Systematically compares world models that encode the study design (assignment mechanism, sampling, measurement) against those that ignore it, showing how design-ignoring models can embed spurious associations or fail to identify the target estimand. Formalises when design-respecting models are necessary for causal identification and proposes practical guidelines for epidemiological settings.

*Why relevant: Formalises how study design enters causal identification — directly relevant to the observational-vs-interventional data distinction and transportability in causal discovery.*

---

### A Unified Framework for Estimating Direct Causal Effects under Spatial Confounding and Interference
**Isqeel Ogunsola, Olatunji Johnson**  
[arXiv:2609.28799](https://arxiv.org/abs/2609.28799) | `stat.ME` — 2026-09-23

Addresses the joint presence of spatial confounding (unmeasured spatial factors) and spatial interference (unit interactions through proximity) in observational causal estimation. Proposes a unified estimator for direct causal effects with the R package `spaci`, accommodating both biases simultaneously rather than treating them independently as prior work does.

*Why relevant: Estimation under spatial latent confounding and interference is an instance of the general problem of identifying causal effects with unobserved confounders; the unified treatment connects to the latent-variable identification challenges in the research profile.*
### Epidemiological Causal Graph Identification: Challenges, Identifiability and Algorithms
**Sambit Mishra, Yingying Wang, Christine K. Johnson, Urbashi Mitra**  
[arXiv:2609.20676](https://arxiv.org/abs/2609.20676) | `cs.LG` `stat.ME`

Proves that the causal edge direction between an ordinal node (ordered logit) and an exponential-family node in a DAG is distributionally identifiable at generic parameter values, and extends prior Ordinal–Poisson results to the full exponential family. A score-based exhaustive search and a DAGMA-based masked optimisation are introduced for structure recovery and validated on mixed-variable DAGs.

*Why relevant: Directly addresses identifiability of DAG edge orientations beyond classical Gaussian/additive-noise SEMs, extending Markov-equivalence-class constraints to mixed-distribution settings relevant to real epidemiological data.*

---

### Causal Discovery via Transformed Low-Rank Quantile Surfaces
**Ryo Kamimura, Thong Pham**  
[arXiv:2609.16931](https://arxiv.org/abs/2609.16931) | `stat.ME`

Introduces Low-Rank Quantile Surfaces (LRQS), a bivariate causal model where a monotone transformation of the conditional quantile surface is low-rank in the causal direction; the paper proves generic identifiability and shows that reverse representability under the same constraints holds only for fine-tuned marginals. A nonparametric fitting procedure alternating between rank-constrained quantile-surface approximation and isotonic estimation of the transformation gives a practical causal score.

*Why relevant: New bivariate causal discovery method with provable identifiability that subsumes location-scale models and post-nonlinear heteroscedastic noise models — broadens the class of identifiable SCMs beyond existing functional-causal-model assumptions.*

---

### Statistical Inference for Bivariate Functional Causal Discovery
**Shreya Prakash, Fan Xia, Elena A. Erosheva**  
[arXiv:2609.16562](https://arxiv.org/abs/2609.16562) | `stat.ME`

Reviews statistical guarantees of existing functional causal discovery methods and identifies a key gap: the absence of a unified inferential framework across model classes. Proposes a test-based approach repurposing goodness-of-fit and independence tests within a hypothesis-testing framework, yielding four causal discovery outcomes with explicit uncertainty quantification; resampling is used to estimate causal outcome rates.

*Why relevant: Fills a long-standing gap by providing valid statistical inference (p-values, rates) for functional causal discovery — directly relevant to anyone who wants to quantify uncertainty in bivariate causal direction tests.*

---

### Provable Guarantees and Efficient Learning of Structural Equation Models with Latent Confounders
**Weijian Yu, Jean Honorio**  
[arXiv:2609.18535](https://arxiv.org/abs/2609.18535) | `cs.LG` `stat.ML`

Proposes an iterative algorithm for linear SEMs with latent confounders that recovers the observed-variable DAG by identifying terminal nodes and decomposing the precision matrix as sparse (conditional dependencies) plus low-rank (latent confounder influence). Establishes that for *p* observed variables, *r* latent confounders, and *s* edges, correct causal structure recovery is achieved from *n* ≳ max{*s* log *p*, *rp*} samples.

*Why relevant: Directly addresses the challenge of causal discovery under latent (unmeasured) confounding with sample-complexity guarantees — central to the JCI / unknown-intervention-target setting where hidden common causes are present.*

---

## Identifiability of Causal Models

### On the Identifiability of Mixed Ordinal and Exponential Family Causal DAGs under Linear Parametric Models
**Sambit Mishra, Urbashi Mitra**  
[arXiv:2609.17942](https://arxiv.org/abs/2609.17942) | `cs.LG` `math.ST`

Proves that every edge between an ordinal node (≥3 categories) and an exponential-family node (≥3 support points) in a linear parametric model is identifiable from the joint distribution alone, regardless of sufficient-statistic form, and gives necessary-and-sufficient converses showing both requirements are binding. Results extend edge-orientation beyond what conditional independence can resolve within a Markov equivalence class.

*Why relevant: Shows that mixed-variable DAGs gain extra identifiability power beyond FCI-style CI-based procedures — important for orienting edges in equivalence classes containing ordinal variables.*

---

### One Intervention per Component is Enough: Towards Identifiability in Linear Stochastic Dynamics from Steady State
**Saber Salehkaleybar**  
[arXiv:2609.19955](https://arxiv.org/abs/2609.19955) | `cs.LG`

Proves that one soft intervention per strongly connected component (SCC) of a multivariate Ornstein-Uhlenbeck drift graph suffices to generically identify all OU-process parameters from steady-state (non-time-series) observational and interventional data, provided the SCC condensation is connected with a single root. A topological recursive algorithm and a regularised least-squares estimator are proposed for the finite-sample case.

*Why relevant: Provides a minimal interventional data requirement for causal parameter identification in linear stochastic dynamics — directly relevant to interventional experimental design and identifiability under unknown soft interventions.*

---

### Kinks vs. Smoothness: Identifiability of Real Analytic nICA for Laplace-like Sources
**Isaac Manring, Kejun Huang**  
[arXiv:2609.21926](https://arxiv.org/abs/2609.21926) | `cs.LG`

Proves exact identifiability (up to permutation and scaling) of nonlinear ICA when source PDFs have finitely many kinks (non-differentiable points) and the mixing function is real analytic — with the Laplace distribution as the canonical example. The proof exploits the contrast between source kinks and the global smoothness of analytic functions, and is compatible with normalising flow or VAE training pipelines using standard activations.

*Why relevant: LiNGAM-family causal discovery exploits non-Gaussianity for DAG identifiability; this nICA result extends the identifiability toolkit to nonlinear mixings under Laplace-like sources, informing the theoretical reach of non-Gaussian causal methods beyond the linear regime.*

---

## Conditional Independence Testing & Kernel Methods

### Conditional Independence Testing in Time Series
**Jieru Shi, Rajen D. Shah**  
[arXiv:2609.20772](https://arxiv.org/abs/2609.20772) | `stat.ME` `math.ST`

Extends the Generalised Covariance Measure (GCM) to time series by proposing the Generalised Temporal Covariance Measure (GTCM): nonlinearly regress both outcome and exposure on their shared history, then test whether the cross-covariance of residuals is zero. Variance-weighted and polynomial-lag data-adaptive variants control type I error under the assumption that regression procedures estimate conditional means at a sufficiently fast rate, without requiring time-series splitting.

*Why relevant: Directly extends the GCM — a core tool in the user's research profile — to the time-series setting for Granger-causality testing, with explicit handling of non-stationarity and weak dependence.*

---

### RKHS-Based Inference for Nonlinear Granger Causality via Conditional Centering
**Yuhan Tian, Adam Waterbury, Marie-Christine Düker**  
[arXiv:2609.22007](https://arxiv.org/abs/2609.22007) | `stat.ME`

Proposes an RKHS test for nonlinear Granger non-causality by decomposing the target regression into an own-history component (estimated by kernel ridge regression) and an orthogonal component capturing the additional predictive contribution of the source history. The squared RKHS norm of the conditionally-centred residual embedding forms the test statistic; a weighted chi-square null limit is established and critical values are calibrated spectrally without resampling.

*Why relevant: Introduces a kernel CI test for Granger causality with formal null distribution theory — combining RKHS/kernel testing machinery (HSIC-adjacent) with non-linear time-series CI testing, both central to the user's profile.*

---

## Graphical Models & Network Structure

### Matrix Graphical Model Via Joint Estimation of Partial Correlations
**Hyewon Kim, Seongoh Park**  
[arXiv:2609.19718](https://arxiv.org/abs/2609.19718) | `stat.ME`

Proposes a joint estimation framework for matrix graphical models under a Kronecker-product separable covariance assumption, simultaneously estimating all row- and column-domain partial correlations within a unified penalised optimisation. Unlike existing multi-regression approaches, the method preserves graph symmetry and eases tuning-parameter selection; experiments and a protein-expression application demonstrate improved edge-recovery.

*Why relevant: High-dimensional graphical model estimation with Kronecker structure is an important special case of the broader conditional-independence / neighbourhood-selection problem; the joint partial-correlation formulation is directly relevant to structure learning.*

---

### Noise-Adjusted Turnover in Estimated Networks
**Sultan Amed, Sayantan Banerjee**  
[arXiv:2609.20044](https://arxiv.org/abs/2609.20044) | `stat.ME`

Studies how to correct observed Hamming-turnover between two estimated graphs for graph-selection error under a homogeneous edge-misclassification model with known sensitivity and specificity, deriving a closed-form unbiased adjustment. Characterises how sparsity, calibration error, and cross-period dependence affect bias after adjustment, showing that a false-positive probability of order p⁻¹ can still generate order-p spurious turnover.

*Why relevant: Addresses the effect of conditional-independence test errors on inferred graph structure changes — relevant to anyone studying how CI-testing noise propagates into structure-learning conclusions across settings or time periods.*

---

## Interventions, Transportability & Estimation

### Efficient Transport and Generalization of Survival Treatment Effects
**Axel Martin, Iván Díaz, Michele Santacatterina**  
[arXiv:2609.18764](https://arxiv.org/abs/2609.18764) | `stat.ME`

Derives efficient influence functions for transporting and generalising causal survival-function differences from a source to a target population in discrete time under standard transportability assumptions. Proposes cross-fitted one-step doubly-robust estimators achieving semiparametric efficiency; introduces estimators that exploit known effect-modifier subsets to reduce reweighting dimensionality and asymptotic variance.

*Why relevant: Extends transportability / external validity methods — a topic adjacent to invariant prediction and distribution shift — to survival outcomes with formal efficiency theory and DML-style estimators.*

---

### Causal Path Analysis from Perturbational and Population-Scale Single-Cell Data with Multiscale Confounding and Measurement Error
**Kwangmoon Park, Hongzhe Li**  
[arXiv:2609.16510](https://arxiv.org/abs/2609.16510) | `stat.ME` `stat.ML`

Develops a framework integrating gene-perturbation (interventional) data with population-scale observational single-cell data for causal path analysis: ancestral relationships from perturbation data constrain network topology, while direct effects are re-estimated from population data. A surrogate-variable procedure corrects for latent heterogeneity and measurement error at both cell and subject levels, with theoretical guarantees for confounder recovery and high-dimensional effect estimation.

*Why relevant: Combines interventional and observational data under latent confounding — a central scenario in JCI / unknown soft-intervention-target causal discovery — with application to gene regulatory networks.*

---

### Covariate Selection for Doubly Robust Double/Debiased Machine Learning Estimators for Causal Inference
**Muwon Kwon, Peter M. Steiner**  
[arXiv:2609.17238](https://arxiv.org/abs/2609.17238) | `stat.ME` `stat.ML`

Shows that differential covariate selection in the propensity-score and outcome models can undermine double robustness in DML estimators, and proposes using the union of the covariate sets selected by both ML models to jointly re-estimate them. Simulation studies demonstrate that union-based selection consistently reduces confounding bias compared to separate selected sets, and that post-Lasso outperforms standard Lasso for bias reduction.

*Why relevant: Addresses the Markov-boundary / covariate-selection problem for causal effect estimation in high dimensions — the union strategy is closely related to propensity-score and outcome Markov-boundary ideas central to doubly-robust identification.*

---

### Splitting the Difference: Interpretable Causal Forests for Treatment Effect Heterogeneity and Bias
**Nicolas Alexander Ihlo, Merle Behr**  
[arXiv:2609.16971](https://arxiv.org/abs/2609.16971) | `stat.ML` `cs.LG`

Introduces a random forest algorithm for individual treatment effect estimation using a splitting criterion that combines a heterogeneity component with a bias-correction component, automatically distinguishing confounders from effect-modifiers without separate orthogonalisation. Interpretability follows directly from the tree structure without post-hoc analysis, and the method handles observational studies with varying propensity without estimating the full propensity function.

*Why relevant: Directly addresses the confounder vs. effect-modifier distinction — a graphical-model question — in ITE estimation, providing a structure-learning perspective on treatment-effect heterogeneity.*

---

## Causal Identification & Sensitivity Analysis

### Identification and Estimation of Causal Estimands with Missing Not at Random Data
**Faria Rauf Ria, Tarikul Islam, Mahbub A. H. M. Latif**  
[arXiv:2609.20113](https://arxiv.org/abs/2609.20113) | `stat.ME`

Derives identification results for average treatment effects and natural direct/indirect effects (mediation) under several MNAR missingness mechanisms using completeness conditions, and proposes EM-based estimators. Simulation comparisons show substantially lower bias than complete-case analysis and multiple imputation under the considered MNAR mechanisms.

*Why relevant: Extends causal identification — including mediation analysis — to settings with partially observed confounders and outcomes under MNAR, a practical obstacle in causal inference with real-world data.*

---

### Doubly Valid and Doubly Sharp Sensitivity Analysis to Unobserved Confounding for Survival Outcomes
**Jean-Baptiste Baitairian, Bernard Sebastien, Rana Jreich, Sandrine Katsahian, Agathe Guilloux**  
[arXiv:2609.18713](https://arxiv.org/abs/2609.18713) | `stat.ME`

Develops DVDS (doubly valid, doubly sharp) bounds for survival-function differences and RMST under the Marginal Sensitivity Model, extending recent non-survival DVDS results to time-to-event outcomes with informative censoring. The method yields tighter bounds and better computational efficiency than prior approaches.

*Why relevant: Sensitivity analysis to unobserved confounding is complementary to identification under latent confounders — provides sharp interval estimates when unmeasured confounders cannot be ruled out in survival analyses.*

---

### Efficient Estimation and the Cost of Complete-Case Coarsening under Monotone Sequential MAR
**Keivan Bolouri**  
[arXiv:2609.17778](https://arxiv.org/abs/2609.17778) | `stat.ME`

Quantifies the semiparametric efficiency loss from discarding partially-observed confounder values (complete-case coarsening) under monotone sequential missing-at-random with two ordered confounders; derives the canonical gradient and an exact drift identity for a cross-fitted sequential multiply-robust estimator. When second-stage response depends on the intermediate confounder, coarsening introduces identification failure, not just efficiency loss.

*Why relevant: Studies confounding-adjustment efficiency under missing data — the interplay between confounder observability and causal identification is directly relevant to partially-observed graph settings.*

---

## Previous Digests

- [2026-W38](archive/2026-W38.md) — September 7 – 14, 2026
- [2026-W37](archive/2026-W37.md) — August 31 – September 7, 2026
- [2026-W36](archive/2026-W36.md) — August 24–31, 2026
- [2026-W35](archive/2026-W35.md) — August 17–24, 2026
- [2026-W34](archive/2026-W34.md) — August 10–17, 2026
- [2026-W33](archive/2026-W33.md) — August 3–10, 2026
- [2026-W32](archive/2026-W32.md) — July 27 – August 3, 2026
- [2026-W31](archive/2026-W31.md) — July 20–27, 2026
- [2026-W29](archive/2026-W29.md) — July 13–20, 2026
- [2026-W28](archive/2026-W28.md) — June 29 – July 6, 2026
- [2026-W27](archive/2026-W27.md) — June 22–29, 2026
- [2026-W26](archive/2026-W26.md) — June 15–22, 2026
- [2026-W25](archive/2026-W25.md) — June 8–15, 2026
