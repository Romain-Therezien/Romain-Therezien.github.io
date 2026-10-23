---
title: "Epistemic Uncertainty in Assessing Fairness for Similarity-Learning"
collection: publications
category: conferences
permalink: /publication/2026-10-23-epistemic-uncertainty-fairness-similarity-learning
excerpt: 'This work quantifies the uncertainty of fairness metrics in similarity learning when the operating point is estimated from the evaluation data. Representing subgroup error rates as ratios of U-statistics, it derives asymptotic distributions and valid confidence intervals under complete, incomplete and stratified pair designs, covering how real-world benchmarks are built, with experiments on face and speaker verification.'
date: 2026-10-23
status: under-review
#citation: 'Therezien, R., et al. (2026). &quot;Epistemic Uncertainty in Assessing Fairness for Similarity-Learning.&quot; <i>Under review</i>.'
use_math: true
mathjax: true
---

*This paper is currently under review. A preprint will be made available soon.*

## Abstract

In similarity learning, decisions are based on comparing pairs of observations using a similarity score. In this context, fairness is typically assessed by comparing error rates across different sensitive groups at a fixed operating point, and the resulting metrics are usually presented as point estimates, without accounting for the uncertainty associated with the finite nature of the evaluation data.

We develop a framework for quantifying this uncertainty when the operating point itself is estimated from the evaluation data. By exploiting the representation of subgroup error rates as ratios of U-statistics, we derive their joint asymptotic distribution at the estimated operating point. This yields asymptotic distributions and confidence intervals for a broad class of fairness metrics, including non-smooth measures based on extremes. We extend the analysis to incomplete pair designs, taking into account the additional variability induced by pairwise sampling. Experiments on facial recognition and speaker verification demonstrate how this uncertainty affects fairness comparisons between models.

## Key Contributions

* **Joint Asymptotics at the Estimated Threshold:** Establishes the joint asymptotic distribution of subgroup error rates (FAR/FRR), written as ratios of U-statistics, at an operating point calibrated on the same evaluation data, and shows that threshold estimation modifies their covariance through a common term.
* **Smooth and Non-Smooth Fairness Metrics:** Derives the asymptotic distribution of a broad class of fairness metrics, including those based on extrema such as the max-min ratio, whose limit is not Gaussian when subgroups are tied (e.g., under perfect fairness).
* **Incomplete Pair Designs:** Extends the results to incomplete pair designs, including the stratified fixed-pair lists used in standard benchmarks, accounting for the additional randomness induced by pair sampling.
* **Valid Confidence Intervals:** Proves the validity of a bootstrap procedure adapted to pairwise data and constructs confidence intervals that remain valid in the presence of ties between subgroups.
* **Applications:** Shows on facial recognition and speaker verification that some fairness differences between models are supported by the data, while others are not.

## Recommended Citation
If you find this research useful for your work, please use the citation text automatically appended below.
