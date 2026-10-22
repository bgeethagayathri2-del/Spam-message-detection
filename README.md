# Spam Message Detection

Classifies SMS messages as spam or ham (normal) using NLP and machine learning.

- **Dataset:** SMS Spam Collection (5,572 messages: 4,825 ham and 747 spam)
- **Method:** TF-IDF text features, then two models
- **Results:**

| Model | Accuracy |
|---|---|
| Naive Bayes | 0.970 |
| Logistic Regression | 0.968 |

- **Naive Bayes detail:**
  - Ham: precision 0.97, recall 1.00
  - Spam: precision 1.00, recall 0.78
- **Top spam words:** claim, prize, 150p, www, uk, tone, 18, guaranteed, 1000, cs
- **Conclusion:** Both models reached about 97% accuracy, and Naive Bayes was marginally ahead. The model never marked a normal message as spam (spam precision 1.00), but it missed about 1 in 5 spam messages (spam recall 0.78). This is partly because the data is imbalanced, with far more ham than spam. The top spam words (claim, prize, guaranteed, www) match what real spam looks like.

## How to run
Open `Spam_detection.ipynb` in Google Colab and click Run all.
