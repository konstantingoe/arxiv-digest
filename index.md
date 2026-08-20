---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest 2026-W34

**Week of August 10 -- 17, 2026**

Categories scanned: `stat.ME`, `math.ST`, `stat.ML`, `cs.LG`
Papers scanned: 821 | Papers selected: 20
# arXiv Digest 2026-W33

**Week of August 3 -- August 10, 2026**

Categories scanned: `stat.ME`, `math.ST`, `stat.ML`, `cs.LG`
Papers scanned: 673 | Papers selected: 11

---

## Causal Discovery & CI Testing

### Conditional Independence Tests for Constraint-Based Causal Discovery: A Survey
**Pavel Averin, Theodoros Moysiadis, Ioannis Katakis**
[arXiv:2608.11156](https://arxiv.org/abs/2608.11156v1) | `stat.ML`, `cs.LG`

A comprehensive survey of conditional independence (CI) testing as the statistical backbone of constraint-based causal discovery, covering algorithms such as PC and FCI with a focus on assumptions (faithfulness, Markov condition), robustness, and scalability in high-dimensional and mixed-type settings common in biomedicine. Covers kernel-based, rank-based, and model-based tests, discussing their behaviour under violations and practical guidance for test selection.

**Why relevant:** Central reference for CI testing in PC/FCI-style causal discovery — exactly at the intersection of CI testing methodology and constraint-based structure learning in the research profile.

---

### Interpretable Causal Discovery via Causal-Effect Constraints
**Cixuan Zhang, Guy Van den Broeck, Benjie Wang**
[arXiv:2608.12640](https://arxiv.org/abs/2608.12640v1) | `cs.LG`, `cs.AI`, `stat.ML`

Frames *conditional causal discovery* as Bayesian inference: given data, identify graphs consistent with the Markov equivalence class that also explain observed causal effect magnitudes. Causal-effect constraints (e.g. "why is this effect so large?") are incorporated as soft evidence, yielding a posterior over candidate DAGs that is both statistically grounded and interpretable.

**Why relevant:** Combines equivalence-class reasoning with causal-effect queries — directly relevant to constraint-based discovery and identification under structural constraints.

---

### Measuring the Arrow of Time: Identification, Estimation, and Inference for Directional Structure in Multivariate Time Series
**Avishek Bhandari**
[arXiv:2608.13431](https://arxiv.org/abs/2608.13431v1) | `econ.EM`, `stat.ME`

Develops a complete frequentist method for inferring the direction (arrow of time) in coupled multivariate time series by isolating the part of joint dynamics that changes when the record is reversed. Builds on spectral characterisations of Granger-causal asymmetry and provides identification conditions, estimators, and bootstrap inference.

**Why relevant:** Rigorous causal-direction identification in time series; the time-reversal identification idea parallels asymmetry-based causal discovery and connects to Granger/structural time-series methods.

---

## Confounding, Identification & Adjustment

### Inverse Confounding Analysis: An Exact Method for Quantifying the Significance of Confounding
**Sergey Porotsky**
[arXiv:2608.11991](https://arxiv.org/abs/2608.11991v1) | `stat.ME`, `stat.AP`

Introduces Inverse Confounding Analysis (ICA), an exact (non-asymptotic) sensitivity-analysis framework that asks: given the observed association, how strong must an unmeasured confounder be to nullify or reverse the estimated effect? Goes beyond worst-case Rosenbaum-style bounds by deriving exact distributions of the confounding-adjusted estimator under structured unmeasured confounding models.

**Why relevant:** Addresses unmeasured confounding — a central concern in the research profile — with an exact quantification rather than worst-case bounds; complements FCI-based latent variable approaches.

---

### COMPACT: Spectral Adjustment Scores from a Complete and Irreducible Causal Criterion
**Eric V. Strobl**
[arXiv:2608.10305](https://arxiv.org/abs/2608.10305v1) | `stat.ME`, `stat.ML`

Proposes COMPACT, a spectral method that constructs adjustment scores from a *complete and irreducible* causal criterion rather than the propensity score. When confounding is diffuse across many variables, spectral features of the joint covariate distribution capture adjustment information that propensity-score methods miss; the paper provides theoretical guarantees and a practical algorithm.

**Why relevant:** Addresses high-dimensional covariate adjustment using graph-theoretic causal criteria and spectral methods — relevant to both graphical models and high-dimensional confounding in the research profile.

---

### Causal Inference for Group-Contaminated Structured Outcomes: Observable Quotients, Lossless Reduction and Exact Randomization Inference
**Usef Faghihi, Amir Saki**
[arXiv:2608.11954](https://arxiv.org/abs/2608.11954v1) | `stat.ME`, `cs.AI`

Studies identification when structured potential outcomes (e.g. microscopy images) are observed only up to an unknown, unit-specific group transformation that may depend on treatment. Characterises the observable information (quotient by the group action), proves a lossless reduction, and constructs exact finite-sample randomisation tests for treatment effects on the equivalence-class level.

**Why relevant:** Novel identifiability and inference framework for structured outcomes under non-standard observation models — methodologically connected to identification under latent transformations and group-equivariant causal reasoning.

---

## Treatment Effect Estimation & Observational Studies

### Bias-Robust Causal Inference for Panel Data
**Angelos Alexopoulos**
[arXiv:2608.09837](https://arxiv.org/abs/2608.09837v1) | `econ.EM`, `stat.ME`

Adapts bias-aware minimax methods (developed for factor-model regression) to panel-data causal targets: the average treatment effect in observational panels where untreated outcomes are imputed. Explicitly accounts for counterfactual imputation error in standard errors, yielding confidence intervals with guaranteed coverage properties even when the imputation model is misspecified.

**Why relevant:** Minimax-robust causal inference under model uncertainty in panel settings; the bias-aware framework connects to the research profile's interest in robust identification under latent confounding.

---

### Local Conformal Prediction for Individual Causal Effects
**Fernando Delbianco, Fernando Tohmé**
[arXiv:2608.09612](https://arxiv.org/abs/2608.09612v1) | `stat.ME`, `econ.EM`

Proposes Individualized Causal Prediction (ICP): a localized conformal prediction framework that constructs finite-sample valid intervals for individual causal effects (ICEs) rather than just CATE means. Calibration is localised to a neighbourhood of the query unit, providing coverage guarantees for individual counterfactuals under strong treatment-effect heterogeneity.

**Why relevant:** Bridges conformal prediction with individual causal effect identification; addresses a gap where standard CATE interval methods fail under heterogeneity — relevant to inference for individual-level causal quantities.

---

### Estimating the Average Treatment Effect under Limited Overlap via Polynomial Approximation and Extrapolation
**Shunichiro Orihara, Sho Komukai, Fan Li**
[arXiv:2608.09329](https://arxiv.org/abs/2608.09329v1) | `stat.ME`

Addresses ATE estimation when covariate overlap is poor: instead of trimming or reweighting, proposes polynomial extrapolation of the outcome model into the non-overlapping region. Derives the bias-variance trade-off of the polynomial degree, establishes asymptotic normality, and shows the method dominates IPW and overlap-weighted estimators when overlap is limited.

**Why relevant:** Tackles a fundamental identification challenge (limited overlap) with a novel extrapolation strategy — relevant to the methodology of causal identification in observational data.

---

### Clustering Informed Inverse Probability Weighting Strategies for Causal Effect Estimation in Observational Studies
**Ruohui Chen, Scott Zuo, Whitney Stevens et al.**
[arXiv:2608.09839](https://arxiv.org/abs/2608.09839v1) | `stat.ME`, `stat.AP`

Compares three IPW strategies under treatment-assignment heterogeneity: standard IPW, clustering-augmented IPW with cluster-specific propensity models, and a global model with cluster membership as a feature. Establishes that cluster-specific models reduce variance in heterogeneous settings, with an analysis of the bias-variance trade-off as cluster granularity changes.

**Why relevant:** Propensity-score methodology under heterogeneous confounding — directly applicable when the propensity model is misspecified for subpopulations, complementing the research profile's focus on high-dimensional observational studies.

---

### Doubly Robust Estimation of Causal Effect on CVR with Targeted Regularization
**Jiayi Dan, Bo Li, Lu Deng et al.**
[arXiv:2608.13461](https://arxiv.org/abs/2608.13461v1) | `cs.LG`

Develops a doubly robust estimator for the causal effect on post-click conversion rate (CVR) that corrects for sample selection bias (only clicked samples are observed). Combines a propensity score correction for selection with outcome-model regularization targeted at the DR estimand, and proves semi-parametric efficiency in this two-stage observational setting.

**Why relevant:** Doubly robust causal estimation under selection bias — extends DR methodology to a two-stage selection/outcome model, illustrating broader identification challenges relevant to the research profile.

---

## Experimental Design & Interventions

### Sharp Minimax Theory for Randomized Experiments
**Timothy Sudijono, Edgar Dobriban, Eric Tchetgen Tchetgen**
[arXiv:2608.13822](https://arxiv.org/abs/2608.13822v1) | `math.ST`, `econ.EM`, `stat.ME`

Derives minimax-optimal randomization designs and estimators for the sample average treatment effect in finite-population experiments, with no restrictions on the design or estimator class. For binary potential outcomes, reduces the minimax risk to a two-parameter problem, establishing second-order sharp bounds and optimal adaptive designs.

**Why relevant:** Optimal experimental design theory with minimax guarantees — directly relevant to the research profile's interest in interventional experimental design and its statistical foundations.

---

### Theoretical Properties of Covariate-Adaptive Randomization with a Diverging Number of Covariates
**Yuhang Tao, Li-Xin Zhang**
[arXiv:2608.13442](https://arxiv.org/abs/2608.13442v1) | `stat.ME`, `math.ST`

Studies two unified families of covariate-adaptive randomization procedures (stratified and minimization-type) when the number of covariates grows with sample size. Establishes consistency of the randomization distribution, asymptotic balance properties, and valid inference for treatment effects in this high-dimensional-covariate regime.

**Why relevant:** Extends adaptive randomization theory to high-dimensional covariates — relevant to the research profile's interest in high-dimensional experimental design for causal studies.

---

### Chance-Constrained Selection of Sequential Intervention Strategies from Counterfactual Estimates
**Minkyoung Kim, Beakcheol Jang**
[arXiv:2608.13209](https://arxiv.org/abs/2608.13209v1) | `stat.ME`, `cs.LG`, `stat.ML`

Addresses the problem of choosing among sequential intervention strategies under a cumulative budget constraint, when both outcomes and costs are counterfactual quantities identified from observational data. Introduces chance-constrained selection that controls the probability of exceeding the budget, going beyond expected-cost formulations used in standard robust decision frameworks.

**Why relevant:** Sequential intervention selection under counterfactual identification from observational data — directly connects to the research profile on interventional causal discovery and optimal experimental design.

---

## Mediation Analysis

### Causal Mediation Analysis for Network Data with Graph Neural Network
**Peikai Wu, Zhiguo Xiao**
[arXiv:2608.13274](https://arxiv.org/abs/2608.13274v1) | `stat.ME`

Develops a nonparametric mediation framework for a single large observed network allowing simultaneous treatment and mediator spillovers (network interference) and high-dimensional network confounding. Uses graph neural networks for nuisance estimation, defines causal estimands via exposure and mediator mappings, and establishes identification and estimation theory without restricting the true interference mechanism.

**Why relevant:** Extends mediation analysis to networked populations under interference — expands the graphical causal framework to settings where SUTVA fails, relevant to causal inference with structured data.

---

### Causal Mediation Analysis with a Time-Dependent Mediator, Time-Dependent Confounders and a Time-to-Event Outcome: Revisiting the Difference Method
**Robin Denz, Nina Timmesfeld**
[arXiv:2608.13094](https://arxiv.org/abs/2608.13094v1) | `stat.ME`

Revisits the difference method for mediation when the mediator and confounders are time-varying and the outcome is a survival time. Establishes under which structural assumptions the difference estimator correctly targets the natural direct/indirect effects, derives its asymptotic properties, and proposes a simple regression-based implementation with bootstrap inference.

**Why relevant:** Identification and estimation of mediation in complex longitudinal settings — extends graphical/structural causal model mediation theory to the survival analysis domain.

---

## Graphical Models & Structure

### Graph Causal Optimal Transport and Wasserstein Distances
**Jan Obłój, Vlad Tuchilus**
[arXiv:2608.13716](https://arxiv.org/abs/2608.13716v1) | `math.PR`, `math.OC`, `math.ST`

Characterises graph causal optimal transport (GCOT): optimal transport where allowable couplings satisfy causal restrictions prescribed by a DAG. Fully identifies which DAGs make the associated graph causal Wasserstein discrepancy a metric, and shows the induced topology agrees with other natural adapted topologies. Connects to causal versions of optimal transport on filtered probability spaces.

**Why relevant:** Provides a metric geometry for causal models encoded by DAGs — a theoretical foundation for comparing causal distributions under structural constraints, relevant to causal structure learning and identification.

---

### From Rating Factors to Crash Mechanisms: A Multiscale Causal DAG Framework Linking Motor Insurance and Road Safety
**Arthur Charpentier**
[arXiv:2608.09441](https://arxiv.org/abs/2608.09441v1) | `stat.AP`, `econ.EM`, `stat.ME`

Proposes a multiscale causal DAG framework that connects actuarial rating factors (observed annually) to the fast causal crash-occurrence process (within seconds/trips). The three-part framework (crash-occurrence graph, severity graph, insurance-observation graph) makes the mismatch between causal mechanisms and observational aggregation explicit and enables principled causal identification across timescales.

**Why relevant:** Applied DAG construction and multiscale causal identification — illustrates causal graph methodology in a domain where temporal aggregation creates identifiability challenges, connecting to graphical model practice.

---

## Other Relevant

### Expert-Guided g-Computation with Large Language Models for Estimating Causal Effects on Timings: Applications to Hospital Quality Improvement
**Patrick Vossler, Jialin Ouyang, F. Richard Guo et al.**
[arXiv:2608.10339](https://arxiv.org/abs/2608.10339v1) | `stat.ME`, `cs.AI`, `stat.AP`

Uses LLMs to elicit expert-encoded structural assumptions that guide g-computation for estimating causal effects of hospital interventions on length-of-stay. The LLM constructs candidate adjustment sets and encodes qualitative causal knowledge, which is then combined with standard g-computation estimators, providing a practical workflow for expert-knowledge-augmented causal inference.

**Why relevant:** G-computation is a core causal identification method; the LLM-knowledge-elicitation angle is a novel interface for encoding graphical-model assumptions in practice.

---

### From Prediction to Incrementality: Causal Optimization for Large-Scale Targeting and Recommendation
**Changshuai Wei, John Bencina, Phuc Nguyen et al.**
[arXiv:2608.10182](https://arxiv.org/abs/2608.10182v1) | `cs.LG`, `cs.AI`

Argues that prediction-based allocation in marketing/recommendation systematically misallocates to users who would act anyway; proposes a decision-centric framework that instead optimises for incremental causal impact (uplift). Develops scalable estimators for heterogeneous treatment effects in high-dimensional feature spaces and demonstrates gains in a large-scale production targeting system.

**Why relevant:** Large-scale heterogeneous treatment effect estimation for decision-making — illustrates how causal inference methods translate to production systems, adjacent to the optimal experiment/intervention design thread.

---

*Digest generated automatically on 2026-08-17. 821 papers scanned via the arXiv API across categories stat.ME, math.ST, stat.ML, cs.LG. Only papers actually returned by the API are included — no fabricated entries.*
### GENESIS: Towards Explainable Causal Discovery
**Abhinav Thorat, Ravi Kumar Kolla, Vishak K Bhat, Harsh Vardhan Singh Chauhan, Niranjan Pedanekar**
[arXiv:2608.03868](https://arxiv.org/abs/2608.03868) | `cs.LG`, `cs.AI`

Proposes GENESIS, a hybrid causal discovery framework that decomposes DAG learning into auditable decision points: it scores three-node structural motifs (chains, forks, colliders) to establish structural priors, then refines the graph by integrating statistical evidence and Markov blanket consistency, invoking LLM domain knowledge only when statistics are insufficient. Every edge decision is traceable to an explicit source of evidence, achieving 100% decision traceability while outperforming purely statistical baselines on SHD.

**Why relevant:** Directly addresses structure learning over DAGs with Markov blanket consistency as a core constraint; the motif-scoring approach is an explicit connection to constraint-based discovery (collider detection, orientation).

---

### SVI-DAG: A Structured Variational Inference Approach to Bayesian Causal Discovery
**Shrenik Zinage**
[arXiv:2608.04930](https://arxiv.org/abs/2608.04930) | `cs.LG`, `cs.AI`

Introduces SVI-DAG, a Bayesian causal discovery method that uses normalizing flows to model dependencies between edges in a DAG posterior, overcoming the edge-independence assumption of prior approaches. Stein variational gradient descent (in acyclicity space) is used to promote mode coverage and reduce mode-seeking bias in the ELBO; experiments show gains in uncertainty quantification over five Bayesian DAG baselines.

**Why relevant:** Addresses identifiability and posterior uncertainty in causal structure learning, with principled handling of multimodal equivalence classes in the DAG posterior.

---

### Adversarial Causal Intervention Falsification
**Mojtaba Eslami**
[arXiv:2608.06427](https://arxiv.org/abs/2608.06427) | `cs.LG`, `cs.GT`, `econ.EM`, `stat.ME`

Frames causal model validation as a sequential game: a structural causal generator proposes observational and interventional distributions, while an adversarial experimentalist selects interventions to maximally falsify it. Proves exact reduction of the adversarial objective to a worst-intervention integral probability metric, identification up to interventional equivalence (with point identification under a separating intervention family), and logarithmic elimination of competing models under a balanced-separation sequential design.

**Why relevant:** Directly addresses active causal discovery via intervention selection, and the distinction between observational fit, interventional equivalence, and point SCM identification — core to the JCI/intervention-target identification framework.

---

### A Fully Nonlinear Structural Vector Autoregressive Model Identified via Independent Innovation Analysis
**Savi Virolainen**
[arXiv:2608.03486](https://arxiv.org/abs/2608.03486) | `econ.EM`, `stat.ME`, `stat.ML`

Develops a nonlinear SVAR where the contemporaneous structural mapping is fully nonlinear and non-additive; identification is achieved by exploiting variation in the conditional distributions of mutually independent structural shocks induced by an observed exogenous variable, using contrastive learning within an exponential-family framework. Under a logistic specification the remaining ambiguity is reduced to permutation and componentwise sign changes, and the structural map is estimated with feed-forward neural networks.

**Why relevant:** Strengthens identification results for non-linear SEMs via exogenous variation — directly relevant to structure learning under non-Gaussian/nonlinear regimes and to the question of how interventional variation identifies structural parameters.

---

## SEM & Graphical Models

### A Bures-Wasserstein Formulation of Matrix Decomposition Structural Equation Modeling
**Naoto Yamashita**
[arXiv:2608.03183](https://arxiv.org/abs/2608.03183) | `stat.ME`

Shows that minimizing the matrix-decomposition SEM (MDSEM) loss is equivalent to minimizing the squared Bures-Wasserstein distance between observed and model-implied covariance matrices, establishing the MDSEM estimator as a minimum-discrepancy covariance-based SEM estimator. This equivalence yields consistency, asymptotic normality, and standard errors, while also providing numerical stability advantages over conventional ML estimation in small samples.

**Why relevant:** Provides a geometric (optimal-transport) grounding for structural equation models; directly relevant to graphical model estimation and the theoretical properties of SEM estimators.

---

## Causal Effects & Unmeasured Confounding

### Regression-Based Proximal Reconciliation of Conflicting Trials with Unmeasured Effect Modifiers
**Daniel A Xu, Eric J Tchetgen Tchetgen, Enrique F Schisterman, Sean C Blackwell, Ellen C Caniglia**
[arXiv:2608.04202](https://arxiv.org/abs/2608.04202) | `stat.ME`, `stat.AP`

Develops a causal inference framework for assessing whether conflicting RCT findings are *reconcilable* when effect modifiers are unmeasured; uses proxy variables (proximal causal inference) to test conditional reconcilability and extends transportability methods to assess marginal reconcilability. Introduces a reconciliation proportion to quantify the degree of marginal reconciliation, illustrated on conflicting trials of 17-alpha-hydroxyprogesterone caproate.

**Why relevant:** Applies proximal causal inference and transportability methodology in the presence of latent effect modifiers — directly connects latent confounding, proxy variables, and evidence synthesis.

---

### Causal Inference with Unstructured Outcomes
**Kevin Christian Wibisono, Yixin Wang**
[arXiv:2608.03085](https://arxiv.org/abs/2608.03085) | `stat.ML`, `cs.LG`

Proposes a causal query framework for settings where outcomes are texts or images (where conventional ATE is ill-defined): the *maximally contrasting feature* (MCF), a learned scalar function that maximally sharpens the contrast between treated and control potential outcomes. Develops identification conditions and estimation algorithms, with extensions to heterogeneous effects and unstructured treatments.

**Why relevant:** Extends the potential-outcomes framework beyond scalar outcomes — methodologically adjacent to causal effect identification in non-standard outcome spaces.

---

## Interventions & Experimental Design

### A Design-Based Minimax Theory for Network Experiments
**Vardis Kandiros, Christopher Harshaw, Fredrik Sävje**
[arXiv:2608.04909](https://arxiv.org/abs/2608.04909) | `math.ST`, `stat.ME`

Establishes minimax risk theory for causal effect estimation in network experiments under an arbitrary neighborhood interference model; shows that the minimax risk is determined by the *conflict graph* (capturing unobservability of estimand-relevant potential outcomes), and provides matching upper and lower bounds via local and global connectivity properties of the conflict graph. Applied to derive minimax rates for direct and global average treatment effects.

**Why relevant:** Brings fundamental lower-bound theory to causal estimation under interference — relevant to the optimal experimental design strand of causal inference and to understanding estimation limits in graph-structured settings.

---

### Target-Weighted Neyman Allocation: Experimental Design for Heterogeneous Treatment Effects under Population Shift
**Hoang Dang, Luan Pham, Minh Nguyen**
[arXiv:2608.06512](https://arxiv.org/abs/2608.06512) | `cs.LG`, `stat.ME`

Proposes TWNA (Target-Weighted Neyman Allocation), a two-stage stratified experimental design that allocates sample sizes and treatment probabilities to minimise variance of the target-population group ATE (GATE) when experiments are run in a source population different from deployment. The oracle allocation balances deployment importance and statistical difficulty; a plug-in rule and an extension robust to uncertain deployment composition are also provided.

**Why relevant:** Addresses experimental design for causal effect estimation under population shift, a transportability-adjacent problem; relevant to optimal intervention design when the target distribution differs from the experimental distribution.

---

## Other Relevant

### Amortized Interventional Forecasting for Multivariate CIR Processes
**Andreas Sauter, Sumit Sourabh, Drona Kandhai, Erman Acar**
[arXiv:2608.03715](https://arxiv.org/abs/2608.03715) | `cs.LG`, `cs.CE`

Introduces CIR-ACTIVA, an amortized framework for distributional causal effect estimation in multivariate Cox-Ingersoll-Ross (mean-reverting) processes, providing calibrated multi-horizon shock responses without retraining per intervention scenario. Also contributes a causal multivariate CIR data-generating process with paired observational/interventional ground truth for benchmarking.

**Why relevant:** Demonstrates amortised interventional inference in a structured parametric family — relevant to efficient causal effect estimation under do-calculus-style interventions in time-series settings.

---

### As Good as it Gets: Bounds for Oracle Time-Varying Treatment Strategies
**Zach Shahn**
[arXiv:2608.03133](https://arxiv.org/abs/2608.03133) | `math.ST`

Extends sharp bounds on oracle individualized treatment rules from the point-exposure to the time-varying setting, deriving bounds on the performance of a strategy that selects the best regime per subject based on unobserved potential outcomes. For continuous outcomes the lower bound can strictly exceed the maximum covariate-based value, and bounds on the CDF of oracle potential outcomes are also derived.

**Why relevant:** Contributes fundamental identification limits for dynamic treatment regimes — relevant to the theoretical underpinnings of interventional causal inference and optimal policy design.

---

## Previous Digests

- [2026-W34](archive/2026-W34.md) -- August 10 -- 17, 2026 (20 papers)
- [2026-W32](archive/2026-W32.md) -- July 27 -- August 3, 2026 (20 papers)
- [2026-W29](archive/2026-W29.md) -- July 13 -- 20, 2026 (15 papers)
- [2026-W28](archive/2026-W28.md) -- June 29 -- July 6, 2026 (14 papers)
- [2026-W27](archive/2026-W27.md) -- June 22 -- 29, 2026 (19 papers)
- [2026-W26](archive/2026-W26.md) -- June 15 -- 22, 2026 (15 papers)
- [2026-W25](archive/2026-W25.md) -- June 10 -- 17, 2026 (19 papers)
- [2026-W32](archive/2026-W32.md) — July 27 – August 3, 2026
- [2026-W31](archive/2026-W31.md) — July 20 – July 27, 2026
- [2026-W29](archive/2026-W29.md) — July 6 – July 13, 2026
- [2026-W28](archive/2026-W28.md) — June 29 – July 6, 2026
- [2026-W27](archive/2026-W27.md) — June 22 – June 29, 2026
- [2026-W26](archive/2026-W26.md) — June 15 – June 22, 2026
- [2026-W25](archive/2026-W25.md) — June 8 – June 15, 2026
