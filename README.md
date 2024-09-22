
# Decision Tree Classification - DonorsChoose Dataset

This project applies **Decision Tree Classification** to predict whether a project proposal on DonorsChoose.org will be approved. The assignment includes hyperparameter tuning and evaluation using AUC and cross-validation.

## Dataset
- **DonorsChoose.org project proposals**.
- **Features**: Project titles, essays, resource summaries, teacher and school metadata.
- **Target**: Binary classification for project approval (1: approved, 0: not approved).

## Key Features
- **Text Processing**:
  - Preprocessed essays and titles using TF-IDF and Word2Vec.
  
- **Categorical Data**:
  - One-hot encoded features like teacher prefix, project categories, and school state.

- **Numerical Data**:
  - Normalized price, quantity, and previously submitted project counts.

## Modeling
- **Decision Tree Classifier**:
  - Performed hyperparameter tuning for maximum depth and minimum sample split.
  - Evaluated model performance using AUC scores and plotted ROC curves.
  - Visualized results using 3D plots and heatmaps for hyperparameter values.

## Results
- **Best AUC**: 0.67 on cross-validation data with a depth of 10 and a minimum sample split of 500.
- **Final Model**: Decision tree with balanced class weights and optimized hyperparameters.

## Conclusion
Decision Trees provide a decent performance in predicting project approval, with proper tuning improving accuracy and AUC scores.

