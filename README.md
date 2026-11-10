# Predict the Breach, Not the Drop: Control-Aligned Learning for Smoothing AI Training Power Swings

**Sayed Raheel Hussain** — Kayaan AI, New York, NY, USA — sayed@kayaan.ai

📄 **Paper (PDF):** [Hussain_PredictTheBreach_PESGM2027.pdf](Hussain_PredictTheBreach_PESGM2027.pdf)

> Status: submitted to the IEEE Power & Energy Society General Meeting 2027 (under review). This is the author's submitted version.

## Abstract
AI training jobs swing GPU power by tens of percent within a second, creating fast load ramps at grid-connected facilities. In an idealized simulation, fill-type smoothing reduces ramp-threshold violations but must be engaged before the fall, at a cost. The forecasting target matters. In a matched-pipeline ablation, a gradient-boosted classifier trained on the usual target, a large power drop, ranks violations poorly (average precision 0.58). Trained on the controller's own event, a violation inside the window a limiter armed now would cover, it reaches 0.96 on held-out H100 traces, against 0.67 for rhythm replay. With a validation-chosen threshold, the learned trigger removes 86.8% of test violations while engaged 45.6% of the time; rhythm replay must stay engaged 99.2%. Across three public datasets, learning significantly beats rhythm replay on two when the site is in the training data. Transfer to unseen sites is unreliable.

**Keywords:** Data centers, energy storage, load forecasting, machine learning, power smoothing

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
