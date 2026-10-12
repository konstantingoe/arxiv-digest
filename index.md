---
layout: default
title: arXiv Digest — Causal Inference & Discovery
---

# arXiv Digest — Causal Inference & Discovery

Weekly digest of arXiv papers relevant to causal inference, causal discovery, graphical models, and conditional independence testing. Updated automatically every Monday.

---

# arXiv Digest — 2026-W42

**Covered:** 2026-10-05 to 2026-10-12 UTC  
**Scanned:** 1 598 papers (stat.ME, math.ST, stat.ML, cs.LG)  
**Selected:** 22 papers

---

## Causal Discovery & Structure Learning

**[DAG-CLIP: A DAG Learning Framework in the Presence of Latent Variables](https://arxiv.org/abs/2610.06086)**  
Siliang Zhang, Yunxiao Chen, Irini Moustaki · *stat.ME, stat.ML* · 2026-10-05  
Proposes a general statistical framework for DAG learning when some or all nodes are latent constructs defined by measurement models, recovering an equivalence class characterised by a new notion of Markov equivalence under partial observability.  
*Why relevant:* Directly addresses structure learning with latent variables—a core challenge in the user's work on ancestral graphs and MAGs/ADMGs.

---

**[Score-Based Learning of Cluster DAGs from Interventions](https://arxiv.org/abs/2610.11947)**  
Gaetano Tedesco, Alex Markham · *stat.ML, cs.LG* · 2026-10-08  
Score-based approach that simultaneously learns the cluster partition and the edges of a cluster DAG from interventional data, building on the notion of interventional coarsening.  
*Why relevant:* Combines interventional causal discovery with causal abstraction/coarsening—relevant to JCI-style multi-environment structure learning.

---

**[GO-Based Clustering for Learning Cluster-Level Causal Gene Regulatory Networks](https://arxiv.org/abs/2610.06042)**  
Azlaan Mustafa Samad, Wei Zhang, Adèle H Ribeiro · *cs.LG* · 2026-10-05  
Uses Gene Ontology annotations to construct admissible cluster partitions that guarantee an acyclic cluster graph, then applies cluster-level causal discovery methods that respect the discovered equivalence classes.  
*Why relevant:* Addresses DAG-over-clusters identifiability and equivalence classes; high-dimensional graphical models angle.

---

**[DAG Structure Learning with Node-Varying Heavy-Tailed Disturbances](https://arxiv.org/abs/2610.13304)**  
Robin Francis, Sundeep Prabhakar Chepuri · *cs.LG* · 2026-10-09  
Extends DAGMA-style continuous-constrained DAG learning to node-varying Student-*t* noise, jointly estimating the DAG and per-node scale/shape parameters via a smooth log-determinant acyclicity penalty.  
*Why relevant:* Score-based DAG learning methodology under non-Gaussian SEMs; connects to non-parametric structure learning.

---

**[Directional Evidence Guided Search-Space Reduction for Exact DAG Learning](https://arxiv.org/abs/2610.09136)**  
Upala Junaida Islam, Abdelmonem Elrefaey, Rong Pan · *cs.LG* · 2026-10-06  
Hybrid (constraint + score) framework DECO that uses non-parametric conditional independence tests to prune the parent-set search space before exact score-based DAG enumeration, substantially reducing computational cost.  
*Why relevant:* Hybrid CI-test + score-based DAG learning; relevant to constraint-based and exact structure-learning methodology.

---

**[AdaPS-LiNGAM: Adaptive Predecessor Selection for LiNGAM under Small-Sample Settings](https://arxiv.org/abs/2610.09782)**  
Shun Yanashima, Kentaro Kanamori, Hirofumi Suzuki · *cs.LG, stat.ML* · 2026-10-07  
Improves DirectLiNGAM in small-sample regimes by adaptively selecting which predecessor candidates to test, reducing error accumulation in the sequential variable-removal procedure.  
*Why relevant:* LiNGAM / linear non-Gaussian causal discovery; practical improvements directly relevant to identifiable observational structure learning.

---

**[Executing Causal Structure Learning with Linear-Attention Transformers](https://arxiv.org/abs/2610.10395)**  
Amartya Roy, Sayar Karmakar · *cs.LG* · 2026-10-07  
Shows that a fixed-weight linear-attention transformer can exactly reproduce one update step of gradient-based continuous DAG optimization, so a deep stack of identical blocks emulates the full optimization trajectory.  
*Why relevant:* Theoretical analysis of algorithm execution by transformers applied to causal structure learning.

---

**[One Thing Leads to Another: The Essentials of Time Series Causal Discovery](https://arxiv.org/abs/2610.13430)**  
Kurt Butler, Damian Machlanski, Michael P. J. Camilleri et al. · *eess.SP, cs.LG, stat.ML* · 2026-10-09  
Tutorial survey unifying time series causal discovery across signal processing, statistics, dynamical systems and ML, covering Granger causality, structural VAR, constraint-based and score-based methods.  
*Why relevant:* Broad-coverage reference for time-series structure learning; useful for grounding causal discovery methods in time-series settings.

---

## Interventions, Identifiability & Latent Confounding

**[ProximalFM: Amortized Proximal Causal Inference under Hidden Confounding](https://arxiv.org/abs/2610.08078)**  
Christophe Muller, Ayub Kharel, Alex Luedtke, Chan Park et al. · *stat.ML, cs.LG* · 2026-10-06  
Introduces a foundation-model approach that amortizes the solution of the proximal ill-posed integral equation over a distribution of CATE estimation tasks, enabling scalable causal effect estimation under unmeasured confounding via proxy variables.  
*Why relevant:* Directly addresses hidden confounding via proximal inference—closely related to soft-intervention identification under latent confounders.

---

**[Score-Based Methods for Selecting Direct Causes in Reweighted Distributions](https://arxiv.org/abs/2610.09100)**  
Jacob M. Chen, Ilya Shpitser · *stat.ME* · 2026-10-06  
Generalises BIC-based model selection to reweighted distributions (e.g. from causal inference, missing data, domain shift) by introducing a *reweighted BIC* that remains consistent for selecting direct causes even when the observed likelihood is distorted.  
*Why relevant:* Score-based cause selection under unmeasured confounding; overlaps with Markov boundary selection and score-based DAG learning in non-identically distributed settings.

---

**[What Should We Measure Next? Finding Identification Strategies by Refining Mechanisms](https://arxiv.org/abs/2610.08092)**  
Mikko Väänänen, Fanyu Cui, Carlos Cinelli, Santtu Tikka · *stat.ME* · 2026-10-06  
Frames identification as an iterative process: given a partially specified causal model, proposes a procedure to find the minimal additional measurements (new variables or interventions) needed to identify a target causal effect.  
*Why relevant:* Active experimental design for identification—directly connected to interventional causal discovery and efficient experimental design for causal queries.

---

**[Symmetry-Informed Causal Partial Identification](https://arxiv.org/abs/2610.09230)**  
Uzair Akbar, Zulfiqar Zaidi, Niki Kilbertus, Krikamol Muandet et al. · *cs.LG* · 2026-10-06  
Exploits known data symmetries (e.g. permutation invariance) as additional constraints in partial identification programmes to tighten otherwise vacuous bounds on causal effects.  
*Why relevant:* Partial identification / causal bounds methodology; relevant to settings with latent confounders where point identification fails.

---

**[The Missing Corner: When Sharp Causal Bounds Fail to Compose](https://arxiv.org/abs/2610.08197)**  
*(stat.ME)* · 2026-10-06  
Characterises exactly when sharp bounds on two separate potential-outcome means can be subtracted to yield sharp bounds on the ATE—showing this fails in general—and derives conditions under which sharp composition is guaranteed.  
*Why relevant:* Fundamental result on partial identification and causal bounds; relevant to sensitivity analysis and bounds-based identification.

---

**[Instrumental Variable Analysis in Underrepresented Subpopulations Powered by Knowledge Transfer](https://arxiv.org/abs/2610.05680)**  
Ruoyu Wang, Zijian Xu, Zijian Guo, Xihong Lin et al. · *stat.ME* · 2026-10-05  
Proposes KNIVES, an IV estimator for underrepresented subpopulations that transfers knowledge from a well-studied source population to combat weak-IV bias and low-efficiency in the target subgroup.  
*Why relevant:* IV methodology for heterogeneous populations; connects to transportability and effect estimation under distributional shift.

---

## Conditional Independence Testing & Methodology

**[Embedding-Bias in Conditional Independence Testing](https://arxiv.org/abs/2610.11584)**  
Nikolaj Thams, Anton Rask Lundborg · *stat.ML, cs.LG* · 2026-10-08  
Shows that conditioning on an embedding *ψ*(*Z*) instead of raw *Z* can inflate type-I error to 1 in a CI test unless the embedding preserves conditional independence; derives a relaxed sufficient condition and a residual-correlation test that mitigates the bias.  
*Why relevant:* Critical methodological point for kernel/embedding-based CI tests used in causal discovery pipelines.

---

**[Sequential Conditional Independence Testing with Machine Learning Models](https://arxiv.org/abs/2610.11388)**  
Angel Reyero-Lobo, Michele Meziu, Sebastian Uriel Arias, Peter Grünwald et al. · *math.ST, stat.ML* · 2026-10-08  
Develops log-optimal e-variables for CI testing under the model-X assumption that incorporate arbitrary ML regression models, enabling sequential/anytime-valid tests with strong power guarantees.  
*Why relevant:* E-variable-based CI testing with data-adaptive models—directly applicable to kernel and ML-augmented CI tests used in FCI/GCM-style procedures.

---

## Causal Representation Learning

**[Block Disentanglement in CRL: Bridging Identifiability and Visual State Estimation](https://arxiv.org/abs/2610.06809)**  
Emre Acartürk, Pranamya Kulkarni, Puranjay Datta, Karthikeyan Shanmugam et al. · *cs.LG, stat.ML* · 2026-10-05  
Studies block-level identifiability of causal latent variables in CRL, proving conditions under which visual observations suffice to recover causally-related latent blocks and demonstrating this on robotic state estimation tasks.  
*Why relevant:* Identifiability of latent causal structure from interventional data; connects to unknown intervention targets and latent confounding.

---

**[Probabilistic Counterfactual Inference for Discrete Outcomes in Gaussian-Process Causal Models](https://arxiv.org/abs/2610.08689)**  
Juliette Sinnott, Amir-Hossein Karimi, Mohammad Kohandel · *cs.LG* · 2026-10-06  
Extends GP-SCM counterfactual inference to heterogeneous variable types (continuous + discrete children) by pairing GP predictors with explicit exogenous noise mechanisms and deriving exact conditional noise-abduction procedures.  
*Why relevant:* Counterfactual inference in SCMs with mixed-type graphs—relevant to nonparametric structural causal models and discrete outcome interventions.

---

## Applied Causal Inference

**[sHAIL-Causal: A Sequential Staircase Procedure for Invariant Causal Predictor Discovery](https://arxiv.org/abs/2610.07057)**  
Ernest Fokoué · *stat.ML, cs.LG* · 2026-10-05  
Instantiates the sHAIL hierarchical incremental learning paradigm with a joint saturation-and-cross-environment-invariance criterion to identify causally stable predictors across environments, extending ICP to a sequential nested-hypothesis-class framework.  
*Why relevant:* Invariant causal prediction / IRM-style invariant risk minimisation; relevant to multi-environment causal discovery.

---

**[Longitudinal Causal Inference under Informative Missingness using the Self-Censoring Model](https://arxiv.org/abs/2610.09234)**  
Iván Díaz · *stat.ME* · 2026-10-06  
Develops identification and semiparametric efficient estimation for longitudinal treatment policies when covariates are missing not at random (MNAR), using a self-censoring structural model as the key identifying assumption.  
*Why relevant:* Observational causal inference from EHR-style longitudinal data with MNAR—connects semiparametric efficiency and causal identification under selection bias.

---

**[Collaborative Representations for Targeted Causal Inference under Outcome Selection](https://arxiv.org/abs/2610.08073)**  
*(stat.ME)* · 2026-10-06  
Proposes a collaborative representation-based targeted learning (TMLE) method that jointly trains outcome, exposure, and selection models to avoid propensity-score over-fit, reducing bias in causal effect estimates under missing outcomes.  
*Why relevant:* Targeted/semiparametric causal estimation with selection mechanisms—relevant to double-robustness and efficient estimation in observational studies.

---

**[Prediction-Powered Data Fusion for Treatment Effect Estimation](https://arxiv.org/abs/2610.12332)**  
*(stat.ML, cs.AI, cs.LG)* · 2026-10-08  
Combines a small randomized trial with a large (possibly confounded) observational study via prediction-powered inference, yielding valid ATE and CATE estimators that borrow observational sample size without assuming observational unconfoundedness.  
*Why relevant:* Data fusion for treatment effect estimation under potential confounding; connects transportability and semi-supervised inference for causal quantities.

---

*This digest is generated automatically. Papers are selected for relevance to causal inference, causal discovery, graphical models, and conditional independence testing.*

---

## Archive

- [2026-W42](archive/2026-W42.md) — 2026-10-05 to 2026-10-12
- [2026-W40](archive/2026-W40.md) — Week 40, 2026
- [2026-W39](archive/2026-W39.md) — Week 39, 2026
- [2026-W38](archive/2026-W38.md) — Week 38, 2026
- [2026-W37](archive/2026-W37.md) — Week 37, 2026
- [2026-W36](archive/2026-W36.md) — Week 36, 2026
- [2026-W35](archive/2026-W35.md) — Week 35, 2026
- [2026-W34](archive/2026-W34.md) — Week 34, 2026
- [2026-W33](archive/2026-W33.md) — Week 33, 2026
- [2026-W32](archive/2026-W32.md) — Week 32, 2026
- [2026-W31](archive/2026-W31.md) — Week 31, 2026
- [2026-W29](archive/2026-W29.md) — Week 29, 2026
- [2026-W28](archive/2026-W28.md) — Week 28, 2026
- [2026-W27](archive/2026-W27.md) — Week 27, 2026
- [2026-W26](archive/2026-W26.md) — Week 26, 2026
- [2026-W25](archive/2026-W25.md) — Week 25, 2026
