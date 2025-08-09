# 🏷️ Arabic Title Generator using AraT5

This project fine-tunes the `UBC-NLP/AraT5-base` model on a custom Arabic dataset to generate titles from documents using the Hugging Face Transformers library.

## 📦 Requirements

Install the required libraries:

```
pip install transformers accelerate nltk datasets regex scikit-learn sentencepiece protobuf fairscale sacrebleu rouge_score
```
---
## How to Run
You can either run the code in a Jupyter Notebook or Google Colab, or convert the cells into a Python script. Here's a sample outline of what the script does:

Install dependencies

Download training script from the AraT5 GitHub repo

Fine-tune the model using your dataset

Evaluate and generate predictions

##📂 Dataset
---
You need two files in .tsv format:

ARGEn_title_genration_sample_train.tsv

ARGEn_title_genration_sample_valid.tsv

Each file should have at least two columns:

document: The input text

title: The expected generated title

##📊 Evaluation
---
Evaluation metrics include:

BLEU Score (using sacrebleu)

ROUGE Score (using rouge_score)


