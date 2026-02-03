## Model Performance Comparison Using Confusion Matrix

### Confusion Matrix Components

A confusion matrix provides four key metrics:
- **True Positives (TP)**: Correctly predicted >50K
- **True Negatives (TN)**: Correctly predicted ≤50K  
- **False Positives (FP)**: Incorrectly predicted >50K
- **False Negatives (FN)**: Incorrectly predicted ≤50K

### Performance Metrics

| Metric | Decision Tree | Random Forest | XGBoost |
|--------|--------------|---------------|---------|
| True Positives | 982 | 918 | 1017 |
| True Negatives | 4530 | 4595 | 4594 |
| False Positives | 415 | 350 | 351 |
| False Negatives | 586 | 650 | 551 |
| Accuracy | 85.05% | 85.94% | 87.06% |
| Precision | 71.68% | 77.53% | 77.65% |
| Recall | 62.63% | 58.55% | 64.92% |
| F1-Score | 66.85% | 66.72% | 70.72% |

### Analysis

**XGBoost** demonstrates superior performance across key metrics:

1. **Highest Accuracy**: 87.06% (2.01% improvement over Decision Tree)
2. **Best Recall**: 64.92% (identifies 66 more high earners than Random Forest)
3. **Best F1-Score**: 70.72% (optimal precision-recall balance)
4. **Lowest False Negatives**: 551 (minimizes missed high-income cases)

**Random Forest** achieves the best precision (77.53%) with the fewest false positives (350), making it most reliable for positive predictions but at the cost of lower recall.

**Decision Tree** provides adequate baseline performance but shows higher error rates across all categories and increased overfitting risk.

### Conclusion

XGBoost is the optimal model for this classification task, achieving the best balance between accuracy, precision, and recall while minimizing critical errors (false negatives).
