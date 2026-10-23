---
title: "On Pairwise Quantile Regression - Statistical Guarantees and Applications"
collection: publications
category: conferences
permalink: /publication/2026-08-18-on-pairwise-quantile-regression
excerpt: 'This article extends quantile regression to the pairwise case, establishing theoretical guarantees and proving fast learning rates using U-processes, with an application analyzing similarity score errors in facial recognition systems.'
date: 2026-08-18
venue: 'Conference on Uncertainty in Artificial Intelligence (UAI)'
#slidesurl: 'http://academicpages.github.io/files/uai2026_pairwise_quantile_slides.pdf'
paperurl: '/files/Therezien2026_Pairwise_Quantile_Regression.pdf'
bibtexurl: '/files/pairwise_quantile.bib'
citation: 'Therezien, R., Clémençon, S., Girard, F., & El-Abdouni, H. (2026). &quot;On Pairwise Quantile Regression - Statistical Guarantees and Applications.&quot; <i>Proceedings of the 42nd Conference on Uncertainty in Artificial Intelligence (UAI 2026)</i>, PMLR 337:6718-6739.'
use_math: true
mathjax: true
---

## Abstract

Quantile regression provides a powerful tool for summarizing the conditional distribution of a real-valued random variable of interest $$Y$$ as a function of covariates $$Z$$ in cases where it shows a large dispersion with high probability. This takes us beyond the situation where standard least-squares regression is informative or predictive. This article aims to extend this methodology to the pairwise case, when the variable to be explained takes the form of a similarity function between two independent observations (such as pixelated ID photos as input data of biometric systems) and the explanatory variables take the form of a pair of covariates of the observations, such as age or hair color. 

We establish theoretical guarantees for solutions of this statistical learning problem, considered here as empirical minimizers of a pairwise version of the pinball loss. Leveraging sharp concentration results for U-processes, we prove generalization bounds and identify mild conditions under which fast learning rates can be achieved. Confirming the probabilistic analysis, experiments based on simulation data also provide solid empirical evidence of the validity of the methodology promoted here for pairwise quantile regression. Finally, its usefulness from an application perspective is demonstrated by a detailed study aimed at analyzing errors in similarity scoring for facial recognition.

## Key Contributions

* **Methodological Extension:** Formulates pairwise quantile regression as the minimization of an empirical pinball loss averaged over all pairs of training observations (expressed as a U-statistic of order 2).
* **Fast Learning Rates:** Proves that the approach yields predictive functions capable of achieving fast "parametric" learning rates of order $$\mathcal{O}_{\mathbb{P}}(1/n)$$ up to a logarithmic factor under very mild conditions, outperforming the standard $$\mathcal{O}_{\mathbb{P}}(1/\sqrt{n})$$ rates typical of empirical processes.
* **Scalability:** Addresses computational burdens ($$\mathcal{O}(n^2)$$) by demonstrating that incomplete U-statistics (sampling a controlled subset of pairs) can offer a highly scalable alternative while maintaining critical theoretical guarantees.
* **Biometric Application:** Demonstrates practical value by deploying the framework on a real-world Facial Recognition dataset to analyze critical error boundaries—specifically looking into why impostor pairs return unusually high similarity scores or why genuine pairs return unusually low scores.

## Recommended Citation
If you find this research useful for your work, please use the citation text automatically appended below.