# Predictive Machine Learning Models

## Overview
This repository contains Python implementations of three machine learning tasks completed as part of my MSc Data Analytics coursework. Each task was applied to a real analytical problem, with findings that have practical business relevance.

## Tasks & Key Findings

### Task 1: Decision Tree Classification — Wine Purchasing Decisions
Built a decision tree classifier to predict whether a customer would buy a wine based on price, type, characteristics, and origin.

**What I found:** The model identified that wine type and price were the strongest predictors of purchasing decisions. The dataset was balanced (5 buy, 5 not-buy), and the tree achieved clean splits using entropy-based information gain — suggesting these features genuinely separate the two classes rather than reflecting noise.

**Why it matters:** For a retailer or distributor, knowing which product attributes drive purchase decisions enables smarter stocking, pricing, and promotional strategies.

### Task 2: K-Means Clustering — Customer/Product Segmentation
Applied K-Means clustering to a four-feature dataset, using the elbow method to determine the optimal number of clusters (k=3).

**What I found:** Three distinct groups emerged with meaningfully different feature profiles. The cluster centroids (returned to original scale) showed clear separation across all four features, confirming the segments are not arbitrary — they reflect genuine patterns in the data.

**Why it matters:** Segmentation like this underpins targeted marketing, personalised recommendations, and resource allocation. Knowing that three distinct groups exist (rather than one homogenous population) changes how you approach each group.

### Task 3: Polynomial Regression — Portfolio Returns vs Risk
Modelled the relationship between a risk factor and portfolio returns using polynomial regression (degree 2), rather than assuming a simple linear relationship.

**What I found:** The model achieved an R² of 0.37, meaning risk explains roughly 37% of the variation in returns. The non-linear fit captured a curved relationship — returns do not simply rise or fall with risk in a straight line. MSE was 0.28, indicating moderate prediction error given the spread of the data.

**Why it matters:** A 37% R² in financial return modelling is meaningful — markets are noisy, and a single risk variable will never fully explain returns. The finding confirms that risk is a relevant but incomplete predictor, which is exactly what portfolio theory would suggest.

## Tools & Libraries
- Python, Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn (DecisionTreeClassifier, KMeans, LinearRegression, PolynomialFeatures)

## Context
Academic coursework completed as part of the MSc Data Analytics programme.
