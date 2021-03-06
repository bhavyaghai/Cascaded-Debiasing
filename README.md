# Cascaded Debiasing: Studying the Cumulative Effect of Multiple Fairness-Enhancing Interventions

- ### Read paper [PDF](https://arxiv.org/abs/2202.03734)

## Overview

Understanding the cumulative effect of multiple fairness enhancing interventions at different stages of the machine learning (ML) pipeline is a critical and underexplored facet of the fairness literature. For example, one might choose to debias the dataset, train a fairness aware classifier over it and then post-process the model's predictions to achieve more fairness. This paper takes the first step in exploring this area by undertaking an extensive empirical study comprising 60 combinations of interventions, 9 fairness metrics, 2 utility metrics (Accuracy and F1 Score) across 4 benchmark datasets. We quantitatively analyze the experimental data to measure the impact of multiple interventions on fairness, utility and population groups.

## Key Findings

- Applying multiple interventions results in better overall fairness and lower utility than individual interventions on aggregate.
- Adding more interventions do no always result in better fairness or worse utility.
- The likelihood of achieving high performance (F1 Score) along with high fairness increases with larger number of interventions.
- Fairness-enhancing interventions can negatively impact different population groups, especially the privileged group.
- This study also highlights the need for new fairness metrics that account for the impact on different population groups apart from just the disparity between groups.
- We offer a list of combinations of interventions that perform best for different fairness and utility metrics to aid the design of fair ML pipelines.

## Code Overview

All the code resides in 4 jupyter notebooks. The notebook titled 'Conduct All Interventions' contains the code for conducting all the simulations/experiments and recording the experimental data. The other 3 notebooks contains analysis on the experimental data to answer different research questions. All the experiemntal data for different datsets can be found in the data folder. For my system, fairlearn version 0.4.6 worked and not the lastest version (0.7.0).

## Citation

```
@article{ghai2022cascaded,
  title={Cascaded Debiasing: Studying the Cumulative Effect of Multiple Fairness-Enhancing Interventions},
  author={Ghai, Bhavya and Mishra, Mihir and Mueller, Klaus},
  journal={arXiv preprint arXiv:2202.03734},
  year={2022}
}
```

Feel free to email me for any questions, comments at bghai@cs.stonybrook.edu
