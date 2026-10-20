# Comparative Analysis of POS Tagging: Standard Italian vs. CMC

## Project Overview
This repository contains a Computational Linguistics project focused on evaluating the performance of a pre-trained Natural Language Processing (NLP) model on the task of Part-of-Speech (POS) Tagging for the Italian language.

Specifically, the project compares the automated output of the **SpaCy** model (`it_core_news_md`) across two contrasting linguistic registers: standard academic Italian and Computer-Mediated Communication (CMC) characterized by informal language, abbreviations, and non-standard syntax. The system's output is compared against a manually annotated Gold Standard to perform a qualitative and quantitative error analysis.

## Repository Structure
* **`NLP_POS_Tagging_Linguistica_Computazionale_Elisabetta_Pellegrini.ipynb`**: The Python codebase (Google Colab notebook) containing the data pipeline, model execution, and evaluation scripts.
* **`Annotazione_POS_Tagging.xlsx` & `Annotazione2_POS_Tagging.xlsx`**: The manual Gold Standard datasets containing human annotations based on the Universal Dependencies (UPOS) tagset.
* **`Paper Linguistica Computazionale.pdf`**: The final academic paper detailing the methodology, the calculated metrics (Accuracy, Precision, Recall, Weighted F1-Score), and the qualitative Error Analysis.
* **Images (`.png`)**: Visualizations of the Confusion Matrices and Inter-Annotator Agreement (Cohen's Kappa) heatmaps.

## Methodology
1. **Data Selection**: Extraction of two text samples representing formal academic language and informal student chat (CMC).
2. **Manual Annotation**: Creation of a human-annotated Gold Standard using UPOS tags, evaluated via Inter-Annotator Agreement (IAA).
3. **Automated Tagging**: Processing the raw texts through the SpaCy NLP pipeline.
4. **Evaluation**: Calculating IAA using Cohen's Kappa score, and measuring the model's performance via `scikit-learn` (Accuracy, Classification Report, Confusion Matrices).

## Tools & Libraries Used
* **Python** (Google Colab)
* **SpaCy** (NLP Pipeline)
* **Pandas** (Data manipulation)
* **Scikit-learn** (Evaluation metrics)
* **Matplotlib & Seaborn** (Data visualization)
