# Model Selection and L1-L2-Regularization with the Digits Dataset

This repository contains materials for a lab focused on exploring model selection and regularization techniques in machine learning. The main objective is to strengthen understanding of L1 and L2 regularization, as well as their impact on sparsity and model performance.

## Project Objective

The goal of this lab is to train a classifier capable of distinguishing between small digits (0 to 4) and large digits (5 to 9) using the Digits dataset from scikit-learn.

## Key Concepts Covered

- **L1 Regularization (Lasso):** Promotes sparsity by forcing some model coefficients to zero.
- **L2 Regularization (Ridge):** Shrinks the magnitude of coefficients without forcing them to zero.
- **Sparsity:** The proportion of model coefficients that are zero.
- **Model Selection:** The process of choosing a model from a set of candidate models.
- **Digits Dataset:** A dataset of handwritten digits.

## Results and Observations

The analysis of L1 and L2 regularization revealed notable differences in coefficient sparsity, but similar model performance in this specific case.

### L1 Regularization:
- Leads to high sparsity, meaning more coefficients are set to zero as the regularization strength (represented by decreasing `C`) increases.
- Observed sparsity ranged from **6.25% to 85.94%**.

### L2 Regularization:
- Maintains a constant sparsity of **4.69%**, regardless of the `C` value. This is because L2 regularization does not set coefficients to zero, but rather shrinks them.

### Model Performance:
- Despite significant differences in sparsity, model performance (score) remained identical (**0.10**) for both L1 and L2 regularization.
- This suggests that, in this particular scenario, coefficient sparsity had no significant impact on the overall model performance.

## Usage

To run the Jupyter notebook and reproduce the results:

1. Clone the repository (or download the `model_selection.ipynb` file).

2. Install the necessary dependencies (if not already installed):

   ```bash
   pip install scikit-learn matplotlib jupyter
