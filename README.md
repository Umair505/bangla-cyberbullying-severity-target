# Bangla Cyberbullying Severity and Target Classification

This project predicts the severity and main target of a Bangla comment.

## Tasks

Each comment receives one label for each task.

| Code | Severity | Target |
|------|----------|--------|
| 0 | Neutral | No Target |
| 1 | Mild | Individual |
| 2 | Moderate | Group |
| 3 | Severe | Community |

## Dataset

The working dataset contains 5,858 unique Bangla comments.

The dataset has five columns.

- text
- Description
- Original_Label
- Final_Severity
- Final_Target

The models use the cleaned text as input.

The data split contains 4,103 training comments,
878 validation comments and 877 test comments.
Duplicate groups are kept within the same split.

## Methods

We compare the following methods.

- TF-IDF with linear classifiers
- BanglaBERT
- XLM-R
- Multilingual BERT
- Single-task and multi-task learning
- Soft voting, weighted voting and stacking

We use SHAP and LIME to study which words affect
the shared BanglaBERT model.

## Evaluation

Models are selected using validation macro-F1.

We report accuracy, macro-F1, class-level scores,
joint prediction accuracy and label agreement.

The annotation records contain three label sets.
Their agreement and label sources are described in the paper.

## Files

- notebooks/ contains the model notebooks.
- paper/ contains the LaTeX source and compiled paper.
- figures/ contains the figures as PDF files.
- results/ contains the evaluation tables.
- requirements.txt lists the Python dependencies.

## Authors

- Mohammad Moinul Islam
- Mohammad Junaidul Haque

## Supervisor

Antu Chowdhury

Department of Computer Science and Engineering
East Delta University, Chattogram, Bangladesh
