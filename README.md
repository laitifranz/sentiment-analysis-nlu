# Sentiment Analysis with PyTorch
This repository has been created for the Natural Language Understanding project course delivered during my Master's program.

## Introduction
This work performs sentiment analysis at document-level using the ``movie_reviews`` dataset, available in NLTK, to classify whether they are positive or negative reviews, known as polarity classification. As suggested by Bo Pang et al., removing subjectivity sentences from movie reviews ”can prevent the polarity classifier from considering irrelevant or even potentially misleading text”. For this reason, the ``subjectivity`` dataset, available in NLTK too, is used to train a subjectivity detector and filter out the ``movie_reviews`` dataset from objective sentences. For this project, I started with a probabilistic classifier and then moved to deep learning models to hopefully achieve better performance. I implemented a Naive Bayes-based approach used as baseline, then I implemented a GRU-based architecture using the Attention mechanism and pre-trained word embeddings, and finally a Transformers-based approach.

## Delivery contents
- Four Jupyter notebooks
  - [**statistics**](statistics.ipynb) contains the source code to extract statistics for ``subjectivity`` and ``movie_reviews`` datasets, available in the NLTK library;
  - [**multinomialNB**](multinomialNB.ipynb) contains the source code to build, train and evaluate a Naive Bayes-based sentiment analysis model using the scikit-learn library. Used as baseline;
  - [**gru**](gru.ipynb) contains the source code to build, train and evaluate a GRU-based sentiment analysis model using the PyTorch library;
  - [**transformers**](transformer.ipynb) contains the source code to import, fine tune and evaluate a Transformer-based sentiment analysis model using Hugging Face tools. BERT-based model used in this project.
- The [**report**](report.pdf) in pdf format that contains all the details of my implementation and the results obtained.