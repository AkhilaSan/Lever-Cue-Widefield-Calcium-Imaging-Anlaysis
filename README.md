Neural Predictors of Motor Skill Learning in Mice

This project analyzes a multimodal dataset (Kondo et al., 2025) to investigate the neural correlates of motor skill acquisition. 
By comparing "fast learners" and "slow learners," we identify specific brain regions that predict motor performance and learning outcomes.

Dataset Overview

Source: Kondo et al. (2025), Nature Scientific 
Data DOI: 10.1038/s41597-025-05482-yScope: 15 sessions over 2 weeks; 25 mice.
Task: Mice were trained to pull a lever to receive water rewards.
Key Phenomenon: By Day 5, the population naturally splits into two distinct cohorts: fast learners and slow learners.

Methodology

We focused on the calcium imaging data Delta F\F across all recorded brain regions for Day 1 and Day 5 of the experiment.
Signal Processing: We calculated the Area Under the Curve (AUC) for Delta F\F signals during the active movement window:
Start: pull_onset
End: The last lever pull before pull_onset + 0.4s (defined as movement_duration).

Statistical Modeling

We employed Linear Mixed Effects (LME) Models to account for inter-animal variability while testing two primary hypotheses:
Validation: Do activity levels in motor regions serve as significant predictors of actual pull durations?
Learning Prediction: Which brain regions predict the t_pull_final (the final mastered pull duration for a session)?

Key Findings

Retrosplenial Area (Lateral Agranular Part): Our model identified this region as a significant predictor of learning outcomes.
Hypothesis: The lateral agranular retrosplenial area plays a critical role in the transition from initial attempts to learned motor patterns, warranting further experimental investigation.
