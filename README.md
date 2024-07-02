# Comparative Analysis of Collaborative Filtering Algorithms on MovieLens 100K Dataset

## Overview

This repository contains the code, data, and report for the Project titled "Comparative Analysis of Collaborative Filtering Algorithms on MovieLens 100K Dataset". The project aims to explore and compare the performance of various collaborative filtering algorithms, specifically matrix factorisation and Transformer-based models, on the MovieLens 100K dataset.

## Table of Contents

- [Abstract](#abstract)
- [Introduction](#introduction)
- [Data](#data)
- [Methods](#methods)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Models](#models)
- [Limitations](#limitations)
- [Conclusion](#conclusion)
- [Usage](#usage)
- [Acknowledgements](#acknowledgements)

## Abstract

The report focuses on recommending interesting movies to users by comparing the performance of matrix factorisation methods and Transformer-based models. The comparison includes two matrix factorisation methods and three Transformer implementations to see how well they predict user ratings on the MovieLens 100K dataset.

## Introduction

The project aims to find the best recommendation system by:
1. Assessing the performance of traditional methods.
2. Comparing less intuitive techniques like Transformers with basic factorisation methods.
3. Investigating potential improvements to Transformer architecture.

The dataset used contains 100,836 ratings from 610 users on 9,742 movies.

## Data

The dataset used is the MovieLens 100K dataset, which includes:
- `ratings.csv`: User ratings for movies.
- `movies.csv`: Movie details.
- `tags.csv`: User-defined tags for movies.
- `links.csv`: Links to IMDb and TMDb.

## Methods

We used Python packages such as PyTorch, NumPy, Pandas, Statsmodels, WordCloud, Matplotlib, and Seaborn. The following methods were applied:
- **Matrix Factorisation**: Used for dimensionality reduction and finding latent matrices.
- **Transformers**: Utilised for their self-attention mechanism to find patterns in user-item interactions and temporal sequences.

## Exploratory Data Analysis

The exploratory data analysis section includes various plots such as histograms, line graphs, and cloud plots to provide insights into the dataset.

## Models

### Data Preprocessing

Data preprocessing involved merging datasets, encoding user and movie identifiers, and splitting the data into training and validation sets.

### Baseline Model

A baseline model using the median rating was created for performance comparison.

### Matrix Factorisation

Two models were implemented:
1. **Without Bias Terms**: Basic matrix factorisation.
2. **With Bias Terms**: Matrix factorisation with user and item bias terms.

### Transformers

Three Transformer models were created with different embeddings:
1. **Model 1**: User and movie embeddings.
2. **Model 2**: User, movie, and rating history embeddings.
3. **Model 3**: User, movie, rating history, and movie genre embeddings.

## Limitations

The limitations include:
- Linearity assumptions in matrix factorisation.
- Handling of sparse data.
- Cold-start problem.
- Complexity and interpretability issues with Transformer models.
- Computational resource requirements.

## Conclusion

The project concluded that Transformer-based models offer higher predictive accuracy than matrix factorisation models. The inclusion of bias terms and sequential data improves predictive performance. Future research may explore hybrid models that combine the strengths of both methodologies.

## Acknowledgements

We acknowledge the use of GPT-4 (OpenAI) and Meta-Llama-3-70B for checking grammar, proofreading, and providing explanations on SGD factorisation and attention mechanisms. These tools also helped in editing plot margins and debugging data preprocessing and PyTorch training loops.

For more details, refer to the full report included in the repository.

---
