House Price Prediction Competition Winner

## Overview

This README documents the process and results of the House Price Prediction Competition, hosted on Kaggle by Prof.xu, where we secured the first place. The competition focused on predicting the selling prices of house properties in Denver using a multilayer perceptron network. The challenge emphasized the construction of the network from scratch, prohibiting the use of pre-existing models or frameworks outside of the multilayer perceptron design.

## Competition Description

The real estate market is typically characterized by high stakes, significant time investment, and stress, often lacking transparency. Both buyers and sellers engage in this major financial decision with various uncertainties. Accurate price estimation is crucial for buyers to assess property values and for sellers to set competitive yet profitable prices.

In this competition, our task was to build and train a multilayer perceptron model to predict house selling prices effectively. The dataset provided was the "Denver Dataset," featuring a range of house properties with diverse attributes.

## Our Approach

### Data Preparation and Analysis

We started by analyzing and visualizing the Denver Dataset, focusing on sale prices, their distribution, and correlation with other features. The dataset included 11,581 training samples and 4,964 test samples, each with 16 different features.

Key steps in data preparation included:

- Splitting the data into training and validation sets.
- Normalizing sale prices for faster training convergence.
- Handling non-numeric features through one-hot encoding.
- Standardizing features and imputing missing values.

### Model Development

Our approach involved experimenting with various multilayer perceptron architectures, including:

1. A base model with 2 hidden layers (256 and 128 neurons).
2. A model with 4 hidden layers (512, 256, 128, and 64 neurons).
3. The inclusion of norm regularization and dropout layers to prevent overfitting.

Each model iteration was evaluated using training and validation error plots, and the best-performing model was selected based on the validation error.

### Hyperparameter Tuning

We conducted extensive hyperparameter tuning to optimize the model's performance. This process included adjusting learning rates, epochs, and weight decay parameters. The optimal set of hyperparameters was determined through dynamic learning rate adjustments and early stopping criteria.

### Training and Validation

Models were trained using GPU acceleration. We employed mean-squared loss for training and median error rate (MER) as the performance metric. The training process involved monitoring both training and validation losses to avoid overfitting and to select the best-performing model iteration.

### Final Submission and Competition Win

Our final submission was based on the predictions from the best-performing model. We successfully achieved the lowest error rate on the test set, leading to our first-place position in the competition.

## Key Deliverables

- **Jupyter Notebook**: Containing all PyTorch code with detailed explanations and markdown text.
- **Model Checkpoint**: `checkpoint.pth`, with all necessary information to retrieve the best model and predictions.
- **Report**: A comprehensive PDF report containing plots of training/validation errors, hyperparameter tables, and profit analysis of the iBuyer business model based on predicted prices.

## Conclusion

Our winning approach in the House Price Prediction Competition demonstrated the effectiveness of meticulously analyzing the dataset, carefully designing and tuning the multilayer perceptron models, and rigorously validating their performance. This success not only highlights our technical proficiency but also our ability to apply theoretical knowledge to solve real-world problems in the dynamic field of real estate pricing.

---

**Note**: This README is part of the documentation for our winning submission in the House Price Prediction Competition and is intended for informational purposes.
"""


