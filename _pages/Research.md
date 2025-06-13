---
title: "Research"
author_profile: true
redirect_from:
  - /talks.html
---

**Aggregating Rashomon Sets for Robust Active Learning** 

[Paper/Presentation](https://neurips.cc/virtual/2024/98966)

Active learning's key task is selecting informative data points to enhance model predictions with a fixed labeling budget. However, when ensemble models such as random forests are used, there is a risk of the ensemble containing models with poor predictive accuracy or redundant trees with the same interpretation. To address this, we develop a novel approach to only ensemble the set of near-optimal models called the Rashomon set in order to guide the active learning process. We demonstrate how taking a Rashomon approach can not only improve the accuracy and rate of convergence of the active learning procedure, but also lead to improved interpretability compared to traditional approaches.

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
