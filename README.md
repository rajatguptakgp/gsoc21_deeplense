# GSoC'21 Evaluation Task: DeepLense
Evaluation Tasks for Google Summer of Code (GSOC) 2021

***
## Results

| Task | Metric | Value  |
| :---:   | :-: | :-: |
| 2 | AUC | 0.853 |
| 3 | Test MSE | 2.449 |
| 4 | AUC | 0.973 |

## Strategy

**Task 2:** Trained an autoencoder to learn embeddings for lensing images with no-substructure. An effectively trained model should be able to reconstruct the images without substructure through the constrained embedding space, but will struggle to reconstruct images with substructure, and hence, reconstruction loss can serve as an evaluation metric. Finally, with a range of thresholds on reconstruction loss, constructed the ROC curve and calculated AUROC.

**Task 3:** Trained a Multi-Layer Perceptron (MLP) to learn a mapping between images and halo mass using PyTorch. The model is ensured to be robust to overfitting by comparing **Validation MSE (2.469)** and **Test MSE (2.449)**.

**Task 4:** Trained a Multi-Layer Perceptron (MLP) for binary classification between images with and without substructure. Calculated True Positive Rate (TPR) and False Positive Rate (FPR) for a range of thresholds to construct ROC curve and calculated AUROC.
