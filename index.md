---
layout: default
---

# arXiv Digest: Causal Inference & Discovery

Weekly curated digest of arXiv papers on causal inference, causal discovery, graphical models, conditional independence testing, and related methodology.

---

# arXiv Digest 2026-W36

**Week of August 24 – 31, 2026**

Categories scanned: `stat.ME`, `math.ST`, `stat.ML`, `cs.LG`
Papers scanned: 793 | Papers selected: 14

---

## Causal Discovery & Structure Learning

### I-FLOP: Fast Learning of Order and Parents from Interventional Data
**Liuting Chen, Alex Markham**
[arXiv:2608.28245](https://arxiv.org/abs/2608.28245) | `cs.LG`, `stat.ML` | 2026-08-28

Extends the FLOP score-based causal structure learning algorithm (Wienöbst et al., 2026) from observational to interventional data using the interventional BIC score of Hauser & Bühlmann, with Cholesky-based score updates preserved for speed. The resulting algorithm recovers a DAG in the correct interventional Markov equivalence class in the sample limit, and is benchmarked against existing methods on real and simulated datasets.

*Why relevant: Directly extends a state-of-the-art score-based DAG learning method to interventional data and interventional Markov equivalence classes — core causal discovery methodology.*

---

### Scalable and Versatile Identification for Hierarchical Structural Causal Models: A New Look at Project STAR
**Janis Aiad, Aghiles Drali, Aymen El Ouadrhiri et al.**
[arXiv:2608.24500](https://arxiv.org/abs/2608.24500) | `stat.ME` | 2026-08-25

Develops a complete pipeline for Hierarchical Structural Causal Models (HSCMs) that bridges symbolic causal identification (via pyAgrum's do-calculus) with practical estimation, applied to the STAR class-size experiment with nested observations. Provides open-source tooling for graph transformations and causal effect identification in multi-level settings.

*Why relevant: SCMs with nested/hierarchical structure and do-calculus identification — extends standard causal identification to a practically important class of experimental designs.*

---

### From Causal Plausibility to Causal Reliability: Evaluating LLMs as Calibrated Direct Causal-Edge Classifiers
**Amit Kumar, Elnur Adl Zarabi, Suranjana Trivedy et al.**
[arXiv:2608.23660](https://arxiv.org/abs/2608.23660) | `cs.LG`, `stat.ML` | 2026-08-24

Systematically evaluates 12 instruction-tuned open-weight LLMs across six benchmark causal graphs and five prompting strategies as sources of prior causal knowledge for structure learning. Finds LLM judgments are strongly recall-dominant (high recall, low precision), with verbalized confidence poorly calibrated relative to logit-based and cross-prompt agreement measures.

*Why relevant: Directly addresses reliability of LLM-derived causal priors used in causal discovery — important for hybrid knowledge+data structure learning pipelines.*

---

### Data Shared Neighbourhood Selection for multi-condition network inference
**Blanche Francheterre, Ruben Colindres Zuehlke, Vivian Viallon et al.**
[arXiv:2608.22901](https://arxiv.org/abs/2608.22901) | `stat.ME` | 2026-08-24

Proposes DSNS, a joint neighbourhood selection method that decomposes nodewise regression coefficients into shared and condition-specific components via a Data Shared Lasso, enabling simultaneous estimation of preserved and altered conditional independence structures across related conditions (e.g., disease vs. control).

*Why relevant: Directly extends Markov boundary / neighbourhood selection to multi-condition settings with shared structure — core graphical model methodology.*

---

## Graphical Models & Semiparametric Theory

### Toward a Semiparametric Efficiency Theory under Equality Constraints in Nested Markov Models
**Razieh Nabi, Anna Guo, Lin Liu**
[arXiv:2608.24602](https://arxiv.org/abs/2608.24602) | `stat.ME`, `math.ST` | 2026-08-25

Develops semiparametric efficiency theory for nested Markov models associated with Acyclic Directed Mixed Graphs (ADMGs), the latent projections of latent-variable DAGs. These models impose Verma constraints on the observed distribution beyond ordinary conditional independencies; the paper derives implications of these equality constraints for efficient estimation.

*Why relevant: Directly addresses ADMGs, nested Markov models, Verma constraints, and latent-variable DAG structure — central to the MAG/ADMG/PAG line of work.*

---

### Graph-based causal variance decompositions: When "variance explained" means causation
**Olli Saarela, Juha Karvanen**
[arXiv:2608.27140](https://arxiv.org/abs/2608.27140) | `stat.ME` | 2026-08-27

Shows that the standard ordered variance decomposition (via law of total variance) lacks causal meaning due to dependence on conditioning order; proposes a graph-based framework that defines causal counterparts of variance components, with component-by-component identifiability assessable against the full causal DAG without requiring the full topological ordering.

*Why relevant: Bridges graphical causal models and variance attribution — useful for root cause analysis and attributing outcome variance to specific causes within a DAG.*

---

## Causal Identification & Inference

### Identification and Inference for Causal Effects in Extremes under General Conditions
**Lisa Leimenstoll, Melanie Schienle**
[arXiv:2608.22957](https://arxiv.org/abs/2608.22957) | `stat.ME`, `math.ST` | 2026-08-24

Studies the Causal Tail Coefficient (CTC) as a measure of causal dependence in extremes within a linear SCM with heavy-tailed innovations, deriving identification conditions and asymptotic inference for tail-regime causal effects — extending standard average-effect econometrics to tail behaviour.

*Why relevant: Causal identification in SCMs extended to the extremes regime — relevant to causal discovery under non-standard distributional assumptions.*

---

### Causal Effects of Modified Treatment Policies under Positivity Violations: A Partial Identification Approach
**Taehyeon Koo, Elizabeth A. Stuart, Kara E. Rudolph et al.**
[arXiv:2608.23971](https://arxiv.org/abs/2608.23971) | `stat.ME` | 2026-08-25

Modified treatment policies (MTPs) shift each individual's treatment by a rule depending on their natural value. When positivity fails (e.g., continuous or multivariate treatments), this paper provides a partial identification framework decomposing the MTP mean outcome into a point-identified part and a bounded remainder, yielding sensitivity bounds without assuming the policy is fully supported.

*Why relevant: Partial identification for interventional causal effects with positivity violations — squarely in the causal identification / intervention design space.*

---

### Transporting Randomized Trial Effects to Real-World Populations via Riesz-Calibrated Optimal Transport
**Anik Burman, Margaret Gamalo, Promit Ghosal et al.**
[arXiv:2608.23453](https://arxiv.org/abs/2608.23453) | `stat.ME` | 2026-08-24

Proposes RICOT, which uses optimal transport to re-weight trial populations toward a target without modelling trial participation propensity scores, and adds a Riesz calibration step to enforce covariate balance. Shown more robust than propensity-score methods under covariate distribution mismatch.

*Why relevant: Transportability of causal effects from trial to target population — a core transportability problem addressed with a new geometric approach.*

---

### Marginal Structural Models for Electricity Demand under Treatment-Confounder Feedback: A Continuous-Treatment Outcome-Adaptive and Fused LASSO Approach
**Shalini Jayanetti, Sumeet Kalia**
[arXiv:2608.26411](https://arxiv.org/abs/2608.26411) | `stat.ME` | 2026-08-26

Applies marginal structural models with IPW to estimate the causal effect of continuous temperature on electricity demand under time-varying treatment-confounder feedback, where standard regression adjustment is biased. Introduces an outcome-adaptive and fused LASSO for weight model selection in continuous-treatment MSMs.

*Why relevant: Marginal structural models for continuous treatments under treatment-confounder feedback — important causal methodology demonstrated in a time-series setting.*

---

### Analyzing Within-Subject Experiments: Identification, Testing, and Sensitivity
**Shiyao Liu, Junni L. Zhang**
[arXiv:2608.26606](https://arxiv.org/abs/2608.26606) | `stat.ME` | 2026-08-27

Formalises a potential-outcomes framework for two-period within-subject (crossover) designs with heterogeneous treatment and carryover effects, characterises when pooling identifies the ATE (only when the gap in average carryover effects across sequences is zero), and provides a carryover sensitivity analysis.

*Why relevant: Causal identification conditions in experimental designs with carryover effects — relevant to interventional causal discovery and experimental design.*

---

## Conditional Independence Testing & Model Specification

### Approximating the null distribution of generalized distance covariance
**Dominic Edelmann**
[arXiv:2608.23793](https://arxiv.org/abs/2608.23793) | `math.ST`, `stat.ME` | 2026-08-24

Proves that the empirical spectra of doubly-centred distance matrices give a uniformly consistent approximation to the limiting null distribution of distance covariance (a weighted sum of chi-squares), rigorously justifying the spectral approximation already used informally for kernel-based independence tests and eliminating the need for expensive permutation testing.

*Why relevant: Directly strengthens the theoretical foundations of distance covariance / kernel independence testing — a key tool in the CI-testing toolkit.*

---

### Randomization tests for model specification in causal inference under network interference
**Supriya Tiwari, Pallavi Basu**
[arXiv:2608.22890](https://arxiv.org/abs/2608.22890) | `stat.ME` | 2026-08-24

Develops randomization-based tests for whether an analyst-chosen exposure mapping is correctly specified in network-interference settings (where Horvitz-Thompson estimators are sensitive to mapping misspecification), providing a principled model-checking step before spillover effect estimation.

*Why relevant: Model specification testing for causal estimators under network interference — connects CI/model testing ideas to causal estimation.*

---

## Interventions & Network Interference

### When Interference Graphs Evolve: Doubly Robust Estimation of Dynamic Peer Effects
**Xiaojing Du**
[arXiv:2608.27187](https://arxiv.org/abs/2608.27187) | `stat.ME` | 2026-08-27

Introduces a controlled contrast framework for peer effects when interaction graphs change after treatment assignment, distinguishing causal roles of pre-assignment history, dynamic peer exposure, and post-assignment network evolution. Derives a doubly robust estimator consistent if either the outcome model or propensity score model is correctly specified.

*Why relevant: Causal estimation of peer effects under evolving interference graphs — extends doubly robust methods to a realistic dynamic network interference setting.*

---

## Previous Digests

- [2026-W35](archive/2026-W35.md) — August 17 – 24, 2026 (18 papers)
- [2026-W34](archive/2026-W34.md) — August 10 – 17, 2026 (20 papers)
- [2026-W33](archive/2026-W33.md) — August 3 – 10, 2026 (11 papers)
- [2026-W32](archive/2026-W32.md) — July 27 – August 3, 2026
- [2026-W31](archive/2026-W31.md) — July 20 – 27, 2026
- [2026-W29](archive/2026-W29.md) — July 13 – 20, 2026
- [2026-W28](archive/2026-W28.md) — June 29 – July 6, 2026
- [2026-W27](archive/2026-W27.md) — June 22 – 29, 2026
- [2026-W26](archive/2026-W26.md) — June 15 – 22, 2026
- [2026-W25](archive/2026-W25.md) — June 8 – 15, 2026
