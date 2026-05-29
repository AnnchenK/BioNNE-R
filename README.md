# BIONNE-R

This repository contains code for biomedical relation extraction in **English**, **Russian**, and **bilingual** settings.  
The task is formulated as **relation classification between pre-annotated entity pairs** in both gold-pair and blind-pair settings.

The project includes:
- data preprocessing and conversion,
- baseline experiments,
- completion-only fine-tuning of LLaMA-based models,
- log-probability inference,
- calibration of inference-time scores,
- experiments with entity markers, few-shot prompting, and hard negatives,
- error analysis and exploratory data analysis.

The model weights, along with the inference scripts, are located in the respective model folders: russian, english, and bilingual. The weights are split into four smaller blocks.

---

## Repository structure

```text
BIONNE-R/
├── bilingual/                   # bilingual model
├── data/                        # data files and intermediate processed files
├── english/                     # English-language model
├── russian/                     # Russian-language model
├── baseline.ipynb               # baseline data processing and model learning
├── calibration.ipynb            # score calibration and post-processing
├── data_analytics.ipynb         # corpus statistics and exploratory analysis
├── entity_markers.ipynb         # experiments with typed entity markers
├── few_shot_preprocessing.ipynb # preparation for few-shot prompting
├── hard_negatives.ipynb         # generation and analysis of hard negative samples
├── logprob_inference.ipynb      # log-probability-based inference
├── logprob_training.ipynb       # completion-only fine-tuning / training
└── README.md
