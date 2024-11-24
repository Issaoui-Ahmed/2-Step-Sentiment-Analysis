# Sentiment Analysis with 2-Step Classification

This project explores a novel approach to sentiment analysis using a **2-step classification method**. The focus is on addressing the challenge of neutrality, which is difficult to classify due to its lack of distinct patterns. The approach is demonstrated on a dataset of tweets in Algerian Arabic, highlighting the potential of breaking down sentiment into separate evaluations of positivity and negativity.

---

## Overview

Sentiment analysis models typically classify text as positive, negative, or neutral in a single step. However, neutrality is not a detectable pattern—it is inferred from the absence of strong positivity or negativity. This project proposes a **2-step classification approach** that evaluates these components separately:
1. **Positivity Detection**: Determine how positive the text is.
2. **Negativity Detection**: Determine how negative the text is.

By combining the results of these evaluations, neutrality can be inferred when both positivity and negativity scores are low. This method mimics human reasoning and provides more accurate results, especially for ambiguous or noisy text.

Key aspects of the project:
- **Preprocessing**: The dataset of tweets is cleaned and normalized, including stopword removal, emoji handling, and tokenization.
- **Embedding Models**: The project leverages pretrained embeddings such as **AraVec** and **DziriBERT** for robust text representations.
- **2-Step Classification**: Independent models for positivity and negativity classification are combined for final sentiment prediction.

---

## Features

- **Innovative Approach**: The 2-step classification method offers a fresh perspective on handling neutrality in sentiment analysis.
- **Low-Resource Focus**: The dataset consists of ~1,600 tweets in Algerian Arabic, demonstrating the feasibility of this approach in low-resource settings.
- **LSTM Models**: The project employs LSTM-based architectures, enhanced with contextual embeddings, to capture sentiment nuances.

---

## Results

The experiments compared traditional single-step sentiment analysis with the proposed 2-step method. The results showed:
- **Baseline Performance**: Models such as Naive Bayes and Logistic Regression achieved accuracies around 50–54%.
- **LSTM with AraVec**: Improved performance to 63%.
- **2-Step Classification**: Achieved **70% accuracy**, outperforming the baselines and offering better handling of neutrality.

---

## Key Takeaways

1. **Handling Neutrality**: The 2-step approach demonstrates how breaking down sentiment into smaller, interpretable components can improve performance on challenging tasks.
2. **Low-Resource Feasibility**: This project highlights how innovative methods can work effectively, even with small and noisy datasets.
3. **Broader Applications**: While this project focuses on sentiment analysis, the methodology can be adapted for other nuanced classification problems.

---

## Future Directions

1. **Larger Datasets**: Expanding the dataset to include more diverse and balanced samples would further validate the approach.
2. **Transformer Models**: Exploring transformer-based architectures like BERT could enhance the model’s understanding of context and subtlety.
3. **Generalization**: Applying the 2-step classification framework to other languages or classification tasks could showcase its versatility.

---

This project represents a meaningful exploration of how to rethink sentiment analysis by addressing its most persistent challenge: neutrality.
