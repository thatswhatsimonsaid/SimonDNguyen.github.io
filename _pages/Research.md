---
title: "Research"
author_profile: true
redirect_from:
  - /talks.html
---

**Reinforcement Learning-Driven Active Learning for Regression** 

[Codebase](https://github.com/thatswhatsimonsaid/WeightedGreedySampling) [ArXiV](https://arxiv.org/abs/2603.10435)

Active learning for regression reduces labeling costs by selecting the most informative samples. Improved Greedy Sampling is a prominent method that balances feature-space diversity and output-space uncertainty using a static, multiplicative rule. We propose Weighted improved Greedy Sampling (WiGS), which replaces this framework with a dynamic, additive criterion. We formulate weight selection as a reinforcement learning problem, enabling an agent to adapt the exploration-investigation balance throughout learning. Experiments on 18 benchmark datasets and a synthetic environment show WiGS outperforms iGS and other baseline methods in both accuracy and labeling efficiency, particularly in domains with irregular data density where the baseline's multiplicative rule ignores high-error samples in dense regions.

**Aggregating Rashomon Sets for Robust Active Learning** 

[Codebase](https://github.com/thatswhatsimonsaid/RashomonActiveLearning) [ArXiV](https://arxiv.org/abs/2603.22750)

Active learning reduces labeling costs by selecting samples that maximize information gain. A dominant framework, Query-by-Committee (QBC), typically relies on perturbation-based diversity by inducing model disagreement through random feature subsetting or data blinding. While this approximates one notion of epistemic uncertainty, it sacrifices direct characterization of the plausible hypothesis space. We propose the complementary approach: Rashomon Ensembled Active Learning (REAL) which constructs a committee by exhaustively enumerating the Rashomon Set of all near-optimal models. To address functional redundancy within this set, we adopt a PAC-Bayesian framework using a Gibbs posterior to weight committee members by their empirical risk. Leveraging recent algorithmic advances, we exactly enumerate this set for the class of sparse decision trees. Across synthetic and established active learning baselines, REAL outperforms randomized ensembles, particularly in moderately noisy environments where it strategically leverages expanded model multiplicity to achieve faster convergence.

**Optimal full matching under a new constraint on the sharing of controls**

[Presentation](https://github.com/thatswhatsimonsaid/SimonDNguyen.github.io/blob/master/files/ICHPS_Presentation.pdf)

Health policy researchers are often interested in the causal effect of a medical
treatment in situations where randomization is not possible. Full matching on the
propensity score [(Gu & Rosenbaum, 1993)](https://www.tandfonline.com/doi/abs/10.1080/10618600.1993.10474623) aims to emulate random assignment by
placing observations with similar estimated propensity scores into sets with either one
treated unit and one or more control units or one control unit and multiple treated
units. Sets of the second type, with treatment units forced to share a comparison unit,
can be unhelpful from the perspective of statistical efficiency. The sharing of controls
are often needed to achieve experiment-like arrangements, but optimal full matching is
known to exaggerate the number of many-one matches that are necessary, generating
lopsided matched sets and smaller effective sample sizes [(Hansen, 2004)](https://www.tandfonline.com/doi/abs/10.1198/016214504000000647).

In this work, we introduce an enhancement of the [Hansen and Klopfer (2006)](https://www.tandfonline.com/doi/abs/10.1198/106186006X137047) optimal
full matching algorithm that counteracts this exaggeration by enabling analysis to
permit treatment units to share a control while limiting the number that are permitted
to do so. The result is a more well-balanced matching structure that prioritizes 1 : 1
pairs as opposed to matches with lopsided, many-to-one configurations of matched sets.
This enhanced optimal full matching is then illustrated in a pilot study on the effects of
Extracorporeal Membrane Oxygenation (ECMO) for treatment of pediatric acute
respiratory distress syndrome. Within this data-scarce pilot study, the existing methods
for limiting the sharing of controls have already resulted in an increased effective sample
size. The present enhancement of Hansen and Klopfer’s optimal full matching algorithm
provides an additional benefit to both effective sample size and covariate balance
