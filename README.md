# Reproducing and Analyzing DistilBERT for COVID-19 Health Sentiment

## Overview
This repository contains the code and dataset used in the paper:

"Reproducing and Analyzing DistilBERT for COVID-19 Health Sentiment:
A Statistical Evaluation of Model Performance"

The study reproduces the DistilBERT-based sentiment classification framework
proposed by Jojoa et al. (2022) and evaluates its performance on a larger,
noisier, five-class COVID-19 Twitter dataset. A small fine-tuning modification
is introduced to assess model stability and convergence under increased
classification complexity.

## Dataset
- Domain: Health-related COVID-19 tweets
- Language: English
- Task: Five-class sentiment classification
- Raw data: provided as separate training and testing files
- Processed data: combined for preprocessing and re-split for experiments

Detailed dataset information is provided in `data/README.md`.

## Methodology
- Models:
  - Baseline: BERT (bert-base-uncased)
  - Modified: DistilBERT (distilbert-base-uncased)
- Framework: Hugging Face Transformers
- Training:
  - supervised fine-tuning
  - cross-entropy loss
  - AdamW optimizer
- Modification:
  - extended fine-tuning to five epochs
  - adjusted learning rate for stable convergence

## Code
All experiments are implemented in a single Jupyter notebook:

`notebook/FP_SML.ipynb`

The notebook includes:
- data preprocessing
- transformer fine-tuning
- evaluation metrics and confusion matrix analysis
- statistical interpretation of results

## Reproducibility
Install dependencies:
```bash
pip install -r requirements.txt
