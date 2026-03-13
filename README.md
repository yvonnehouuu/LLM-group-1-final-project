# LLM-group-final-project
**LLM-Based Toxic Comment Classification Project**

This project explores **toxic comment classification using Large Language Models (LLMs)**.  We evaluate the effectiveness of **zero-shot and few-shot prompting strategies** for detecting toxic content in text.

The goal of this project is to investigate how well modern LLMs can perform text classification tasks without traditional model training.



## Project Overview

Online platforms face increasing challenges with toxic and harmful comments.  
Traditional machine learning approaches require large labeled datasets and training pipelines.

This project instead explores:

- Zero-shot prompting
- Few-shot prompting
- Prompt-based classification using LLMs

to classify whether a comment is **toxic or non-toxic**.



## Methodology

The project evaluates different prompting strategies:

* **Zero-Shot Classification**

  The model classifies comments without seeing any labeled examples.

* **Few-Shot Classification**

  The model is provided with a small number of labeled examples in the prompt to guide classification.

* **Multiple Random Seeds**

  Experiments are repeated with different seeds to observe performance stability.



## Project Structure
```
.
├── data/ # Dataset samples
├── zero_test_predictions_*.csv # Zero-shot prediction results
├── few_test_predictions_*.csv # Few-shot prediction results
├── train_zero_predictions.csv
├── train_few_predictions.csv
├── LLM Group final.ipynb # Main experiment notebook
├── vidualisation.py # Visualization and analysis
└── README.md
```


## Dataset
**Jigsaw Toxic Comment Classification Dataset**

**Source**: Kaggle / HuggingFace

**Size**: ~159,000 annotated comments from Wikipedia

**Labels (multi-label)**: toxic, severe_toxic, obscene, threat, insult, identity_hate

**Download**: https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data


## Experiments

We compare:

- Zero-shot prompting
- Few-shot prompting

Across different random seeds to analyze:

- Prediction accuracy, macro f1, hamming loss, precision, recall
- Stability across runs
- Performance differences between prompting methods



## Results

Results are stored as CSV files containing:

- Model predictions
- Ground truth labels
- Evaluation subsets

These files allow further analysis and visualization of model performance.



## Technologies Used

- Python
- Jupyter Notebook
- Large Language Models (LLMs)
- Pandas
- Data Visualization (matplotlib, seaborn)


