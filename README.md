# Predict the Breach, Not the Drop: Control-Aligned Learning for Smoothing AI Training Power Swings

**Sayed Raheel Hussain** — Kayaan AI, New York, NY, USA — sayed@kayaan.ai

📄 **Paper (PDF):** [Hussain_PredictTheBreach_PESGM2027.pdf](Hussain_PredictTheBreach_PESGM2027.pdf)

> Status: submitted to the IEEE Power & Energy Society General Meeting 2027 (under review). This is the author's submitted version.

## Abstract
Large AI training jobs can swing GPU power by tens of percent within a second, and synchronized jobs can create fast load ramps of concern at large grid-connected facilities. In an idealized simulation, fill-type smoothing, using filler GPU work or storage, can reduce violations of an illustrative ramp threshold, but it must be engaged before the fall and keeping it engaged has a cost. Forecasting can decide when to engage it. We find that the choice of training target matters substantially. In a matched-pipeline ablation, a gradient-boosted classifier trained on the usual target, "a large power drop is coming", ranks the violations a ramp limiter must catch poorly (average precision 0.58). Trained on the controller's own event, "a ramp-limit violation will occur while a limiter armed now would be armed", the same pipeline reaches 0.96 (difference 95% CI 0.28 to 0.49) on held-out H100 training and inference traces, against 0.67 for no-learning rhythm replay of the same target. With a threshold chosen on validation for a 90% removal target, the learned trigger removes 86.8% of test violations with the actuator engaged 45.6% of the time, while rhythm replay meets the target only by staying engaged 99.2% of the time, i.e. effectively always on. Across three public datasets covering H100, B200 and V100 nodes and both benchmark and labelled cluster jobs, the learned trigger has significantly higher AP than rhythm replay on two datasets when that site is in the training data, after harmonizing sensor averaging; the third is inconclusive. Transfer to an unseen site is unreliable, which we report as an open problem.

**Keywords:** data centers, AI workloads, ramp rate, load forecasting, power smoothing, energy storage

## Contents
- `Hussain_PredictTheBreach_PESGM2027.pdf` — the paper (4 pages, IEEE conference format)
- `latex/` — LaTeX source and figures (`main.tex`, compile with pdfLaTeX/tectonic)

## Citation
```bibtex
@misc{hussain2026predictthebreach,
  author = {Sayed Raheel Hussain},
  title  = {Predict the Breach, Not the Drop: Control-Aligned Learning for Smoothing AI Training Power Swings},
  year   = {2026},
  note   = {Submitted to IEEE PES General Meeting 2027},
  howpublished = {\url{https://github.com/sayedRaheel/predict-the-breach}}
}
```

## AI-use disclosure
Per IEEE policy, the paper's Acknowledgment discloses AI assistance (Claude, Anthropic; Codex, OpenAI; Kimi, Moonshot AI). The author designed the study, checked all code, data and results, and is responsible for the content.

## License
© 2026 Sayed Raheel Hussain. All rights reserved. If the paper is accepted, IEEE copyright terms will apply to the published version.
