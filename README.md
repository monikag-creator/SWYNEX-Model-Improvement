# SWYNEX Model Improvement — Task 3

Internship task for SWYNEX Technologies: improve and validate the selected ML model.

## Base Model (from Task 2)
CNN — 88.7% accuracy

## Improvements Applied
- Data augmentation (random flip, rotation, zoom)
- Dropout (0.5) to reduce overfitting
- Lower learning rate (0.0005)

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| CNN (Original) | 0.887 | 0.897 | 0.887 | 0.888 |
| CNN (Improved) | 0.846 | 0.861 | 0.846 | 0.842 |

## Conclusion
The improved CNN scored lower within 15 epochs because dropout and augmentation 
are regularization techniques that trade short-term accuracy for better 
generalization. The original model showed overfitting signs (96.7% train vs 
88.7% val accuracy). The improved model's validation accuracy was still rising 
steadily at epoch 15, suggesting it would surpass the original with more 
training time.
