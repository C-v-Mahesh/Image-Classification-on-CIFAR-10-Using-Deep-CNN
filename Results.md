# 📊 Experimental Results

This section highlights the outcomes of our CNN-based image classification model trained on the CIFAR-10 dataset. The results show a clear performance advantage of our deep learning model over traditional machine learning approaches.

---

## ✅ Final Performance Metrics (CNN)

| Metric         | Value     |
|----------------|-----------|
| Test Accuracy  | **74.7%** |
| Test Loss      | **0.26**  |
| Best Accuracy (Paper) | **88.0%** |

> ⚠️ Note: The paper model achieved 88% accuracy with advanced tuning. The base code here achieves ~74.7%.

---

## 🧪 Accuracy vs Loss Graphs

**Training vs Validation Accuracy**

![Accuracy](results/accuracy_plot.png)

**Training vs Validation Loss**

![Loss](results/loss_plot.png)

---

## 📌 Confusion Matrix

The confusion matrix below shows model predictions versus actual labels for the test dataset.

![Confusion Matrix](results/confusion_matrix.png)

- Strong performance on classes like `Ship`, `Frog`, `Automobile`
- Misclassifications between similar-looking categories like `Cat`, `Dog`, and `Deer`

---

## 🔍 Sample Predictions

Here are 15 test images with predicted and actual labels:

![Predictions](results/sample_predictions.png)

- **Blue titles** indicate correct predictions
- **Red titles** indicate incorrect predictions

---

## 🔁 Comparison with Traditional ML Models

| Model            | Accuracy (%) | Test Loss (%) |
|------------------|--------------|----------------|
| SVM (Linear)     | 36           | 44             |
| SVM (Polynomial) | 40           | 42             |
| HOG              | 40           | 50             |
| KNN              | 34           | 66             |
| **CNN (This Work)** | **74.7**     | **26**         |

---

## 📌 Observations

- CNN significantly outperforms traditional models due to its ability to extract hierarchical spatial features.
- Data augmentation and dropout effectively reduce overfitting.
- Early stopping improves generalization without excessive training.

---

## 📈 Room for Improvement

- Hyperparameter tuning (learning rate, batch size)
- Deeper CNN with residual connections (e.g., ResNet)
- Transfer learning with pre-trained weights

---


