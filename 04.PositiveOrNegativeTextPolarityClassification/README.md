# Sentiment Classification Competition

## Description

This competition challenges participants to classify a piece of text as either positive or negative. The classification is not strictly defined, as texts may contain mixed sentiments. The goal is to discern the overall sentiment based on the tone of the text's conclusion. The competition is designed to mirror real-world conditions where labeled data is scarce but the need for classification is crucial. Participants must work individually.

## Approach

### Introduction

- Focus on sentiment analysis using Natural Language Processing (NLP), a key technology in social media analysis, brand monitoring, and market research.

### Technology Overview

- **Machine Learning Methods**: Use of traditional algorithms like SVMs and Random Forests with extensive feature engineering.
- **Deep Learning Methods**: Adoption of deep neural networks, including CNNs, RNNs, and Transformer-based models like BERT, GPT, and RoBERTa, which offer superior context and semantic understanding.

### Application Scenarios

- Monitoring social media, analyzing customer feedback, and predicting financial market trends through sentiment analysis.

### Dataset

- Contains 2000 entries with three fields: `row_id` (unique identifier), `TEXT` (text for analysis), and `LABEL` (sentiment label, where '1' is positive and '0' is negative).

### Methods

#### Data Preprocessing

- Convert text to lowercase, remove punctuation and extra spaces, and prepare data for BERT tokenization to enhance processing and understanding.

#### Model Training

- **Optimizer**: Adam
- **Learning Rate**: 2e-5
- **Batch Size**: 32
- **Epochs**: 4
- **Loss Function**: Cross-Entropy Loss
- **Regularization**: Early Stopping to prevent overfitting and conserve resources.

### Results and Future Work

- Achieved an accuracy of 85% on the validation set.
- Future improvements might include more advanced data augmentation and preprocessing techniques, and exploring different model architectures.

## Conclusion

- The model successfully predicted text sentiment with a public test data score of 0.74159. Areas for improvement include refining early stopping criteria and validation set selection to enhance model performance and reliability.
