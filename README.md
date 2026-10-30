# Airline Customer Experience NLP

Natural-language-processing project analysing airline customer reviews using **sentiment analysis** and **topic modelling** to identify recurring customer-experience themes.

## Project overview

This project was completed for Advanced AI for Business at Deakin University. It applies NLP techniques to unstructured airline-review text and translates model outputs into interpretable customer-experience insights.

The analysis includes comparisons involving Qantas and Jetstar and investigates differences across airline, cabin and service-related dimensions where available in the source data.

## Analytical workflow

The notebook covers:

1. Review-data preparation and exploratory analysis.
2. Text preprocessing.
3. Tokenisation and stop-word handling.
4. Lemmatization.
5. VADER sentiment scoring.
6. Sentiment classification and aggregation.
7. LDA topic modelling with Gensim.
8. Topic-coherence analysis.
9. Interpretation and visualisation of recurring customer-experience themes.

## Technology

- Python
- pandas
- NumPy
- NLTK
- VADER
- Gensim
- Latent Dirichlet Allocation (LDA)
- Matplotlib
- Seaborn
- WordCloud
- Jupyter Notebook

## Methods

### Sentiment analysis

VADER was used to derive sentiment scores from customer-review text. The analysis then aggregated and compared sentiment across relevant airline/customer-experience categories.

### Topic modelling

After preprocessing the review text, LDA topic modelling was used to identify latent themes appearing across the review corpus. Topic coherence was used as part of the topic-model assessment process.

## Repository structure

```text
.
├── README.md
├── requirements.txt
└── notebooks/
    └── airline_nlp_analysis.ipynb
```

## Reproducibility

The notebook is preserved from the original university analysis. A fresh run may require the original source dataset and installation/download of the NLTK resources used by the notebook.

This repository intentionally does not claim production deployment or predictive-model accuracy: the project is an applied NLP analysis focused on sentiment, topic discovery and business interpretation.

## Portfolio context

The project demonstrates an end-to-end applied NLP workflow: converting unstructured customer feedback into structured sentiment measures and recurring themes that can support customer-experience analysis.

A BI/dashboard layer may be added separately in the future for analyst-focused portfolio use; it is not required to understand the NLP work contained here.

## Limitations

- VADER is lexicon-based and can miss domain-specific nuance, sarcasm and context.
- LDA topics require human interpretation and can vary with preprocessing and modelling choices.
- Findings depend on the composition and representativeness of the review dataset.
- This is an analytical research/portfolio workflow, not a deployed production NLP service.
