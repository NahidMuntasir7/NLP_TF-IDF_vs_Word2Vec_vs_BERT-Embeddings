# Sentiment Classification Project

This project compares three different text representation methods for sentiment analysis, **TF–IDF**, **Word2Vec**, and **BERT Embeddings** and all trained using a **Logistic Regression** classifier. The goal is to evaluate how different feature extraction techniques influence performance.

## Results Summary
| Method          | Test Accuracy | Test F1 | Training Time (s) |
|-----------------|---------------|---------|--------------------|
| TF–IDF + LR     | **0.8905**    | **0.8910** | 22.17 |
| Word2Vec + LR   | 0.8299        | 0.8295 | 43.23 |
| BERT Embeddings + LR   | 0.8236        | 0.8190 | 948.31 |

## Key Findings
- **TF–IDF + Logistic Regression** performed the best, achieving the highest accuracy and F1-score.
- **Word2Vec + Logistic Regression** gave moderate results. Averaging word vectors caused loss of contextual information.
- **BERT Embeddings + Logistic Regression** underperformed because only pre-trained embeddings were used without fine-tuning.
- More complex embeddings did **not** necessarily improve results — TF–IDF was both the most accurate and the fastest to train.

## What the Project Demonstrates
- Effects of classical vs. modern text representation methods.
- Performance comparison using consistent classification (Logistic Regression).
- Trade-off between accuracy, complexity, and computational cost.

## Conclusion
Even without deep model fine-tuning, traditional TF–IDF features combined with Logistic Regression can outperform more complex embedding-based methods. This provides a strong baseline for future improvements, such as fine-tuning BERT or adding neural network classifiers.
